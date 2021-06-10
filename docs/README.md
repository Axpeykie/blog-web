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
* 预处理器语言使用 sass
* 包管理工具使用 yarn
* 组件库使用 element ui
* 代码检验使用 eslint
* 代码格式化使用 prettier
* 提交仓库时必须添加commit说明，格式为fix:<说明>，参考https://segmentfault.com/a/1190000017790694

## 分支说明
* master 主分支
* develop 开发分支
* f-* 新增功能分支
  * 格式：f-开发起止时间-开发者名字缩写 日常开发分支，如 f-202106070707-zwb f-202106070707-zzp
* b-* bug修复分支
  * 格式：b-开发起止时间-开发者名字缩写 日常开发分支，如 b-202106070707-zwb b-202106070707-zzp

## 开发-测试流程
1. 开发：确定开发某功能时，基于develop拉取分支，按照 f-年月日-开发者缩写 创建自己的开发分支进行开发
2. 测试：功能开发完成后合并到develop分支中进行测试
3. bug修复：在测试过程中出现bug则从develop中拉取分支进行修复，按照f-年月日-开发者缩写 创建bug分支进行修复，修复完成合并到develop中
4. 发布：develop功能实现、测试通过后合并到master进行发布
5. 有新功能重复以上过程