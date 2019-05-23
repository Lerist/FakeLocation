# 常见问题（更新时间：2019年5月24日）

官方下载地址：[https://www.coolapk.com/apk/com.lerist.fakelocation](https://www.coolapk.com/apk/com.lerist.fakelocation)

## 支付问题 （更新时间：2019年4月27日）

### 1、订单码说明

订单码是在使用支付宝支付时临时生成的随机代码，该代码包含 FL(Fake Location) 账号以及您选择的专业版套餐等信息，是完成充值的重要依据，并且并非支付宝订单号；订单码仅可单次使用，完成充值后订单码会立即失效，因此请勿在下次充值时继续使用同一订单码。

### 2、点击支付宝支付方式，未能成功跳转到支付页面

请尝试升级支付宝客户端，或者采用手动转账方式，转账账号: lerist@163.com，转账时请记得备注上订单码。

### 3、支付宝支付完成，专业版长时间仍未开通

请先确认支付时，是否有在备注栏（下图1划红线处）里附带订单码

 * 若没有附带订单码，请在专业版开通页面的支付宝续期弹框里点击"忘记备注订单码"(下图2红框处)，重新提交一下。订单码会自动生成，您只需粘贴上支付宝订单号提交就行了（订单号是在支付宝账单详情里，年份开头那串数字）。记得提交前选择与支付金额一致的专业版套餐。

* 若有附带订单码，请将支付详情截图以邮件方式发给开发者处理，或者也可以直接采用前面没有附带订单码的方法，再次提交一下订单给开发者审查。
开发者邮箱：lerist.5@gmail.com

<img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/Screenshot_2019-04-27-05-54-30-945_com.eg.android.png" width="30%" height="30%" />       <img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/IMG_20190427_041839.jpg" width="30%" height="30%" />

- - - -

## 使用问题 （更新时间：2019年5月24日）

### 1、使用 Magisk root 开启模拟时一直转圈

一直转圈是在等待 Root 授权，请先不要把 Magisk 隐藏。某些手机还需保持 Magisk 在后台运行。

### 2、ROOT模式下开启模拟提示System分区不可写

可以先尝试使用 Syslock 解锁分区，若 Syslock 解不了的话，可以安装 Magisk 来解锁：先下载安装 Magisk Manager，然后取消 Magisk Manager 安装选项里的"保留 AVB 2.0/dm-verity"选项再点击Magisk 后面的"安装"，选择"直接安装"（需先授予 Magisk Manager Root权限才有此选项）。

若系统版本是 Android 9.0+ 的话，需将“ https://raw.githubusercontent.com/topjohnwu/magisk_files/master/canary_builds/release.json ”粘贴进 Magisk Manager 设置里的自定义更新通道里，然后重新打开 Magisk Manager ，这时会提示更新，点击 Magisk Manager 后面的更新按钮，更新完成后再执行前面的安装 Magisk 操作即可。

Syslock下载地址：[https://www.coolapk.com/apk/com.lerist.syslock](https://www.coolapk.com/apk/com.lerist.syslock)

Magisk Manager 下载地址：[https://www.coolapk.com/apk/com.topjohnwu.magisk](https://www.coolapk.com/apk/com.topjohnwu.magisk)

### 3、ROOT模式下开启模拟提示错误码103

103是系统分区空间不足了，使用RE管理器进到/system下删掉一些无用文件即可；小米可以删掉/system/data-app，魅族可以删掉/system/MzApp，一加可以删掉/system/reserve，其他机型可以将/system目录截图邮件发给开发者审查可删文件。开发者邮箱：lerist.5@gmail.com

### 4、ROOT模式下开启模拟提示错误码104

* 华为手机：华为近期发布的EMUI内核不支持ptrace操作，目前只有刷第三方解除了限制的内核才能使用ROOT模式，建议可以去xda论坛找找第三方内核

* 三星手机：三星官方内核和KNOX服务限制，不能关闭SELinux，目前也只有刷解除限制了的第三方ROM和内核才能使用ROOT模式

* 其他机型：请打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现错误后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（某些邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

### 5、ROOT模式下开启模拟提示“虚拟位置服务连接失败”

请不要在虚拟空间里安装运行，不要修改FL安装包；若是在更新版本后出现的这个问题，请先重启手机，再进FL的设置里清理一下运行环境即可，若是问题依旧，请打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现上述错误后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（某些邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

### 6、程序后台运行一段时间后自动关闭（摇杆退出或摇杆罗盘不随手机方向旋转）

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

### 7、关于反检测功能的使用

反检测功能需要手动设置“反检测应用”和“检测应用”
* 反检测应用：即需要隐藏的应用，或者不想被检测到的应用；如：Fake Location。点击页面内的“反检测应用”卡片进行设置。
* 检测应用：即会检测其他应用的应用；如：DD、一些游戏等。点击页面内的“+”按钮进行添加。

注：“反检测应用”和“检测应用”的关系是：“反检测应用”里勾选的应用不会被“检测应用”列表里的应用检测到，千万不要搞反了，并且两者里面不能同时包含同一应用。

### 8、手机没有ROOT权限，使用ROOT模式下的功能

手机没有ROOT权限的话，可以在虚拟大师里使用ROOT模式，虚拟大师：https://www.coolapk.com/apk/com.vmos.app  ，安装虚拟大师后，把 Fake Location 和 需要使用Fake Location功能的应用一并安装进虚拟大师，就可以使用ROOT模式下的功能了。

### 9、避免被DD检测

* ROOT模式（手机有ROOT权限）：在反检测页面中点击"+"按钮添加DD到"检测应用"，然后开启反检测即可。
* NOROOT模式（手机无ROOT权限）：可使用FL设置里的"隐藏Fake Location"功能重新安装一个随机包名的版本并卸载掉原版。

注：需确保手机上没有其它虚拟定位软件以及XP框架。

### 10、避免被游戏检测

* ROOT模式（手机有ROOT权限）：在反检测页面中点击"+"按钮将游戏添加到"检测应用"里，然后开启反检测即可；需确保手机上无其他虚拟定位软件及辅助软件。为保险起见，建议再用 存储重定向 为游戏“启用存储空间隔离”，存储重定向下载地址：https://www.coolapk.com/apk/moe.shizuku.redirectstorage
* NOROOT模式（手机无ROOT权限）：之前"隐藏Fake Location"的方式已经无效了，目前可以尝试把游戏安装进Shelter中使用，如果您的手机不支持Shelter的话，可以把FL导入进OurPlay等多开软件中使用（注意导入时需要勾选"复制安装目录"选项，并且导入完成后需要卸载原FL）；如果是小米手机的话，可以直接用系统自带的应用双开功能把游戏双开后使用。还有一点，NOROOT模式下不要打开FL设置里的"允许搜索GPS信号"选项。Shelter下载地址：https://www.coolapk.com/apk/net.typeblog.shelter  ，OurPlay下载地址：https://www.coolapk.com/apk/com.excean.gspace

注：请合理使用模拟软件，速度不要超过10，也不要长时间保持同一速度，尽量避免位置漂移。


### 未完待续...
