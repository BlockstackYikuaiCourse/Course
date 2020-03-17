# Lesson 2 参考资料

- [create-react-app 简介](https://www.html.cn/create-react-app/docs/getting-started/)
- [Blockstack HelloWorld Demo 教程](https://docs.blockstack.org/browser/hello-blockstack.html)
- [gavin.id 的 core 节点数据](https://core.blockstack.org/v1/names/gavin.id)
- [gavin.id 的 profile.json](https://gaia.blockstack.org/hub/18WqH3phVrTwFCkHTA9VNeLu7fBMQqTU1H/profile.json)
- [Blockstack 身份层对应比特币网络交易细节（不推荐深入研究）](https://docs.blockstack.org/core/wire-format.html)
- [UserSession 用法API](http://blockstack.github.io/blockstack.js/classes/usersession.html)
- [Blockstack.js API](http://blockstack.github.io/blockstack.js/index.html)
- [官方 twitter banter.pub](https://banter.pub/)

## 本节课UserSession用到的函数
- userSession.redirectToSignIn()
  - 从身份管理器登入
- userSession.signUserOut()
  - 清理登陆缓存并登出
- userSession.handlePendingSignIn()
  - 处理登陆过程中是否完成（异步）
- userSession.isUserSignedIn()
  - 判断用户是否登陆（同步）
- userSession.loadUserData()
  - 加载用户基本信息（用户名、头像、社交地址等等明文信息）
