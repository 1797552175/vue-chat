# airchat

### 介绍

这是我的毕设项目，产品功能和页面参照qq，微信，TIM，不完全一样，有些是自己的想法。前后端都写。
感觉是一个挺不错的全栈入门项目，各种交互各种业务逻辑，对node（koa）和vue学习挺有帮助，现在开源出来（注意别拷贝去当毕设，仅供学习使用），接下去将继续不断完善😄欢迎star

### 技术栈：

前端vue，vue-router,vuex ，vue-cli和axios，做了移动端适配，没有用第三方组件。
后端用koa2，用gulp构建工具实现自动刷新后端代码运行。
数据库用mysql，基于Token的jwt鉴权机制，用socket.io做双向通信；

### 线上地址

[点击线上查看](http://www.hxvin.com:3000/)

建议打开手机模式

### 进度

开始 -----------------2018.01.13

- [x] 登录
- [x] 注册
- [x] 登出
- [x] 弹窗，提示等组件
- [x] 机器人智能聊天回复
- [x] 私聊
- [x] 群聊

-----------------2018.02.01

- [x] 用户资料卡
- [x] 加好友及验证好友请求
- [x] 好友请求通知
- [x] 删除好友
- [x] 未读消息提示

-----------------2018.02.10  吐槽一下，不得不佩服qq，微信的用户体验，功能细节挺多。。。。。还有，春节快到了，找我玩(茬)的bug也不少呀ಥ_ಥ

- [x] 搜索用户，群组
- [x] 创建群
- [x] 群资料卡
- [x] 加群
- [x] 退群
- [x] 修改备注

-----------------2018.02.11 一开始我只想做个简单的即时通讯而已的（认真脸），为啥抑制不住洪荒之力 orz 。暂时停更功能，先写毕设去了，毕业要紧毕业要紧🎓

- [ ] 通讯录展示
- [ ] 聊天发表情
- [ ] 聊天发图片
- [ ] 支持聊天代码美化，md语法
- [ ] 用户上传头像
- [ ] 性能优化，redis做缓存
- [ ] 发布到线上

### 使用步骤 

#### 本次开发我用了三个git分支，分别是主分支master ，开发分支dev ， 线上分支online，如果你要fork到你的本地跑，请fork master分支 。如果你想看看我是怎么打包发布上线的，请切换到online分支，查看那个名为"打包上线"的commit，你可以看到我为了打包上线做了哪些修改。

关于如何打包上线到云主机，可以看看我的这篇总结文章[airchat 打包上线小记](https://github.com/hxvin/blog/issues/28)

（注意下到本地后如果要体验soket.io通信互聊，用两个浏览器各打开一个账号，不能用同一个浏览器，因为我用localstorage缓存账户信息）

Fork 或者 下载本项目

然后进入本项目的文件夹，把airchat/server/init/sql 的 airchat.sql文件 拉到你的msyql客户端(我使用的是mac下的 `Sequel Pro` 挺好用的)

```js
npm i
```
```js
npm run dev
```
```js
cd server 
```
```js
npm i
```
接着下面两条命令执行一条就行，看着选；（如果想要修改后端代码即时保存刷新，用第一条；如果像想用chrome进行debug调试，用第二条)

```js
npm run start  
```
```js
npm run dev
```

> 老习惯，代码注释比较详细，需要注释而没有注释的我也尽快补上;
后面也会写几篇博客来详细介绍本项目，希望更好的帮助到入门的小伙伴(大神请略过，或者给些指导建议😄)

##### 如果对您有帮助，希望给个start，鼓励我继续更新^ ^

### 材料

[socket.io英文文档](https://socket.io/docs/server-api/)

[socket.io中文文档](https://zhuanlan.zhihu.com/p/29148869)

[socket.io  in github](https://github.com/socketio/socket.io/)

[socket.io-client in github](https://github.com/socketio/socket.io-client)

[聊天机器人api](http://www.tuling123.com/)

### 项目展示 （交互很多挺细，没放全，有兴趣的伙伴可以下到本地跑起来看看）

github貌似没展示完全gif图
可直接戳链接查看

[gif链接1](http://ooytyiziz.bkt.clouddn.com/airchat1.gif)

![airchat1](http://ooytyiziz.bkt.clouddn.com/airchat1.gif)

[gif链接2](http://ooytyiziz.bkt.clouddn.com/airchat2.gif)

![airchat2](http://ooytyiziz.bkt.clouddn.com/airchat2.gif)

[gif链接3](http://ooytyiziz.bkt.clouddn.com/airchat3.gif)

![airchat3](http://ooytyiziz.bkt.clouddn.com/airchat3.gif)

