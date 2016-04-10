# 一个 iOS 开发者的 OS X 工作环境

## 目录
1. [OS X](#1-os-x)
2. [常用工具](#2-常用工具)
    - 2.1 [Alfred](#21-alfred)
        - [推荐 Alfred workflow](#推荐alfred-workflow)
    - 2.2 [Moom](#22-moom)
    - 2.3 [Jitouch](#23-jitouch)
    - 2.4 [OmniFocus](#24-omnifocus)
    - 2.5 [Path Finder](#25-path-finder)
    - 2.6 [PopClip](#26-popclip)
    - 2.7 [1Password](#27-1password)
    - 2.8 [CheatSheet](#28-cheatsheet)
    - 2.9 [Eudic 欧路词典](#29-eudic-欧路词典)
    - 2.10 [其他常用工具](#210-其他常用工具)
    - 2.x [Finder 空格文件预览插件](#finder-文件预览插件)
    
3. [开发工具](#3-开发工具)
    - 3.1 [Homebrew](#31-homebrew)
    - 3.2 [iTerm2](#32-iterm2)
        - [常用快捷键](#常用快捷键) 
    - 3.3 [zsh](#33-zsh)
    - 3.4 [基础命令](#34-基础命令)
    - 3.5 [SublimeText 3](#35-sublimetext-3)
    - 3.6 [其他开发工具](#36-其他开发工具)
4. [chrome 插件及 web 应用](#4-chrome-插件及-web-应用)
5. [团队协作工具](#5-团队协作工具)

## 1. OS X

- 关闭 Dock 的 Magnification，将 Dock 位置移到左侧。
- 关闭 微信、QQ 的弹窗通知
- 键盘快捷键设置中开启`全键盘控制`
- 开启 Magic Mouse 的所有手势，开启 Trackpad 的所有手势

## 2. 常用工具

### 2.1 Alfred

[Alfred](https://www.alfredapp.com/)，快速启动工具，推荐购买升级包，快捷键设为 alt + j

#### 推荐alfred-workflow:
- Baidu-Map, # *bmap 鼓浪屿*, 搜索鼓浪屿相关地址列表
- Caffeinate Control, # *caff 1h*, 1小时内不进入待机状态
- Chrome Bookmarks, # *cb ios*, 搜索收藏夹内包含 ios 的收藏
- Chrome History, # *ch ios*, 搜索 chrome 历史访问记录中包含 iOS 标题的访问
- CocoaPods, # *pod yykit*, 在 cocoapods 中搜索 yykit
- colors, # *#60aa82*, *hsl*, 显示颜色、转换颜色表示、显示拾色器
- CountDown, # *timer 25m*, 简易的番茄时间计时器
- Dash, # *iOS UIView*, 在 Dash 中的 iOS channel 搜索 UIView
- Douban, # *book iOS*搜索 iOS 图书， *movie 豪斯* 搜索豪斯
- encode-decode, # base64 encode/decode
- Evernote
    - Search:
        - ens keyword, 搜索 evernote
        - ens @ , to search in a selected notebook.
        - ens # , to search notes with a selected tag.
        - ent, Search in Notes Titles
        - enr, Search Reminders Notes
        - entodo, Search todo notes
        - enrec, Search Last Updated Notes
        - enu, Search Notes with URL
        
    - Create:
        - enn, Create New note.
        - typenote, Type a New note, Notebook: (default) | Tags: (none) | Reminder: (none) | Note: (type it). 
        
- Finder-Settings, # Finder Settings & desktop settings
- flushdns, 
- Github repos, # Search your github repositories
- HTTP-codes, # *http 400*, 返回 http 编码值义
- ip-address, # *ip*, 返回当前 ip
- kill-process, # 
- Last+changed+files, # *.last*, list last changed files.
- New OmniFocus Task, # Omnifocus Action! @Context ::Project #Start #Due $Duration //Note
- Simulator-Folders, 
- sublime-text,
- Timestamp,  # 标准日期转换
- Wi-Fi-Toggle, # Wifi 控制
- Workflow-Search, # Alfred workflow 搜索

### 2.2 Moom

[Moom](https://manytricks.com/moom/)，窗口尺寸快速管理，配合快捷键可快速平铺多个应用程序窗口。
keyboard 设置，方便以可视化的模式变更窗口大小：

- Trigger keyboard control with hot key:  ⌥ + 9, ☑ show cheat sheet, ☑ repeat to show grid.
![moom-keyboard](https://github.com/EuanChan/set-up-mac/blob/master/screenshot/screenshot-moom-keyboard.png)
    
- 自定义快捷键，方便快速在窗口最大化、还原、以半屏的方式展示之间切换，方便在多个显示器里快速布局窗口。
    - ⌥ + 1, move & zoom, 最大化窗口.
    - ⌥ + 2, revert to original dimensions. 还原大小
    - ⌥ + 3, move & zoom, 最大化到当前窗口左半屏幕
    - ⌥ + 4, move & zoom, 最大化到当前窗口右半屏幕
    - ⌥ + 0, move to other display, ☑ Resize proportionally, ☑ Loop through displays.
    ![moom-custom](https://github.com/EuanChan/set-up-mac/blob/master/screenshot/screenshot-moom-custom.png)

### 2.3 Jitouch
[Jitouch](https://www.jitouch.com/)，触摸板/Magic Mouse手势增强

### 2.4 OmniFocus
[OmniFocus](https://www.omnigroup.com/omnifocus)，主力任务管理工具，适合多任务、多环境并进时的复杂任务管理，配合 iPhone 版使用

### 2.5 Path Finder
[Path Finder](http://www.cocoatech.com/pathfinder/)，替代系统 Finder

### 2.6 PopClip
[PopClip](https://pilotmoon.com/popclip/)，选中文本后弹出快捷操作（搜索、翻译、新建OmniFocus任务等）
    
### 2.7 1Password
[1Password](https://agilebits.com/onepassword/mac)，配套 iOS 版使用，管理常用密码

### 2.8 CheatSheet
[CheatSheet](http://www.mediaatelier.com/CheatSheet/)，快速查看当前程序的快捷键列表，默认的快捷键是长按`⌘`

### 2.9 Eudic 欧路词典
[EuDic 欧路词典](http://www.eudic.net/eudic/mac_dictionary.aspx)  
支持柯林斯词典，支持词库导入。分享两个词典
- [英语常用词疑难用法手册.mdx](http://pan.baidu.com/s/1nt8b6dj)
- [葛传椝英语惯用法词典.mdx](http://pan.baidu.com/s/1dDqGP1Z)

### 2.10 其他常用工具
- [Evernote](https://evernote.com/)，使用国际版，包含分享功能
- [Quiver](http://happenapps.com/#quiver)，Evernote 主要用于笔记收藏和手机记事，Quiver 主要用于代码、工作笔记
- [Day One](http://dayoneapp.com/)，主要用于写私人日记
- [ArcSoft Photo+](http://www.arcsoft.jp/photoplus/features.html) Mac 上目前找到的最顺手的快速浏览图片应用 
- [Dropbox](https://www.dropbox.com/)
- [iThoughtsX](http://toketaware.com/ithoughts-osx)，Mac 版脑图工具，更常用web的话推荐[百度脑图](http://naotu.baidu.com/)
- [Lantern](https://getlantern.org/)，Open Internet for Everyone，遇上过几次 vpn 被封，现在的主力工具  
- [Movist](https://itunes.apple.com/us/app/movist/id461788075?mt=12)，主力电影播放器，怀念windows QQ影音
- [Reeder](http://reederapp.com/mac/)，RSS 阅读
- [RescueTime](https://www.rescuetime.com/)，记录个人应用程序使用时间、浏览网站时间，统计分析个人工作习惯，辅助改善工作效率
- [TeamViewer](https://www.teamviewer.com/en/index.aspx)，跨平台远程协助工具

### Finder 文件预览插件
先安装 [brew cask](#31-homebrew)。然后安装[常用文件预览插件](https://github.com/sindresorhus/quick-look-plugins)，增强 Mac 的文件预览功能。
- QLColorCode (代码高亮) `brew cask install qlcolorcode`
- QLStephen (预览无拓展名文本文件，如 README) `brew cask install qlstephen` 
- QLMarkdown (预览 markdown 文件) `brew cask install qlmarkdown`
- QuickLookJSON (预览 JSON 文件) `brew cask cask install quicklook-json`
- BetterZipQL (预览 zip 包内容) `brew cask install betterzipql`
- QLImageSize (预览图片分辨率、大小) `brew cask install qlimagesize`
- WebP (预览 WebP 图片) `brew cask install webpquicklook`
- Suspicious Package (预览 pkg 包目录) `brew cask install suspicious-package`
- ProvisionQL (预览 iPa 包信息) `brew cask install provisionql`

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


### 3.2 iTerm2
终端使用 [iTerm2](https://www.iterm2.com/)，代替系统 Terminal。方便支持主题，画面分隔，自定义快捷键

个人习惯开启全局呼出快捷键，快速显示隐藏 iTerm，设置为 `⌘`+`.` ，在 profile 的 key 标签页，把`Left option (⌥) key acts as`和`Right option (⌥) key acts as`都设置成`+ESC`，更多设置可以参考 [打造好用的终端](http://imwuyu.me/talk-about/cool-iterm2.html/)。

#### 常用快捷键：
```
### Editor
- Ctrl + r          history reverse search
- Ctrl + s          history forward search
- Ctrl + g          Escape from history searching mode
- cmd + ;           autocomplete
- cmd + shift + h   paste history

- Ctrl + a / e      beginning/end of line
- Ctrl + f / b      forward/back 1 char
- Ctrl + p / n      previous/next history
- Ctrl + d / h      delete current/previous char
- Ctrl + w          delete the word behind point
- Ctrl + k          delete text from the point to the end of the line
- ctrl + u          delete current line

- Alt + f / b       forward/back 1 word
- Alt + d           delete the word after the cursor
- Alt + w           delete text from the point to the beginning of the line

- cmd + k           clear buffer
- Ctrl + l          clear screen

- !!                Execute last command in history
- !abc              Execute last command in history beginning with abc
- !abc:p            Print last command in history beginning with abc

### Process Control
- Ctrl + C          Interrupt/Kill whatever you are running (SIGINT)
- Ctrl + l          Clear the screen
- Ctrl + s          Stop output to the screen (for long running verbose commands)
- Ctrl + q          Allow output to the screen (if previously stopped using command above)
- Ctrl + D          Send an EOF marker, unless disabled by an option, this will close the current shell (EXIT)
- Ctrl + Z          Send the signal SIGTSTP to the current task, which suspends it.
                    To return to it later enter fg 'process name' (foreground).

### Tab Navigation
- cmd + t               open new tab
- cmd + shift + ] / [     next/previous tab

### Pane navigation
- cmd + d           split pane left-right 
- cmd + shift +d    split pane top-bottom 
- cmd + ] / [       next/previous pane    

### Search
- cmd + f           open search bar
- cmd + g           find next

### Zooming / Font Resize
- cmd + +           make font larger
- cmd + -           make font smaller

### Input to all panes
- cmd + alt + i     input to all panes in current tab
```

### 3.3 zsh 
使用 zsh 代替系统默认 shell，详情[终极 shell](http://macshuo.com/?p=676)。

安装 [oh my zsh](https://github.com/robbyrussell/oh-my-zsh) 来快速配置 zsh。

oh my zsh 插件，通过 ~/.zshrc 的 plugins 配置
- autojump
使用 brew 安装
```
brew install autojump
```
> Add the following line to your ~/.bash_profile or ~/.zshrc file (and remember
to source the file to update your current session):
  [[ -s $(brew --prefix)/etc/profile.d/autojump.sh ]] && . $(brew --prefix)/etc/profile.d/autojump.sh

根据 brew 安装提示，在.zshrc 中添加配置.

#### zsh + oh-my-zsh + 常用插件使用
- 历史记录功能， 输入 git 然后使用上下箭头可以翻阅执行过的 git *** 命令
- 更全面的补全：路径、命令、命令参数、插件内容补全。按 tab 键触发补全，按两下 tab 键列出所有补全项，使用 *ctrl + n/p/f/b* 在补全项间切换。
- 智能跳转：结合 autojump，zsh 会记录访问过的目录，通过 j + '目录名' 即可直接进行目录跳转，且目录名支持模糊匹配和自动补全。可以使用 j -s 查看记录及权重。
- 历史目录浏览、跳转： 输入 d，列出当前会话的目录访问记录，输入序号可直接跳转
- 当前目录，上级目录跳转可省略 cd 
- 通配符搜索：*ls -l **/*.sh*， 文件少时可以代替 find 命令

### 3.4 基础命令
- [tldr](http://tldr-pages.github.io/)，没耐心看 man 时，可使用 tldr 方便查看命令基本用法。
    ![tldr](https://github.com/EuanChan/set-up-mac/blob/master/screenshot/screenshot-tldr.png)

- man, eg. man grep

- stree，设置从命令行启动 SourceTree 的快捷方式

    set "alias stree='open -a SourceTree'" in .zshrc first, launch git repo in SourceTree with "stree /path-of-repo"
    eg: "stree .", 在 SourceTree 打开当前目录

- open, 打开 Finder, eg "open ./" 在 Finder 打开当前目录
- st, 快捷启动 SublimeText

    eg: "st ." open current path in SublimeText

- [autojump](https://github.com/wting/autojump#usage)  
    ![autojump](https://github.com/EuanChan/set-up-mac/blob/master/screenshot/screenshot-autojump.png)
    - j foo, Jump To A Directory That Contains foo.
    - jo foo, Instead of jumping to a directory, you can open a file explorer window.

- grep, Matches patterns in input text.
    ```sh
    grep -i something file_path     # Search without case-sensitivity
    grep -r something .             # Search recursively in current directory for an exact string
    egrep ^regex$ file_path         # Use a regex
    grep -C 3 something file_path   # See 3 lines of context
    grep -c something file_path     # Print the count of matches instead of the matching text
    grep -n something file_path     # Print line number for each match
    cat file_path | grep something  # Use the standard input instead of a file
    ls -l | grep -i name            # list the files filename contain "name"
    ```

- find
    ```
    find root_path -name '*.py'                              # Find files by extension 
    find root_path -path '**/lib/**/*.py'                    # Find files matching path pattern 
    find root_path -name '*.py' -exec wc -l {} \;            # Run a command for each file, use {} within the command to access the filename
    find root_path -name '*.py' -mtime -1d                   # Find files modified since a certain time                       
    find root_path -size +500k -size -10MB -iname '*.TaR.gZ' # Find files using case insensitive name matching, of a certain size
    find root_path -name '*.py' -mtime -180d -delete         # Delete files by name, older than a certain number of days
    find root_path -empty                                    # Find empty files or directories 
    find root_path -name '*.py' -or -name '*.r'              # Find files matching more than one search criteria 
    ```

- file operate  
    - cp, -r        # "cp file.html{,.backup}", make a backup.
    - mv,
    - rm, -i -f -r

- ps, Information about running processes.
    ```
    ps aux | grep string    # Search for a process that matches a string
    ps aux                  # 查看系统所有的进程数据  
    ps ax                   # 查看不与terminal有关的所有进程  
    ps -lA                  # 查看系统所有的进程数据  
    ps axjf                 # 查看连同一部分进程树状态 
    ```

- command line + &      # Put command line run in background.
- jobs -l               # List all task status in the background.
- fg %jobnumber         # put background task to foreground.
- bg %jobnumber         # put foreground task to background.
- kill
    ```
    kill -signal %jobnumber     # get jobnumber from *jobs* command
    kill -signal PID            # get PID from *ps* command
    
    signal values:
    1：SIGHUP，启动被终止的进程  
    2：SIGINT，相当于输入ctrl+c，中断一个程序的进行  
    9：SIGKILL，强制中断一个进程的进行  
    15：SIGTERM，以正常的结束进程方式来终止进程  
    17：SIGSTOP，相当于输入ctrl+z，暂停一个进程的进行  
    ```

### 3.5 SublimeText 3
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

### 3.6 其他开发工具
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

- [Bugtags](https://www.bugtags.com/), 需求反馈、bug 收集管理工具
- [BearyChat](https://bearychat.com/)，团队沟通工具，团队网络环境较好时推荐用`Slack`
- [Worktile](https://worktile.com/)，目前团队使用的协作工具，团队网络状况良好时推荐 Trello + Google Apps for work.
- [Slack](https://slack.com/)，团队协作沟通工具，配合机器人与其他团队协作工具，生产力工具是时候抛弃QQ群而使用slack
- [Trello](https://trello.com/)，团队协作工具，抛开网络环境不谈体验最好

