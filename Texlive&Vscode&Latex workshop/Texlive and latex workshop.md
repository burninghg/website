# 1. Texlive and latexworkshop 

## 1.1. Forward searching 

## 1.2. Backward searching


```
"latex-workshop.view.pdf.external.synctex.command": "C:/Program Files/SumatraPDF/SumatraPDF.exe",//你的SumatraPDF所在文件夹
"latex-workshop.view.pdf.external.synctex.args": [
    "-forward-search",
    "%TEX%",
    "%LINE%",
    "-reuse-instance",
    "-inverse-search",
    "D:\\Program Files (x86)\\Microsoft VS Code\\Code.exe", // 未配置环境变量时必须使用Code.exe的全路径, 这个是你的Vscode软件主程序所在的文件夹, 其中\\是绝对路径
    "\"D:\\Program Files (x86)\\Microsoft VS Code\\resources\\app\\out\\cli.js\" -r -g \"%f:%l\"",//如果上面Vscode的位置更改后, 这个位置也要相应的改变
    "%PDF%",
]
```

在Sumatra<kbd>设置</kbd><kbd>选项</kbd>输入
```
"D:\Program Files (x86)\Microsoft VS Code\Code.exe" "D:\Program Files (x86)\Microsoft VS Code\resources\app\out\cli.js" -r -g "%f:%l"
```
在Sumatra<kbd>设置</kbd><kbd>高级选项</kbd>搜索 <kbd>InverseSearchCmdLine</kbd>
修改对应的项为
```
InverseSearchCmdLine = "D:\Program Files (x86)\Microsoft VS Code\Code.exe" "D:\Program Files (x86)\Microsoft VS Code\resources\app\out\cli.js" -r -g "%f:%l"
```

SumatraPDF一定要从Vscode打开, 否则在SumatraPDF里面双击只会跳转到Cli.js文件[1](#14-参考文献)
![](2020-10-05-23-08-36.png)
## 1.3. 快捷键

按 <kbd>Alt</kbd>+<kbd>S</kbd>可以实现正向搜索

## 1.4. 参考文献

[1] [使用VSCode编写LaTeX](https://zhuanlan.zhihu.com/p/38178015)