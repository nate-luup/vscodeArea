# VsCode

VsCode 自从诞生以来，以其优异的特性迅速走红。尤其是对于前端开发小伙伴来说，几乎成为必不可少的开发工具。所以熟练掌握 VsCode 的各种使用技巧会让你的日常开发工作效率倍增。

## 基本技巧

### 快速启动

VsCode 安装后，会自动写入环境变量，终端输入`code`即可唤起 VsCode 应用程序

1. CMD+Shift+P （打开命令面板）
   - 安装命令行 `install` install 'code' command in PATH
2. 技巧参考 https://code.visualstudio.com/docs/getstarted/tips-and-tricks

### 常用快捷键

- `command + p`: 快速搜索文件并跳转，添加`:`可以跳转到指定的行
- `command + shift + p`: 根据您当前的上下文访问所有可用命令
- `ctrl + ~`: 显示隐藏终端面板
- `command + \`: 快速拆分文件编辑
- `option + 单击左键`: 添加多处光标
- `option + shift + 单击左键`: 多列选择
- `alt + 上键或下键`: 将当前行或者选中的区域上移/下移一行

### 垂直标尺

在配置文件中添加如下配置，可以增加字符数标尺辅助线

```json
"editor.rulers": [80, 120],
```

## 调试

- 默认支持 node 调试，`F5`启动调试
- 若要支持网页调试，需要安装`Debugger for Chrome`

## 设置

### 用户设置

- 这种方式进行的设置，会应用于该用户打开的所有工程
- Mac $HOME/Library/Application Support/Code/User/settings.json

### 工作空间设置

工作空间是指使用 VS Code 打开的某个文件夹，在该文件夹下会创建一个名为`.vscode`的隐藏文件夹，里面包含着**仅适用于当前目录的**VS Code 的设置

- 工作空间的设置会覆盖用户的设置
- 工作空间设置的文件保存在当前目录的`.vscode`文件夹下

### 修改设置

1. Preferences: Open User Settings 或 Preferences: Open Workspace Settings

## 插件 plugins

- coding
  - html | xml | markdown
    - Auto Close Tag
    - Auto Rename Tag
    - HTML CSS Support
    - Markdown All in One
  - javascript | css
    - Path Autocomplete
    - Path Intellisense
    - fileheader
    - Bracket Pair Colorizer
    - SCSS Formatter
    - PostCSS Language Support
    - node-snippets
    - vetur (vue 相关)
    - Vue VSCode Snippets (vue 相关)
    - React/Redux/react-router Snippets (react 相关)
    - React Bootstrap 4 Snippets (react 相关)
    - Simple React Snippets (react 相关)
    - React Hooks Snippets (react 相关)
    - Ant Design Snippets (react 相关)
    - React Native Tools (react native 相关)
  - tools
    - Auto Import
    - Code Runner
    - open-in-browser
    - Live Server
    - Debugger for Chrome
    - vscode-typescript-tslint-plugin
    - Prettier - Code formatter
    - vscodevim
    - hexdump `查看二进制的源文件`
    - Version Lens `查看package.json中依赖包的版本，并且给出最新版本提示`
- git | local
  - Git History Diff
  - GitLens -- Git supercharged
- preference
  - colorize
  - Terminal
  - Bookmarks
  - filesize
  - vscode-icons

## Q&A

1. vscode 卡顿解决办法

```
vscode 设置 - followSymlinks - 设置为false， 即可解决！

"search.followSymlinks": false
```

# reference

- [用法](https://juejin.im/post/5b123ace6fb9a01e6f560a4b)
- [Extensions](https://marketplace.visualstudio.com/)
- [自定义 snippets](https://github.com/bubucuo/ReactArticles/blob/master/react%E9%9C%80%E8%A6%81%E7%9A%84vscode%E6%8F%92%E4%BB%B6.md)
- [深入讲解 VsCode 各场景高级调试与使用技巧](https://mp.weixin.qq.com/s/YSxqD1cWZCVsEx1X9kMpZA)
