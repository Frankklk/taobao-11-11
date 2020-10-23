# 2020双十一超级星秀猫自动化脚本
### 淘宝
* 支持自动做【去完成】类任务
* 支持自动做【去浏览】类任务
* 支持自动做【去搜索】类任务
* 支持自动做【领取奖励】任务

### 支付宝
* 支持自动做【逛一逛】类任务


## 创作说明
看了很多网上传的双十一脚本的源码，大多都**采用find控件再click这种触发事件**的方式

感觉还是有些问题的，因为**整个脚本并没有直接去点击屏幕**（在开发者模式是抓不到点击状态的）

而且。。。这些脚本所有动作的时间间隔都是**固定不变**的，整个脚本流程会**生硬许多**，**很容易被检测到**。

作为一个**PHPer**，也懂点auto.js，所以就自己写了个双十一的脚本。。。

这个脚本**完全模拟人工点击操作**，没有采用直接触发控件事件的方式。

而是找到控件的坐标范围，再在这个范围生成随机数**随机模拟点击**。

滑屏操作也并非机器式直线滑屏，**通过算法模拟真人滑屏（会有曲率），并有线性的速度（滑动过程先快后慢）**，感兴趣的可以在开发者工具看一下滑屏曲线

另外呢，**所有操作的时间间隔也加入了随机数**，不会固定一个间隔，所以应该能比较好地避开风控检测

目前来说，**多账号多手机亲测可用，可获全额奖励**

## 更新日志
### V 1.3.0   ——2020.10.23 18:11
新增支付宝自动化任务功能

### V 1.2.0   ——2020.10.23 11:24
修复进入打开淘宝特价版任务会卡住的问题

### V 1.1.1   ——2020.10.22 12:29
优化打开活动页方式，运行脚本可自动打开活动页

### V 1.1.0   ——2020.10.22 11:02
新增仿真滑屏动作，避开脚本检测

## 重要说明
* 高版本淘宝有**制裁规则**，会监控auto.js等脚本app进程，**奖励会变得特别低**
* 亲测淘宝V9.5.7版不会监控进程，可以获得全额奖励，推荐使用此版本
* [淘宝9.5.7下载](https://www.wandoujia.com/apps/32267/history_v278)

## 脚本说明
* 此脚本可自动做淘宝双十一的超级星秀猫任务，完全解放双手
* 市面上其他脚本都是直接触发控件，并没有真正去点击屏幕，容易被判定作弊
* 此脚本完全模拟人工点击（包括滑屏操作），所有操作均加入随机数，在脚本算法层面有效提升过风控几率

## 使用说明
* **安卓设备**（无需root）安装Auto.js，APP下导入js脚本
* 开启无障碍服务并授权给Auto.js
* Auto.js APP下导入js脚本，运行即可
* [auto.js-4.1.0下载](https://share.weiyun.com/5a9g8ys)
* 仍不了解怎么使用的，建议度娘一下
