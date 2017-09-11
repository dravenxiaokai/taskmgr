# taskmgr

## Angular 2+ Material 开发企业协作平台

#### [我的微博](http://weibo.com/u/3826537889?refer_flag=1001030201_&is_all=1)

## SideNav

- 用途：侧边栏导航，同时可以作为容器
- 侧滑的三种模式：over,push,side
- 一般和<md-sidenav-container>联合使用

## Toolbar

- 用途：一般用于头部、标题栏
- 通过<md-toolbar-row>可以支持多行
- 默认内部布局是支持flex的

## md-icon

- 使用图标字体，内建material icon支持
- 支持svg：通过注入MdIconRegistry和DomSanitizer完成

`this.iconRegistry.addSvgIcon('project',this.sanitizer.bypassSecurityTrustRescourceUrl('assets/img/sidebar/project.svg'))`

如果每个都需要重复调用的话，就可以做成一个工具类，在core构造中调用这个加载方法

## input

- 指令：mdInput在<md-input-container>内部，有前缀后缀
- <md-error>:只有验证不通过时才出现，对两种类型表单都是如此
- <md-hint>:当error显示时,hint会隐藏

## card

适合图文形式突出某一主题

## Button

- md-button 是以指令形式提供的
- 标准按钮：md-button,md-raised-button,md-icon-button
- 浮动按钮：md-fab,md-mini-fab
