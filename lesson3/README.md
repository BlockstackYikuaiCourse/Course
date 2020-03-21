# Lesson 3 参考资料

- [UserSession 用法API](http://blockstack.github.io/blockstack.js/classes/usersession.html)
- [Blockstack.js API](http://blockstack.github.io/blockstack.js/index.html)
- [React 组件生命周期](https://www.runoob.com/react/react-component-life-cycle.html)

## 本节课UserSession用到的函数
- userSession.getFile()
  - 从Gaia存储器读出
- userSession.putFile()
  - 从Gaia存储器存入

## React 组件生命周期

- componentWillMount 在渲染前调用,在客户端也在服务端。
- componentDidMount : 在第一次渲染后调用，只在客户端。之后组件已经生成了对应的DOM结构，可以通过this.getDOMNode()来进行访问。 如果你想和其他JavaScript框架一起使用，可以在这个方法中调用setTimeout, setInterval或者发送AJAX请求等操作(防止异步操作阻塞UI)。

在Demo中我们通过userSession.isUserSignedIn() 来判断应该加载哪个组件，并且在componentDidMount中获取想要的信息。

在Profile组件中，由于我们已经在App组件通过 userSession.isUserSignedIn() 来确保userSession已经为登陆状态，所以通过componentWillMount在组件还没加载的时候把信息输入，并且在组件加载后直接显示出来。
