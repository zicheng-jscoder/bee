# 微信小程序——餐饮点餐商城

微信小程序——餐饮点餐商城，是针对餐饮行业推出的一套完整的餐饮解决方案，实现了用户在线点餐下单、外卖、叫号排队、支付、配送等功能，完美的使餐饮行业更高效便捷！

大家如果在使用过程有什么问题，欢迎通过lssues与我们交流！

如果本项目对您有所帮助或者启发，请给我们 Star 吧，您的鼓励是我们最大对动力～

# 招募开发者

希望找一些志同道合的朋友一起来完善这个开源项目，持续更新下去，有兴趣的可以加入QQ群 ( 详见下面的QQ群 ) 联系管理员，期待您的加入！

# 加微信联系我

15884572638

# 推荐一个订座取号的开源项目

最近经常有人咨询说需要订座和取号的功能，api工厂有一个基于 uni-app 的开源模板，可能大家没注意，再把地址贴一下，有需要的自取：

- [仿海底捞订座排队 (uni-app)](https://github.com/gooking/dingzuopaidui)
- [码云镜像](https://gitee.com/javazj/dingzuopaidui)


# 自提/外卖 扫码体验

<img src="https://dcdn.it120.cc/2021/01/19/b388b014-7ae0-4b3a-9d6f-30c8b3082fe6.jpg" width="200px">


# 扫码点餐演示

| 座号A1 | 座号A2 | 座号A3 | 座号A4 | 座号A5 |
| :------: | :------: | :------: | :------: | :------: |
| <img src="https://dcdn.it120.cc/cuser/27/2021/09/26/cbb91217-47b1-4af1-a0e5-55df0efd3566.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/cbb30b43-15df-4564-87ef-3416f58ab0c8.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/150cd47b-e769-49fc-bca6-be8c5fe84f49.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/b5a44d1f-cea4-437f-802d-a36c728ff459.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/99c47ba3-50ba-4431-93c6-e10f527a5e28.png" width="200px"> |


| 座号A6 | 座号A7 | 座号A8 | 座号A9 | 座号A10 |
| :------: | :------: | :------: | :------: | :------: |
| <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/aca7a7fd-72c9-4d89-a903-d82e6b8b8f83.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/77f16752-656f-4218-99df-c82c5db1921a.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/e3be04c4-9c0f-41c8-9482-b645699d1df4.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/352c7e84-56ec-4961-9e7d-cc4e752cf154.png" width="200px"> | <img src="https://dcdn.it120.cc/cuser/27/2023/01/04/78adb196-231d-41b7-be8d-51febc022bac.png" width="200px"> |

## 桌号管理

    登录后台，左侧菜单 “桌号管理”，添加并管理你的桌号信息，添加以后在列表你将可以看到 ID 和 密钥，这两个数据用来生成桌子的二维码

<img src="https://dcdn.it120.cc/2022/12/30/e76a0320-992a-4932-9d58-dec3fd6630b8.png">

## 生成桌子二维码

    例如上面的ID为 308，密钥为 d3PiIY，那么现在去左侧菜单微信设置 -> 小程序设置 -> 获取小程序二维码（圆形码），即可获取小程序码：
    填写信息如下：
- 页面路径: pages/index/index
- scene参数: shopId=12879,id=308,key=d3PiIY

其中 shopId 为你对应的门店ID，其他参数默认就可以了

<img src="https://dcdn.it120.cc/2022/12/30/6c807326-8db9-465a-912e-58847b28658c.png">




# 本项目使用了下面的组件，在此鸣谢

- [vant-UI库](https://youzan.github.io/vant-weapp/)

- [小程序在线接口-SDK](https://github.com/gooking/apifm-wxapi)

- [api工厂](https://admin.it120.cc)

- [FMUI-轻松活泼-icon](https://www.iconfont.cn/collections/detail?spm=a313x.7781069.0.da5a778a4&cid=17041)

- [小程序HTML解析组件](https://github.com/jin-yufeng/Parser)

- [生成条码和二维码](https://github.com/alsey/wxbarcode)

# 使用教程
## 注册开通小程序账号
https://mp.weixin.qq.com/
根据自己的实际情况选择 “企业”、“个体工商户”身份，注册小程序账号，商城类小程序不支持个人用户上线，所以一定要选择企业或者个体户，获得你自己小程序的 appid 和 secret 信息，保存好，下面会用到：
- [如何查看小程序的AppID和AppSecret](https://jingyan.baidu.com/article/642c9d340305e3644a46f795.html)
你需要设置小程序的合法域名，否则开发工具上运行正常，手机访问的时候将看不到数据
- [设置合法服务器域名](https://www.it120.cc/help/tvpou9.html)
## 注册开通后台账号
https://admin.it120.cc/
免费注册开通新后台后登录，登录后的首页，请记下你的专属域名，后面会用到
左侧菜单 “工厂设置” --> “数据克隆” --> “将别人的数据克隆给我”
对方商户ID填写 27
点击 “立即克隆”，克隆成功后，F5 刷新一下后台
## 配置小程序APPID/SECRET
左侧菜单，微信设置，填写配置上一步获得的 appid 和 secret
这一步很重要！！！
如果没有正确配置，下面步骤中打开小程序将无法连接你的后台
## 配置微信支付
左侧菜单，系统设置 -->  在线支付配置，填写您自己的微信支付的信息
## 下载安装开发工具
https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html
## 运行小程序看效果
双击运行第一步安装的小程序开发工具，打开看效果：

<img src="https://dcdn.it120.cc/yuque/0/2019/png/572726/1575349127431-00ff2059-dd5e-4e4b-99a7-e1d605db02c7.png?x-oss-process=image%2Fresize%2Cw_1500 " width="200px">

导入项目这里，目录选择你 “第二步” 中下载并加压的小程序代码所在目录

APPID 务必要改成你自己的小程序的 APPID
APPID 务必要改成你自己的小程序的 APPID
APPID 务必要改成你自己的小程序的 APPID

然后点击导入按钮

- [如何查看小程序的AppID和AppSecret](https://jingyan.baidu.com/article/642c9d340305e3644a46f795.html)

## 配置对接你自己的后台
在开发工具中 config.js 中的subDomain 改成你自己专属域名， ctrl + s 保存

<img src="https://dcdn.it120.cc/yuque/0/2020/png/572726/1581236703094-ce5c7f32-c60d-4e1b-bacb-21439e1d2721.png?x-oss-process=image%2Fresize%2Cw_1500 " width="200px">

- [如何查看自己的subDomain](https://www.it120.cc/help/qr6l4m.html)

## 用户自提的订单如何扫码核销

用户选择自提的订单，会在底部取餐菜单界面显示订单信息以及取餐码，商家可通过 “我的” --> “扫码核销” 菜单，点击以后调起手机相机，扫用户出示的取餐码完成核销

但是默认情况下，是看不见  “我的” --> “扫码核销” 菜单的，需要在后台 “系统设置” --> “系统参数” ，添加文本类型的参数：

- 参数名 order_hx_uids
- 参数值，具有核销权限的用户的用户编号，多个用户编号，使用英文的逗号分隔

重新进入小程序以后，就可以看见 “扫码核销” 的菜单了

# 配置说明

## 如何修改小程序首页标题

登录后台，左侧菜单 “系统设置” --> “系统参数” ，添加一个文本类型的参数： mallName （注意大小写），小程序即可显示你后台填的名称

## 根据选择的不同门店，区分显示商品（只显示当前门店的商品）

登录后台，左侧菜单 “系统设置” --> “系统参数” ，添加一个开关类型的参数： shop_goods_split，开启为区分，关闭为不区分

## 如何设置服务范围（多少公里）

后台 “商场管理” --> “门店管理” ，编辑门店，服务距离处，填写你希望配送的距离即可

## 如何显示销量

商品列表接口、商品详情接口，都会返回商品的销量数据，分别是 numberOrders 和 numberSells 两个字段，你可以在界面上任何希望显示销量的地方，进行展示即可

- numberOrders 订单数量
- numberSells 商品数量

假如说用户下了一个订单一次性购买10份这个商品，那么 numberOrders = 1 ，numberSells = 10

## 如何区分门店显示商品

后台左侧菜单“系统设置” -> “系统参数”，增加一个开关类型的参数: shop_goods_split

开启则只会显示当前门店的商品，关闭则显示所有门店的商品

## 在线订座如何配置

1. 左侧菜单 “预约报名” --> “项目设置” ，添加一个项目，添加完以后会得到一个编号
2. 左侧菜单 “系统设置” --> “系统参数”， 修改编号为 `zxdz` 的参数，将你的编号填进去即可

# 常见问题

## 无法登陆 / 无法获取 openid

1. 请检查 config.js 文件中的 subDomain 是否已经修改成你自己的专属域名了
    
    [如何查看自己的subDomain](https://www.it120.cc/help/qr6l4m.html)

2. 确保下面3个地方的 appID 你填的是一样的

    - 登录你的小程序商户后台（https://mp.weixin.qq.com）左侧菜单 “开发” --> “开发设置” 中的 appid
    - 点击你的小程序开发工具 右上角 的“详情” --> “基本信息” 中的 appid
    - 登录你的 api工厂 后台（https://admin.it120.cc），左侧菜单微信设置中的 appid

## 获取手机号码失败，提示没权限

https://developers.weixin.qq.com/miniprogram/dev/framework/open-ability/getPhoneNumber.html

官方文档有说明，获取手机号码的前提条件是：非个人开发者，且完成了认证的小程序开放（不包含海外主体）
