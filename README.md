# 更新记录 
* pg.20240929-0011.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.黑科技再升级，tgsearch已可以直接内置到手机运行，无需服务器部署（需要使用本频道另外提供的tgsearch多平台包到其他运行环境获取一次sessionstring），相关配置在网盘设置-》网盘相关配置。彻底降伏了python编译成静态化后在安卓的安全性高压环境中运行的难题，没有黑科技真是寸步难行。
2.修复tgsearch缓存异步加载问题。彻底实现群组内容无感更新。jar加载后除了首次搜索略慢，之后搜索永远快如闪电。
* tgsearchpack.20240928-2355.zip tgsearch多平台独立运行文件，使用./tgsearch
-h可以看帮助，也支持环境变量赋值（防止被坏人偷窥hash），具体环境变量分别是API_ID,API_HASH,STRINGSESSION,API_PROXY。TG
api改为短连接解决TG断连问题。允许小于8位的api_id。修复stringsession问题。修复android平台无法在app中运行的问题。修复代理 设置等相关问题。修复arm64v8无法在android运行的问题。支持对结果编码，防止外网vps使用时容易触发GFW规则。增加搜索分页功能。内置了赵总贡献的api_id，省去申请api_id的步骤。赵总说他要生10个儿子。
本日更新：增加runtgsearch.sh脚本，在服务器部署时可以运行本脚本简化后台运行过程，需要修改脚本内相应字段。允许不编码返回结果。改用异步更新缓存，除首次搜索外不再卡顿，缓存改回5分钟有效。
修复缓存异步加载错误。
* pg.20240927-2303.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.黑科技再升级，tgsearch已可以直接内置到手机运行，无需服务器部署（需要使用本频道另外提供的tgsearch多平台包到其他运行环境获取一次sessionstring），相关配置在网盘设置-》网盘相关配置。彻底降伏了python编译成静态化后在安卓的安全性高压环境中运行的难题，没有黑科技真是寸步难行。
2.修复csp_Youtube分辨率过低问题。
3.修复tgsearch运行产生缓存未清理的问题。
4.允许tgsearch不配置代理运行。
5.修复csp_TGYunPan和csp_TGYunPanLoca对搜索结果处理的bug，更稳定返回结果。
6.tgsearch增加分页设置，防止结果集过大崩溃播放器，需要更新zip和tgsearch，外部运行的tgsearch需要用独立包更新。
7.tgsearch内置赵总贡献的api_id，免去申请api，仍需登录手机号获取session，赵总说他要生10个儿子。
* pg.20240926-2129.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.优化了两个TG搜索，都支持了磁力。其中TG登录后搜索为了支持异步并发使用了新的协议，和真心的服务器不再兼容。优化了两个TG搜索对应的频道和群组。其中TG本地搜索只搜索频道。TG登录后搜索只搜索群组，登录后搜索默认群组最近500条内容，可以在配置群组列表时指定搜索的条数，越多越慢。登录后搜索程序需要配置api_id,api_hash和api_session以及proxy地址，其中api_id和api_hash都可以通过tg网站自助申请。tgsearch的使用方法可以./tgsearch -h获取帮助。登录后搜索所对应的tgsearch另外发帖提供，该tgsearch包含三个平台分别是arm,x86_64,windows，除win外都是静态编译，因此可以随意拿到任何对应的cpu主机上运行，当然运行在手机里或路由器上也是可以的，不依赖任何docker环境。
3.修复csp_Youtube，改用IOS标识，最高只能支持到1080p，凑合看吧。如果之前配置过标识，需要到网盘设置-》youtube设置-》修改标识，改成第一个IOS
* pg.20240924-1859.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.播放视频时，新增TV.kodi目录中的可以外部打开的strm文件，命名规则是在原来strm文件基础上加上ip地址，把这个带ip地址的strm文件从WSA复制到windows中，就可以用kodi的windows版打开WSA内的蓝光ISO或其他普通视频文件了。
2.修复影巢(csp_Hdhive)
3.实验性增加针对android13以上的系统级主动限速设置，自测没什么效果，较新的手机可以测一下看看，目前是固定在主动限速100M的。
* pg.20240923-1806.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.优化针对115的主动限速逻辑，手机或高端盒子可以更流畅的播放115蓝光iso而不被惩罚限速了，建议设置20M限速测试（默认不限速）。
2.修复115主动限速有时会失效问题。使用了更精确的限速算法，可以精确限制速度。并确认了盒子和电视为何播放115的iso不会被惩罚限速的原因，是因为盒子和电视通常是安卓9，而安卓9的内核网络接收缓冲区默认是2M，手机的接收缓冲区通常是4M。而且盒子或电视的无线模块通常速度不快，恰好在115惩罚限速附近，而且不会因为内核缓冲过大而额外加载内容导致超过限速。手机因为无线模块比较先进，会远超115限速范围，而且手机使用较高内核版本又有较大的缓冲区，因此使用本zip做了主动限速也不能完全避免超过限制。现在只能说在技术允许的范围内尽量做了流畅播放的努力。另外似乎115对iso和其他文件有不同的限速策略，目的是让iso不能流畅播放防止过多消耗其带宽和流量成本，所以115的remux的大文件通常可以不限速随意播放。本次更新需要重新加载GO代理。
* pg.20240922-1710.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.115主动限速增加8M一档。用手机播放115iso遇到5-15秒一卡顿的可以尝试主动限速8-10M，在网盘设置-》115设置-》115手机限速中设置。
2.優化阿里秒傳115和115秒傳阿里的處理邏輯，增加提示信息。
* pg.20240921-1923.zip 【对不起，我是阿里不限速网盘资源全秒播：https://t.me/pandagroovechat 阿里,UC,夸克使用本zip包不限速，阿里原画不需要svip也不用三方权益包，播放阿里内容不需要115账号秒传也不需要115VIP会员，115的分享内容无需付费即可欣赏，115分享大包和阿里分享大包不用建索引全部秒搜，UC原画不需要会员，夸克原画非会员3G以内的视频随意看，88VIP80G以内的视频随便看。所有网盘全自动删除转存垃圾文件，不限次数。所有网盘资源3秒起播让等待归零。可能是地球上唯一一个可以流畅在线播放ISO原盘的zip（注：使用外部播放器播放原盘ISO需要在任务列表中把影视锁定不被杀掉后台才能稳定播放）。注意：不支持仅使用jar，必须zip完整解压使用。网盘原画仅支持原版的影视、OK影视、EasyBox。對本zip内的核心jar的魔改或縫合都會導致網盤原畫不可播放。多个播放器或多次外挂本zip情况下，需要只保留一个播放器或1个外挂运行，其他的要主动杀掉，否则可能出现网盘播放异常】

今日更新内容：(更多内容阅读zip内的README.txt)
1.豆瓣首页(csp_Douban)也会初始化aliproxy了。
