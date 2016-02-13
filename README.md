# 一个 iOS 开发者的 OS X 工作环境

## 目录
1. [OS X](#1-os-x)
2. [常用工具](#2-常用工具)
3. [开发工具](#3-开发工具)
    - [Homebrew](#31-Homebrew)
    - [iTerm2](#32-Iterm2)
    - [SublimeText3](#33-SublimeText-3)
    - [其他开发工具](#34-其他开发工具)
4. [chrome 插件及 web 应用](#4-chrome-插件及-web-应用)
5. [团队协作工具](#5-团队协作工具)

## 1. OS X

- 关闭 Dock 的 Magnification，将 Dock 位置移到左侧。
- 关闭 微信、QQ 的弹窗通知
- 键盘快捷键设置中开启`全键盘控制`
- 开启 Magic Mouse 的所有手势，开启 Trackpad 的所有手势

## 2. 常用工具

- [1Password](https://agilebits.com/onepassword/mac)，配套 iOS 版使用，管理常用密码
- [Alfred](https://www.alfredapp.com/)，快捷键设为 alt + j

    安装的 workflow:
    - Baidu-Map
    - Chrome History
    - CocoaPods
    - colors
    - Douban
    - encode-decode
    - Finder-Settings
    - flushdns
    - GithubSearch
    - HTTP-codes
    - ip-address
    - kill-process
    - Last+changed+files
    - meituanSuggest
    - Network Info
    - New OmniFocus Task
    - Simulator-Folders
    - Site+Search
    - stackoverflowSearch
    - sublime-text
    - Timestamp
    - Wi-Fi-Toggle
    - Workflow-Search
    - zhihu_Search

- [ArcSoft Photo+](http://www.arcsoft.jp/photoplus/features.html) Mac 上目前找到的最顺手的快速浏览图片应用，静等 Picasa 更新浏览图片功能 
- [Caffeine](https://itunes.apple.com/en/app/caffeine/id411246225?mt=12)，离开电脑时想不自动待机时使用
- [CheatSheet](http://www.mediaatelier.com/CheatSheet/)，快速查看当前程序的快捷键列表，默认的快捷键是长按`⌘`
- [Day One](http://dayoneapp.com/)，写私人日记
- [Dropbox](https://www.dropbox.com/)
- [EuDic 欧路词典](http://www.eudic.net/eudic/mac_dictionary.aspx)  
    
    支持柯林斯词典，支持词库导入。分享两个词典
    + [英语常用词疑难用法手册.mdx](http://pan.baidu.com/s/1nt8b6dj)
    + [葛传椝英语惯用法词典.mdx](http://pan.baidu.com/s/1dDqGP1Z)

- [Evernote](https://evernote.com/)，使用国际版，包含分享功能
- [huhamhire-hosts](https://github.com/huhamhire/huhamhire-hosts)，更新 google 等服务的 ip
- [instacalc](http://instacalc.com/)，计算器
- [iThoughtsX](http://toketaware.com/ithoughts-osx)，Mac 版脑图工具，更常用web的话推荐[百度脑图](http://naotu.baidu.com/)
- [Jitouch](https://www.jitouch.com/)，触摸板/Magic Mouse手势增强
- [Lantern](https://getlantern.org/)，Open Internet for Everyone，遇上过几次 vpn 被封，现在的主力工具  
- [Moom](https://manytricks.com/moom/)，窗口尺寸快速管理，配合快捷键可快速平铺多个应用程序窗口
- [Movist](https://itunes.apple.com/us/app/movist/id461788075?mt=12)，主力电影播放器，怀念windows QQ影音
- [OmniFocus](https://www.omnigroup.com/omnifocus)，主力任务管理工具，适合多任务、多环境并进时的复杂任务管理，配合 iPhone 版使用
- [Path Finder](http://www.cocoatech.com/pathfinder/)，替代系统 Finder
- [PopClip](https://pilotmoon.com/popclip/)，选中文本后弹出快捷操作（搜索、翻译、新建OmniFocus任务等）
- [Reeder](http://reederapp.com/mac/)，RSS 阅读
- [RescueTime](https://www.rescuetime.com/)，记录个人应用程序使用时间、浏览网站时间，统计分析个人工作习惯，辅助改善工作效率
- [TeamViewer](https://www.teamviewer.com/en/index.aspx)，跨平台远程协助工具

## 3. 开发工具

### 3.1 Homebrew
安装包管理工具 [Homebrew](http://brew.sh/)
在安装 Homebrew 之前，需要将 Xcode Command Line Tools 安装完成，这样你就可以使用基于 Xcode Command Line Tools 编译的 Homebrew。

在 terminal 中复制以下命令（不包括 $），跟随指引，将完成 Hombrew 安装。
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

安装完后，运行以下命令，确保 brew 运行正常。
```
$ brew doctor
```
安装完成后，Homwbrew 会将本地 /usr/local 初始化为 git 的工作树，并将目录所有者变更为当前所操作的用户，将来 brew 的相关操作不需要 sudo 。

#### Homebrew cask
安装 brew-cask，通过 brew-cask 快速安装、管理图形界面程序
```
$ brew tap caskroom/cask  // 添加 Github 上的 caskroom/cask 库
$ brew install brew-cask  // 安装 brew-cask
```

- [文件预览插件](https://github.com/sindresorhus/quick-look-plugins)
有些插件可以让 Mac 上的文件预览更有效，比如语法高亮、markdown 渲染、json 预览等等。

### 3.2 iTerm2

- [iTerm2](https://www.iterm2.com/)，替代系统 Terminal。

    个人习惯开启全局呼出快捷键，快速显示隐藏 iTerm，设置为 `⌘`+`.`  
    bash 常用快捷键： [详细版](http://ss64.com/bash/syntax-keyboard.html)
    - ctrl + a/e, 将光标移到行开头/行结尾
    - ctrl + b/f, 将光标往左移/右移一个字符
    - alt + b/f, 将光标左移/右移一个单词（需在 profile 的 key 标签页，把`Left option (⌥) key acts as`和`Right option (⌥) key acts as`都设置成`+ESC`

- [Oh My Zsh](http://ohmyz.sh)
    个人安装的插件：git, autojump, sublime

### 3.3 SublimeText 3
[Sublime Text](https://www.sublimetext.com/)，Xcode 外的主力编辑工具 个人安装的插件：

- All Autocomplete，搜索所有打开文件来寻找匹配提示词
- BracketHighlighter, 匹配括号、引号
- ConvertToUTF8，查看非 utf-8 编码的文档
- Git
- GitGutter, 在侧边槽显示 git diff
- LiveReload
- MarkdownEditing
- Pretty JSON
- SideBarEnhancement，侧边文件夹栏增加常用右键菜单
- SideBarGit，侧边文件夹栏增加 git 常用命令
- SublimeLinter，高亮错误代码

### 3.4 其他开发工具
- [Beyond Compare](http://www.scootersoftware.com/features.php) ，离开 windows 平台时念念不忘的比较工具，已有 Mac 版
- [Charles](http://www.charlesproxy.com/)，http 抓包工具
- [CodeRunner](https://coderunnerapp.com/)，支持多语言的快速代码编写、运行工具，主要用于小段c/cpp/python代码的编写
- [Dash](https://kapeli.com/dash)，常用 API 文档浏览器，代码片段管理
- [FauxPas](http://fauxpasapp.com/)，iOS Mac 工程代码静态检查
- [iFunBox](http://i-funbox.com/ifunboxmac/)，iPhone/iPad 文件夹管理
- [Mark Man](http://www.getmarkman.com/)，设计稿标注、测量工具
- [Little Snitch](https://www.obdev.at/products/littlesnitch/index.html)，监控、控制应用程序的网络进出请求
- [Liya](http://cutedgesystems.com/software/liya/)，数据库文件查询管理工具，支持 SQLite, MySQL, PostgreSQL 数据库。
- [Parallels Desktop](http://www.cocoatech.com/pathfinder/)，虚拟机
- [PyCharm](www.jetbrains.com/PyCharm‎)，Python 开发 IDE
- [Pngyu](http://nukesaq88.github.io/Pngyu/)，使用 pngquant 引擎的一款有损 png 图片压缩工具
- [Reveal](http://revealapp.com/)，iOS Debug 工具，辅助实时查看当前运行 iOS App 的视图层
- [SimPholders](https://simpholders.com/)，帮助快速访问 iPhone 模拟器，重置库和文件
- [Sketch](http://www.sketchapp.com/)，界面设计工具
- [SourceTree](https://www.sourcetreeapp.com/)，比较过几个 GUI git 工具，Mac 下使用最顺手的 git 工具。建议先熟悉 git command 后再使用GUI工具。
- [Yummy FTP](http://www.yummysoftware.com/)，FTP+SFTP+FTPS 客户端

## 4. Chrome 插件及 web 应用

- 1Password
- [AdBlock](https://chrome.google.com/webstore/detail/adblock/gighmmpiobklfepjocnamgkkbiglidom), 广告拦截插件
- [Awesome Screenshot](https://chrome.google.com/webstore/detail/awesome-screenshot-screen/nlipoenfbbikpbjkfpfillcgkoblgpmj)，网页截图插件
- [Awesome Screenshot App](https://chrome.google.com/webstore/detail/awesome-screenshot-app/mfpiaehgjbbfednooihadalhehabhcjo)，窗口截图、标注修饰 web App
- [Better History](https://chrome.google.com/webstore/detail/better-history/obciceimmggglbmelaidpjlmodcebijb), 增强历史网页浏览记录
- [Evernote Web Clipper](https://chrome.google.com/webstore/detail/evernote-web-clipper/pioclpoplcdbaefihamjohnefbikjilc) Evernote 快速剪贴插件，剪贴后定期整理分类到各个不同子笔记本
- [JSON Editor](https://chrome.google.com/webstore/detail/json-editor/lhkmoheomjbkfloacpgllgjcamhihfaj)，JSON 查看、格式化、编辑 web App
- [JSONView](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc)，JSON 文档查看插件
- [Koding](https://koding.com/), 支持多种语言环境的在线IDE
- [LiveReload](http://livereload.com/), 使用浏览器查看正在编辑的本地文件时，自动更新变动，免去手动刷新 
- [MagicSel](https://chrome.google.com/webstore/detail/%E6%99%BA%E8%83%BD%E9%80%89%E6%8B%A9/dmobhfhmcgcceenmkcpckkffmfkkmkbf)，选中浏览器中的不同货币、单位，转换为人民币，国家标准单位
- [MarkView](https://chrome.google.com/webstore/detail/markview/iaddkimmopgchbbnmfmdcophmlnghkim), markdown 文档预览插件，支持多种格式化样式 
- [Marxico](https://chrome.google.com/webstore/detail/marxico/kidnkfckhbdkfgbicccmdggmpgogehop)，Evernote 上写 Markdown 文档的辅助 web app
- [Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop), API 测试 web App
- [Save to Pocket](https://chrome.google.com/webstore/detail/save-to-pocket/niloccemoadcdkdjlinkgdfekeahmflj), 稍后阅读插件
- [Speed Dial 2](https://speeddial2.com/), 定制chrome首页
- [StayFocused](https://chrome.google.com/webstore/detail/stayfocusd/laankejkbhbdhmipfmgcngdelahlfoji), 限制网站的最长访问时间
- [TabCloud](https://chrome.google.com/webstore/detail/tabcloud/npecfdijgoblfcgagoijgmgejmcpnhof)，将当前 chrome 窗口的所有 tab 保存，方便后续恢复继续查看
- [Yet Another Drag and Go](https://chrome.google.com/webstore/detail/yet-another-drag-and-go/hnoonkgmmnklbdehoepdjcidhjbncjmi)，拖拽 url 打开新的 tab，拖拽文字搜索
- [眼不见心不烦（新浪微博）](https://chrome.google.com/webstore/detail/%E7%9C%BC%E4%B8%8D%E8%A7%81%E5%BF%83%E4%B8%8D%E7%83%A6%EF%BC%88%E6%96%B0%E6%B5%AA%E5%BE%AE%E5%8D%9A%EF%BC%89/aognaapdfnnldnjglanfbbklaakbpejm)，屏蔽微博上的一些营销信息，减少信息干扰

## 5. 团队协作工具

- [BearyChat](https://bearychat.com/)，团队沟通工具，团队网络环境较好时推荐用`Slack`
- [Worktile](https://worktile.com/)，目前团队使用的协作工具，团队网络状况良好时推荐 Trello + Google Apps for work.
- [Slack](https://slack.com/)，团队协作沟通工具，配合机器人与其他团队协作工具，生产力工具是时候抛弃QQ群而使用slack
- [Trello](https://trello.com/)，团队协作工具，抛开网络环境不谈体验最好

