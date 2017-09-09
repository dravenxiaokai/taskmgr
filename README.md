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