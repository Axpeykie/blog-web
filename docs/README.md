## 项目结构说明
- config 环境配置
- docs 项目文档
- src 源代码
    - api 接口统一管理
    - asset 静态文件
    - components *全局*的公共组件
    - router 路由表
    - store vuex状态管理
    - utils 工具函数
    - views 页面组件

## 约定
预处理器语言使用 sass
包管理工具使用 yarn
组件库使用 element ui
代码检验使用 eslint
代码格式化使用 prettier
提交仓库时必须添加commit说明，格式为fix:<说明>，参考https://segmentfault.com/a/1190000017790694

## 分支说明
master 主分支
feature-wish 功能分支
test 测试分支
f-开发起止时间-开发者名字缩写 日常开发分支，如 f-202106070707-zwb f-202106070707-zzp

## 开发-测试流程
确定开发某功能时，基于 feature-wish 拉取分支，按照 f-年月日-开发者缩写 创建自己的开发分支进行开发。
开发完成后合并到test分支进行测试。
测试完成后合并到 feature-wish 分支，即算当前开发功能已完成，再将 feature-wish 分支合并到master分支。
开发下一个功能时，将当前 feature-wish 分支删除，重新从 master 分支创建 feature-wish 分支进行开发。