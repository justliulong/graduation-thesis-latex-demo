# latex_demo
本校可使用的论文模板

- fonts文件夹保存了可能用到的字体
- images文件夹保持所有用到的图片
- paper里的article.tex是模板代码文件
- 仓库的里面有几乎所有用得上的字体

## 安装Latex的方法是：
- 官方下载

    1、下载安装texlive环境
    https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/
    2、下载安装latex编辑器textstudio
    https://mirrors.tuna.tsinghua.edu.cn/github-release/texstudio-org/texstudio/LatestRelease/

    参考地址：https://zhuanlan.zhihu.com/p/617431548

- 使用arch系操作系统直接安装

    ```shell
    sudo pacman -S texlive
    ```
    使用vscode编辑器，安装latex-workshop插件，利用vscode编辑器来启动项目，最后运行结果会出现在 paper 文件夹下的pdf中

> 项目最近更新将单文件编译变成了多文件编译，正常情况下主文件的编译是没有问题的，但是子文件会由于找不到参考文献的bib和bst文件，将会在bibtex的编译过程中失败，所以这里使用的latex插件的编译配置方案是自定义的，这里设置了一个名为“xelatex->trybib->xelatex\*2”的配置方案，这个配置将会优先考虑编译完整流程（xelatex -> bibtex -> xelatex\*2），如果bibtex编译失败则会只使用xelatex来编译，这样的话子文件就能独立编译，只是参考文献是无法正常显示的，只有去主文件编译，参考文献才会正常出现

## 字体问题

- 如果出现字体问题，未显示可以在fonts文件夹保存了可能用到的字体寻找字体，如果还有问题，需要在仓库的 Release 中下载字体扩展包，并且放置到系统对应的文件夹中