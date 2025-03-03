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

## 字体问题

- 如果出现字体问题，请在本人github下另一个叫`latex_demo`的项目的release中下载字体扩展包，并且放置到系统对应的文件夹中