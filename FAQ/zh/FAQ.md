# 常见问题
## 支付问题 （更新时间：2019年4月27日）
* 1. 订单码说明
>订单码是在使用支付宝支付时临时生成的随机代码，该代码包含 FL(Fake Location) 账号以及您选择的专业版套餐等信息，是完成充值的重要依据；订单码仅可单次使用，完成充值后订单码会立即失效，因此请勿在下次充值时继续使用同一订单码。

* 2. 点击支付宝支付方式，未能成功跳转到支付页面
>请尝试升级支付宝客户端，或者采用手动转账方式，转账账号: lerist@163.com，转账时请记得备注上订单码。

3. 支付宝支付完成，专业版长时间仍未开通
>请先确认支付时，是否有在备注栏（下图1划红线处）里附带订单码
> * 若没有附带订单码，请在专业版开通页面的支付宝续期弹框里点击"忘记备注订单码"(下图2红框处)，重新提交一下订单码。订单码会自动生成，您只需粘贴支付宝订单号提交就行了（订单号在支付宝账单详情里，年份开头那串数字）。记得提交与支付金额一致的订单码
>* 若有附带订单码，请将支付详情截图邮件发送给开发者处理，或者也可以直接采用前面没有附带订单码的方法，再次提交订单给开发者审查。
开发者邮箱：lerist.5@gmail.com
><img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/Screenshot_2019-04-27-05-54-30-945_com.eg.android.png" width="30%" height="30%" />       <img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/IMG_20190427_041839.jpg" width="30%" height="30%" />

## 使用问题 （更新时间：2019年4月27日）
* 1. ROOT模式下开启模拟提示错误码103
>103是系统分区空间不足了，使用RE管理器进到/system下删掉一些无用文件即可；小米可以删掉/system/data-app，魅族可以删掉/system/MzApp

* 2. ROOT模式下开启模拟提示错误码104
>*华为手机：华为近期发布的EMUI内核不支持ptrace操作，目前只有刷第三方解除了限制的内核才能使用ROOT模式，建议可以去xda论坛找找第三方内核
> 
>*三星手机：三星官方内核和KNOX服务限制，不能关闭SELinux，目前也只有刷解除限制了的第三方ROM和内核才能使用ROOT模式
> 
>*其他机型：请打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现错误后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（某些邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

* 3. ROOT模式下开启模拟提示连接虚拟位置服务失败
>请不要在虚拟空间里安装运行，不要修改FL安装包。若是其它情况，打开FL设置里的"日志记录"功能，重启一下手机，再开启模拟，出现上述错误后，点击侧边栏里的"反馈"，选择邮件方式把日志文件发给开发者分析具体原因（某些邮箱客户端附带不了日志文件，建议使用网易邮箱客户端发送）

* 4. 程序后台运行一段时间后自动关闭（摇杆退出）
>这种情况通常是程序被系统或其它某些应用清理掉了，请尝试允许FL后台运行，以及关闭省电优化之类的设置：
>*华为手机允许程序后台运行：
[https://zhidao.baidu.com/question/521051452342852205.html](https://zhidao.baidu.com/question/521051452342852205.html)
> 
>*华为手机忽略电池优化：
[https://zhidao.baidu.com/question/652261302590163205.html](https://zhidao.baidu.com/question/652261302590163205.html)
> 
>*Oppo 手机允许程序后台运行：
[https://zhidao.baidu.com/question/1545944666186333827.html](https://zhidao.baidu.com/question/1545944666186333827.html)
> 
>*Vivo 手机允许程序后台运行：
[https://jingyan.baidu.com/article/046a7b3e9462f2f9c27fa9e9.html](https://jingyan.baidu.com/article/046a7b3e9462f2f9c27fa9e9.html)
> 
>*小米手机：进入应用详情页，打开“自启动”开关，并把“省电策略”设为无限制，如下图所示
> 
><img src="https://raw.githubusercontent.com/Lerist/fakelocation.github.io/master/FAQ/zh/img/Screenshot_2019-04-27-08-17-37-981_com.miui.secur.png" width="30%" height="30%" />

* 5. 避免被DD检测
>
请使用FL设置里的"隐藏Fake Location"功能重新安装一个随机包名的版本并卸载掉原版，并且确保手机上没有其它虚拟定位软件以及XP框架

* 6. 避免被某游戏检测
>
建议使用设置里的"隐藏Fake Location"功能重新安装一个随机包名的版本并卸载掉原版，并且请合理使用模拟软件，速度不要超过5，也不要长时间保持同一速度，尽量避免位置漂移。还有一点，NOROOT模式下不要打开FL设置里的"允许搜索GPS信号"选项

* 未完待续...
