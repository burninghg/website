How to use zotero scientifically
<!--more-->

## Zotero与Zotero connector的安装
<!-- ![音标](2020-07-03-13-05-25.png) -->
Zotero是一款开源且跨平台的文献管理软件. 安装Zotero需要两个部分
- [Zotero客户端软件](https://www.zotero.org/download/)
- [Zotero Connector(浏览器插件)](https://www.zotero.org/download/)

### Zotero客户端的安装

### Zotero connector安装

### Zotero connector获取PDF

Zotero connector利用Zotero translator来实现抓取文献信息功能的, [具体内容请看这里](https://mp.weixin.qq.com/s/JA0ZPKQC4n0rznzuuVbCig)
## Zotero插件

### Zotfile

Zotfile是一款重命名文件并可以把文件传输到另一台设备的插件   

#### Zotfile的重命名功能

在菜单栏<kbd>工具</kbd><kbd>Zotfile preference</kbd>中选择<kbd>Renaming rules</kbd>, 可以得到下图所示的画面
> ![Renaming rules](https://git.nju.edu.cn/HG87/image/-/raw/master/zotero/2020-07-07-21-19-35.png)


在这里我选择的是以年份_文章名_期刊名称_作者命名的.下图为预期的命名效果
> ![Renaming sample](https://git.nju.edu.cn/HG87/image/-/raw/master/zotero/2020-07-07-21-22-29.png)

将本地文献拖到Zotero文件夹里面, Zotero会自动识别并为其创建父条目, 然后会根据网上获取的信息给你的文献命名, 但此时的命名效果并不好, 需要手动去用Zotfile命名来实现你所需要的结果.
#### 将文献同步到平板上观看
![](2020-09-29-12-37-02.png)
![](2020-09-29-12-36-55.png)
![](2020-09-29-12-37-10.png)
![](2020-09-29-12-37-17.png)
### Zotero doi manager&sci-hub

#### Zotero doi manager

使用[Zotero doi manager](https://github.com/bwiernik/zotero-shortdoi/releases)插件可以获得文件的doi信息, Zotero doi manager有三个选项
- Get shortdois
- Get longdois
- Verify and clean dois

选项里面的Get longdois和Verify and clean dois可以得到文件的Longdoi, 而Longdoi是可以被Sci-hub所识别的.

#### 配置Zotero pdf获取方式为Sci-hub

通过Sci-hub获取文献的方式有三种, 网址, 名称和Doi, 利用上面的Zotero doi manager获取文献的doi信息后, 利用Sci-hub获得文献的PDF.  
具体的配置步骤为
1. 菜单栏编辑->首选项->高级
2. 在高级菜单下的常规选项中找到设置编辑器
3. 在设置编辑器里面搜索<kbd>extensions.zotero.findPDFs.resolvers</kbd>
4. 右键点击修改, 删除默认的<kbd>[]</kbd>并修改为为下面代码所示内容, 点击保存即可.
```
{
    "name":"Sci-Hub",
    "method":"GET",
    "url":"https://sci-hub.tw/{doi}",
    "mode":"html",
    "selector":"#pdf",
    "attribute":"src",
    "automatic":true
}
```

#### 两者的配合使用方法

1. 如果Zotero connector没有获得文件的pdf, 但是在Zotero生成了文件的题录, 可以右键点击文献的题录, 点击选项<kbd>Get longdoi</kbd>或者<kbd>Verify and clean dois</kbd>来找到文献的doi![找到doi](2020-07-03-13-30-00.png)
5. 得到文献的doi后可以用sci-hub作为pdf解析器, 具体使用方法为点击右键文献题录, 点击<<kbd>找到可用的PDF</kbd>>![找到可用的pdf](https://git.nju.edu.cn/HG87/image/-/raw/master/zotero/2020-07-03-13-27-10.png) 
### Zotero Quicklook


## Zotero其他设置

### Webdav同步

Zotero可以通过Webdav进行同步, 坚果云可以实现Webdav同步, 南大Box也是有Webdav的功能的, 只需要在南大Box里新建一个Zotero文件夹, 然后按下图设置就好.
![Box](https://git.nju.edu.cn/HG87/image/-/raw/master/zotero/2020-06-24-18-30-40.png)
