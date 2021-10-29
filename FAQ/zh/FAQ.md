# 常见问题（更新时间：2020年06月09日）

APK下载地址：[https://github.com/Lerist/fakelocation.github.io/releases](https://github.com/Lerist/fakelocation.github.io/releases/)     |    [http://lerist.net/fakelocation](http://lerist.net/fakelocation)

## 支付问题

### 1、订单码说明

订单码是在使用支付宝支付时临时生成的随机代码，该代码包含 FL(Fake Location) 账号以及您选择的专业版套餐等信息，是完成充值的重要依据，并且并非支付宝订单号；订单码仅可单次使用，完成充值后订单码会立即失效，因此请勿在下次充值时继续使用同一订单码。

### 2、点击支付宝支付方式，未能成功跳转到支付页面

请尝试升级支付宝客户端，或者在支付弹窗中点击"扫码"按钮，用支付宝扫码支付。

### 3、支付宝支付完成，专业版长时间仍未开通

请先确认支付时，是否有在备注栏里附带订单码。（目前已经采用自动附带订单码方式）

 * 若没有附带订单码，请在专业版开通页面的支付宝续期弹框里点击"提交订单"，重新提交一下。订单码会自动生成，您只需粘贴上支付宝订单号提交就行了（订单号是在支付宝账单详情里，年份开头那串数字）。记得提交前选择与支付金额一致的专业版套餐。

* 若有附带订单码，请将支付详情截图以邮件方式发给开发者处理，或者也可以直接采用前面没有附带订单码的方法，再次提交一下订单给开发者审查。
  开发者邮箱：lerist.5@gmail.com

- - - -

## 使用问题 

### 1、开启模拟时一直转圈

* 使用的 Magisk Root：一直转圈是在等待 Root 授权，请不要在 Magisk Hide 里勾选 Fake Location，或者暂时在Magisk设置中关闭“Magisk Hide”选项；有些手机还需保持 Magisk 在后台运行。

* 使用的魅族 FlymeOS 自带的Root：部分机型 FlymeOS 自带的 Root 可能出现更新系统后失效的情况，需要关闭并重新启用 Root 才能恢复。

### 2、ROOT模式下开启模拟提示System分区不可写

可以先尝试使用 Syslock 解锁分区，若 Syslock 解不了的话，可以安装 Magisk 来解锁：先下载安装 Magisk Manager，然后取消 Magisk Manager 安装选项里的"保留 AVB 2.0/dm-verity"选项再点击Magisk 后面的"安装"，选择"直接安装"（需先授予 Magisk Manager Root权限才有此选项）。

若系统版本是 Android 9.0+ 的话，需将“ https://raw.githubusercontent.com/topjohnwu/magisk_files/master/canary_builds/release.json ”粘贴进 Magisk Manager 设置里的自定义更新通道里，然后重新打开 Magisk Manager ，这时会提示更新，点击 Magisk Manager 后面的更新按钮，更新完成后再执行前面的安装 Magisk 操作即可。

Syslock下载地址：[https://www.coolapk.com/apk/com.lerist.syslock](https://www.coolapk.com/apk/com.lerist.syslock)

Magisk Manager 下载地址：[https://www.coolapk.com/apk/com.topjohnwu.magisk](https://www.coolapk.com/apk/com.topjohnwu.magisk)

### 3、ROOT模式下开启模拟提示错误码103

103是系统分区空间不足了，使用RE管理器进到/system下删掉一些无用文件即可；小米可以删掉/system/data-app，魅族可以删掉/system/MzApp，一加可以删掉/system/reserve，其他机型可以将/system目录截图邮件发给开发者审查可删文件。开发者邮箱：lerist.5@gmail.com

### 4、ROOT模式下开启模拟提示错误码104

* 华为手机：华为近期发布的EMUI内核不支持ptrace操作，目前只有刷第三方解除了限制的内核才能使用ROOT模式，建议可以去xda论坛找找第三方内核

* 三星手机：三星部分机型的内核和KNOX服务限制，不能关闭SELinux，目前也只有刷解除限制了的第三方ROM和内核才能使用ROOT模式

* 其他机型：请打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现错误后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（若邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

### 5、ROOT模式下开启模拟提示“虚拟位置服务连接失败”

请先确保使用的是正版且最新版本的程序（最新版本下载地址见本页面顶部），然后不要在虚拟空间（例如一些多开软件）里安装运行，不要修改FL安装包，不要使用破解版本；若是在更新版本后出现的这个问题，请先重启手机，再进FL的设置里清理一下运行环境即可；若是问题依旧，可以查看设备的SELinux是否支持关闭(SELinux状态可用镧工具箱APP查看)，若不支持关闭，则需刷第三方支持关闭SELinux的内核才能解决，若支持关闭，请打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现错误提示后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（若邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

### 6、NOROOT模式下开启位置模拟后，部分APP依然显示真实位置

有些APP需要在ROOT模式下才有效，NOROOT模式测试无效就只能使用ROOT模式；手机没有ROOT的话可以参考下面第 10 条。

### 7、ROOT模式下开启位置模拟后，被模拟软件提示 定位失败、获取位置信息失败 之类的提示

可能被模拟软件使用的是基站定位，请尝试在位置模拟页面点击"基站"开启基站模拟。

### 8、程序后台运行一段时间后自动关闭、跳回真实位置、摇杆退出或摇杆罗盘不随手机方向旋转

这种情况通常是程序被系统或其它某些应用清理掉了，请尝试允许FL后台运行，以及关闭省电优化之类的设置：

* 华为手机允许程序后台运行：
  [https://zhidao.baidu.com/question/521051452342852205.html](https://zhidao.baidu.com/question/521051452342852205.html)

* 华为手机忽略电池优化：
  [https://zhidao.baidu.com/question/652261302590163205.html](https://zhidao.baidu.com/question/652261302590163205.html)

* Oppo 手机允许程序后台运行：
  [https://zhidao.baidu.com/question/1545944666186333827.html](https://zhidao.baidu.com/question/1545944666186333827.html)

* Vivo 手机允许程序后台运行：
  [https://jingyan.baidu.com/article/046a7b3e9462f2f9c27fa9e9.html](https://jingyan.baidu.com/article/046a7b3e9462f2f9c27fa9e9.html)

* 小米手机：进入应用详情页，打开“自启动”开关，并把“省电策略”设为无限制，如下图所示

<img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/Screenshot_2019-04-27-08-17-37-981_com.miui.secur.png" width="30%" height="30%" />

* 其他手机请自行百度允许程序后台运行的方法

### 9、关于APP隐藏功能的使用

APP隐藏功能需要手动设置“隐藏应用”和“检测应用”

* 隐藏应用：即需要隐藏的应用，或者不想被发现检测的应用；如：Fake Location、Xposed等。点击页面内的“隐藏应用”卡片进行设置。
* 检测应用：即会检测其他应用的应用。点击页面内的“+”按钮进行添加。

注：“隐藏应用”和“检测应用”的关系是：“隐藏应用”里勾选的应用不会被“检测应用”列表里的应用检测到，不要搞反了，并且两者里面不能同时包含同一应用。

### 10、手机没有ROOT权限，使用ROOT模式下的功能（不保证所有机型都适用）

手机没有ROOT权限的话，可以尝试在虚拟大师里使用ROOT模式，虚拟大师：https://www.coolapk.com/apk/com.vmos.app  ，安装虚拟大师后，把 Fake Location 和需要使用Fake Location功能的应用一并安装进虚拟大师，就可以使用ROOT模式下的功能了。(提示：有些APP可能不支持在虚拟大师里运行，还请自行测试)。

### 未完待续...
