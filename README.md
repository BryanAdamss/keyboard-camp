# keyboard-camp

> 键盘侠训练营

- https://www.wolai.com/cuixiaorui/f5fvBC5pJiRhZumGE4esYr
- https://learn.cuixueshe.com/p/t_pc/course_pc_detail/camp_pro/course_2Eo5kBtrovv2UqWVy75SmYZP6UM

## 高频

### vim

- 移动
  - `hjkl`
  - `shift+j`+`shift+k`
  - `w/b`单词间导航
  - `ctrl+f/b` 下上翻页
  - `zz`当前行置于中间
  - `gg`移动到文件首
  - `行数+gg`跳到指定行
  - `gd`跳转到定义/引用处
  - 跳转历史栈中移动
    - `ctrl+o/i`回到上/下一个记录
- 插入
  - `i`光标前
  - `a`光标后
  - `A`行尾
  - `o`换行插入
  - `ea`在单词结尾插入
- 拷贝/剪切(删除)/粘贴/替换
  - `yiw`拷贝光标所在单词
  - `yy`拷贝当前行
  - `dd`剪切当前行
  - `diw`剪切光标所在单词
  - `cc`剪切当前行并进入插入模式
  - `x`删除单个字符
  - `dL`删除到行尾
  - `dae`删除当前文本文件所有内容
  - `p`粘贴
  - `r/R`替换单个或多个字符
- 撤销/恢复
  - `u` 撤销
  - `ctrl+r` 恢复
- 框选
  - `viw`选中当前单词
  - `V`选中当前行
  - `V`配合移动或`ctrl+v`进入多行编辑
  - `gb`快速选中多个当前单词,配合`A`进入多选编辑
- 查找
  - `f+{char}{char}`
  - `;`和`,`结果中跳转
- 手动替换
  - `f+{char}{char}`先替换
  - `cw`改成替换后的
  - 用点重复
- 替换包裹字符
  - `c+s+双引号+反引号`将双引号换为反引号
  - `y+s+iw+{`在当前字符外加上花括号
- 替换字符串
  - 替换公式`:[range]s[ubstitute]/{pattern}/{string}/[flags]`
  - `:%s/node2?js/java/gc`全文替换`nodejs`和`node2js`为`java`,替换时确认
- 大小写转换

  - `normal`模式
    - `guiw`将当前单词转为全小写
    - `gUiw`将当前单词转为全大写
  - 可视化模式
    - `viwU`将当前单词转为全大写
  - `~`大小写互换

- 注释
  - `gc+范围`单行注释
    - `gcL`注释当前行
  - `gC+范围`block 注释
  - 可视化模式下,范围可忽略
- 删除一个函数
  - `daI`改键后为`dai`,适用光标在函数体内
  - `V$%d`,适用光标在函数声明头处

### vscode

- 窗口管理/移动
  - `command+\`新建
  - `command+w`关闭文件
  - `command+option+t`关闭当前窗口其他文件
  - `ctrl+;`切换到`file explorer`
  - `ctrl+'`切换到`editor`
- 弹窗 dialog
  - `Don't Save` ⌘D or ⌘⌫
  - `Delete*` ⌘⌫
  - `Cancel` Esc
  - `Save` ⌘S or Enter
- 增/删/重命名,文件和文件夹
  - `file explorer`区域
    - 增,文件/文件夹分别用`a`和`shift+a`
    - 删,文件/文件夹用`d`
    - 重命名,文件/文件夹用`r`
  - `editor`区域
    - 增,文件/文件夹分别用`<Leader>+n+f`和`<Leader>+n+d`
- 搜索
  - `shift+command+f`全局搜索
  - `command+shift+o`在当前文件中搜索,以`@`开头
    - 在`@`后可加上`:`搜索能让结果分类
  - `ctrl+tab`最近文件切换
- 编码
  - `coomand+点`show code action
  - `ctrl+点`参数提示
  - 跳转到下一个错误处`f8`
  - `command+f2`选中所有当前单词
- 文件
  - `command+k+r`在`finder`中显示
  - `command+k+p`拷贝当前文件路径
- 重构
  - 重命名方法/变量`<Leader>+r+n`
- 终端
  - `ctrl+,`打开
  - `cmd+k`或`clear命令`清屏
  - `cmd+\`左右分屏(同分窗口一样)
  - `cmd+[/]`分屏切换
  - `shift+alt+q`杀死当前终端实例`
  - `shift+alt+n`新建终端实例
  - `shift+cmd+[/]`多终端实例窗口切换
- `gh`悬浮提示

### Vimium c

- `?`帮助页面
- 移动
  - `j/k/u/d`上下滚动
  - `gg`移动到头部
  - `f`显示标记点,点击后在当前页面打开
  - `gi`聚集搜索框
- 标签
  - `J/K`标签页切换
  - `p`将剪切板中内容(url/文本...)在当前`tab`打开
  - `T`在所有标签页中搜索(可跨多窗口)
  - `x`关闭当前标签,`X`恢复最近关闭标签
  - `^`或`g[`切换到最近访问的上一个标签页
  - `t`新开标签页
  - `yt`复制当前标签页
  - `W`移动当前标签页到下一个窗口
  - `<<`和`>>`左移/右移标签页
  - `alt+p`固定/取消固定标签页
- `H/L`后退/前进
- `yy`拷贝当前页面 url
- `yv`进入文本选择模式
- 搜索&查找
  - `o`多功能搜索
  - `b`收藏夹搜索
  - `ge`显示搜索框并编辑当前网址
  - `/`进入页内查找模式
    - `n`在页内查找下一处
    - `N`在页内查找上一处

### devtools

- 打开`f12`/`cmd+opt+i`/`cmd+opt+j`/`cmd+opt+c`
- `ctrl+反引号`聚集`console`面板
- `cmd+k`清空`console`
- `ctrl+p`搜索文件
- `cmd+[/]`切换面板
- debug
  - `cmd+b` toggle 断点
  - `cmd+'`或`f10` StepOver
  - `cmd+;`或`f11` StepInto
  - `cmd+\`或`f5` 跳到下一个断点
  - `cmd+f8` 激活/失活所有断点
  - `cmd+shift+e`打印选中代码
  - `shift+cmd+o`列出当前文件所有函数
  - `ctrl+g` 跳转到指定行

### iTerm2

- 分屏
  - `cmd+反引号`左右
  - `cmd+shift+反引号`上下
  - `cmd+[/]`切 j 换
- 标签
  - `cmd+t`新建
  - `cmd+w`关闭
  - `opt+数字/方向`切换
  - `cmd+shift+方向`移动标签顺序

## Mac

- 全局
  - `cmd+,`app 设置
  - `cmd+q`退出 app
  - `cmd+m`最小化当前窗口
  - `cmd+反引号`同一个`app`多窗口切换
  - `ctrl+cmd+f`全屏
- 文本快捷键
  - `alt+left/right`向左/右移动一个单词
  - `alt+backspace`向前删除一个单词
  - `ctrl+d` 删除光标右边一个字符
  - `shift+alt+left/right`向左/右选中一个单词
- `finder`
  - `cmd+[/]` 文件夹前进后退
  - `cmd+d` 复制当前文件或文件夹
  - `cmd+i` 文件或文件夹信息
  - `cmd+shift+n`创建文件夹
  - `cmd+del`删除文件或文件夹
  - `cmd+n` 新开一个`finder`

### obsidian

- 移动`h/j/k/l/H/J/K/L`
- `[[`给选中文字加上双链
- `cmd+反引号`分屏
- `shift+上/下/左右` 多分屏切换
- `cmd+shift+t` 恢复关闭的文件
- `cmd+k`给选中文字加链接
- `alt+down/up` 移动行
- `![[` 直接嵌入某个资源(图片/音频/视频等)
- `cmd+shift+n`选中内容创建新笔记
- `cmd+[/]` toggle left/right sidebar
- `cmd+opt+r` 在`finder`中展示
- `cmd+f` 搜索当前文件或用`vim`的`/`
- `cmd+opt+f` 搜索+替换
- `cmd+shift+f` 全局搜索

### alfred

- `file-search`
  - `space`或`'` 搜索文件
  - 输入`find`可查找文件,`enter`可打开文件所在文件夹,可直接用`cmd+enter`代替 **推荐**
  - 输入`in`可进入内容搜索 **推荐**
  - 输入`tags`可用`tag`搜索
- `web-search`
  - 输入关键字,然后用`ctrl+enter`触发浏览器搜索
- 浏览器书签搜索
  - 输入`bm`触发
- 特定网站搜索
  - 自带`gg`->`google`
  - 自定义
    - `ghs`->`https://github.com/search?q={query}`
    - `npm`->`https://www.npmjs.com/search?q={query}`
    - `bb`->`https://search.bilibili.com/all?keyword={query}`

### Moon

- `opt+cmd+left/right/up/down` 左/右/上/下半屏
- `opt+-` move to next display
- `opt+9/0` 自定义屏幕快照

### MouseCatch

- `cmd+1/2/3` 主/次/副屏
