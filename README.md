# vscodeArea
默认有代码智能提示

## 调试
- 默认支持node调试，`F5`启动调试
- 若要支持网页调试，需要安装`Debugger for Chrome`

## 设置
### 用户设置
- 这种方式进行的设置，会应用于该用户打开的所有工程
- Mac $HOME/Library/Application Support/Code/User/settings.json
### 工作空间设置
工作空间是指使用VS Code打开的某个文件夹，在该文件夹下会创建一个名为`.vscode`的隐藏文件夹，里面包含着**仅适用于当前目录的**VS Code的设置
- 工作空间的设置会覆盖用户的设置
- 工作空间设置的文件保存在当前目录的`.vscode`文件夹下

### 修改设置
1. CMD+Shift+P （打开命令面板）
2. Preferences: Open User Settings 或 Preferences: Open Workspace Settings

## 插件 plugins
- coding
    - html | xml | markdown
        - Auto Close Tag
        - Auto Rename Tag
        - HTML CSS Support
        - Markdown Preview Enhanced
    - javascript | css
        - Path Autocomplete
        - Path Intellisense
        - fileheader
        - Bracket Pair Colorizer
        - SCSS Formatter
        - node-snippets
        - vetur (vue 相关)
        - Vue VSCode Snippets (vue 相关)
    - tools
        - Code Runner
        - open-in-browser
        - Live Server
        - Debugger for Chrome
        - vscode-typescript-tslint-plugin
        - Prettier - Code formatter
        - vscodevim
- git | local
    - Git History Diff
    - GitLens -- Git supercharged
- preference
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
