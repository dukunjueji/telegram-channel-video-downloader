# 更新记录 
* pg.20240610-1437.zip 优化csp_Youtube播放页，因为它主要目的是让人沉迷的长视频平台，因此默认只播放一个视频是不太合理的，所以现在会把播放列表或相关推荐放到主播放线路中，这样就可以连续欣赏了呢。
* pg.20240609-1718.zip csp_Youtube優化搜索輸入界面佈局，防止在電視上被輸入法遮擋。優化所有遠程輸入佈局。同時修復csp_Youtube中如果點擊了頻道内容后無法再切換分類的問題
* pg.20240609-1614.zip csp_Youtube增加jar内搜索，ext中支持配置搜索關鍵詞，會出現在搜索框内，這個搜索儘搜索csp_Youtube内部。還支持遠程輸入，可以用手機向電視遠程輸入搜索關鍵詞。有了這個功能，就可以隨時臨時搜索感興趣的關鍵詞了呢。需要注意的是輸入超時為60秒（或更短）如果搜索無結果，可以返回一步再次點擊。修復搜索崩潰問題
* pg.20240609-1200.zip csp_Youtube增加视频时长显示。
* pg.20240609-1007.zip csp_Youtube优化频道列表，不再加载频道全部视频，改为 以频道名称搜索视频
* pg.20240609-0743.zip csp_Youtube修复翻页问题，优化lib/youtube.json
* pg.20240609-0626.zip csp_Youtube修复分类导致的播放列表和频道视频无法播放问题。修改json的分类加载机制，filters中的名称会完全替换分类搜索关键词（之前是两者相加），具体例子参考lib/youtube.json
* pg.20240609-0047.zip csp_Youtube支持使用json方式配置分类页，例子在lib/youtube.json，大分类下使用筛选获得细分分类。json配置时type自动失效
* pg.20240608-2253.zip csp_Youtube字幕偏左问题修复，是原版字幕就特意设定了位置，已经使用独家修复技术修复到中间了，同时优化了字幕语言选择问题，根据系统语言自动默认选择相应语言字幕。优化嗅探。
* pg.20240608-2020.zip csp_Youtube支持AI字幕，字幕支持影片内置的听障字幕，也支持上传者上传的额外外挂字幕，如果字幕没有中文和英文，会使用AI自动翻译中文和英文字幕加上。
* pg.20240608-0914.zip 優化csp_Youtube相關推薦和頻道内容的排序。可以用youtube愉快追劇了呢！無廣告又高清還免費而且不用設置token/cookie之類的麻煩事，這是伊甸園嗎？
* pg.20240608-0829.zip 徹底修復csp_Youtube分類和搜索經常爲空的問題（原開源項目的bug），修復磁力狗，優化所有嗅探，修復smb。
* pg.20240607-2049.zip csp_Youtube支持指定編碼，"ext":{"codecs":"av|vp"}表示支持av開頭的和vp開頭的編碼，如果播放器不支持vp系列編碼，則只保留av即可，此字段爲空時表示支持所有編碼。在處理相關推薦時做了些優化，如果有播放列表或頻道視頻列表，則只加載20個相關推薦。讓我們為youtube窒息
* pg.20240607-2002.zip csp_Youtube支持頻道視頻列表和播放列表，搜索時自動識別。嘗試支持youtube字幕，但似乎不成功。
* pg.20240607-1257.zip /proxy?do=yt改为老的方式播放，只有加载失败时才尝试新的csp_Youtube方式播放。csp_Youtube相关性推荐从20个增加到60个。
* pg.20240607-0954.zip 修复yt直播。tokenm.json中增加"youtube_proxy"配置项，在push中推送任意youtube地址也可以用上指定代理了呢。因为push完全接管了youtube链接，所以之前说android9以下用csp不能播youtube的可能现在用推送也不能播了。。。。修复了一个长期以来的初始化问题，在低端设备上jar初始化被中断而导致加速SO异常的情况会大幅减少
* pg.20240606-2324.zip 優化團長（csp_TZFile），中國高清網(csp_Gaoqing），愛看機器人(csp_Ikanbot)，使用最新的過盾技術，提高頁面載入成功率
* pg.20240606-2102.zip 徹底修復Youtube部分直播無法欣賞問題。徹底修復某族無法播放問題。
* pg.20240606-1719.zip 优化某族，过盾成功率更高。
增加Youtube(csp_Youtube)，支持指定代理，可以搜索，兼容普通视频和直播源。
* pg.20240606-1108.zip 修复某族忘了改的几个过盾bug，提高人机成功率。修复某堂搜索结果无法播放问题。重申一下miss必须不使用指定代理才能过盾（无代理或全局代理都可以）。修复哔滴播放失败问题（修改首页地址即可）
* pg.20240605-2143.zip 修复miss
* pg.20240605-2112.zip 提高某族列表加载成功率，滑动验证窗口1分钟内最多显示一次。
* pg.20240605-2000.zip 大幅提高嗅探效率，大幅提高嗅探过盾能力，某堂某族的土盾洋盾都已经被降伏，某族挂全局代理也可以过盾了，但某族首个分类内容较多，可能要多刷几次才能看到列表。
* pg.20240605-1621.zip 优化网盘及弹幕设置中的输入框，增加迅雷/PikPak的转存画质选项。
* pg.20240605-1501.zip 继续修复某族某堂
* pg.20240605-1252.zip 优化某族某堂，某堂指定代理无法过盾，所以需要不指定代理或使用全局代理。某族改域名到最新域名即可http://777631.xyz/
* pg.20240605-0934.zip 修复PikPak转存原画播放失败问题，该问题是前几天PikPak反制清明下载器家族引起的，属于误伤。
* pg.20240604-2009.zip 修复某堂，不能指定代理
* pg.20240604-1044.zip 再次修复持续作妖的团长资源(csp_TZFile)
* pg.20240602-1730.zip 修复团长资源(csp_TZFile)
* pg.20240602-1004.zip 增强代理安全性，防止隐私泄露
* pg.20240530-1542.zip 优化WebView嗅探资源占用。顺便修复某族某堂
* pg.20240529-1555.zip 恢复阿里云转存线程数自定义功能，最高为10，但小于16G视频会强制使用单线程。转存线程在“网盘及弹幕配置”中设置。
* pg.20240529-0734.zip 继续修复迅雷和PikPak登录时忽略了tokenm中设定的captchatoken的问题。
* pg.20240528-2228.zip 修復迅雷/PikPak使用網盤配置登錄時忽略tokenm.json配置問題。彈幕加載失敗不再提示。
* pg.20240528-1240.zip 屏蔽高速加速及其配置项。磁力解析使用普通加速so。
* pg.20240527-1436.zip 优化磁力高速加速速度探测算法，更加精准有效，减少本来有高速加速却回落到普通加速的现象。
* pg.20240527-1108.zip 优化磁力高速加速速度探测手段
* pg.20240526-2314.zip 修復Bdys搜索結果很多不可播放的問題。阿里/夸克/迅雷/PikPak的配置界面裏，都增加了遠程輸入提示和小二維碼，此二維碼只是遠程輸入用，并不是掃碼登錄的二維碼。遠程輸入可用於輸入Cookie或CaptchaToken等超長的内容，從PC或手機直接遠程輸入到播放器。
* pg.20240526-2038.zip 修復Bdys在綫播，Bdys改爲只有搜索才使用指定代理，其他情況不使用指定代理。優化高速加速用戶創建流程，如果遇到提示高速加速注冊或登錄失敗，可以到網盤及彈幕設置中的磁力設置選擇重新創建高速用戶。
* pg.20240526-1826.zip 修复哔滴影视搜索(csp_Bdys01)，因为使用了谷歌搜索，因此需要指定代理使用搜索功能。而且为了保证磁力播放顺畅已降该csp加入push全家桶，因此还要让ext第一项是./lib/tokenm.json
* pg.20240526-0917.zip 继续优化迅雷/PikPak登录流程，试图提高登录成功率。优化磁力播放流程，减少不必要的初始化
* pg.20240524-1845.zip 尝试优化PikPak登录流程，减少对captchatoken的依赖。
* pg.20240524-1552.zip 优化嗅探逻辑，如果不指定代理，则完全使用原有流程。另外某灵已经去掉所有盾。
* pg.20240524-1109.zip 使用了全新的嗅探黑科技，可以使用指定代理对付cf盾了，所以某灵可以直接用指定代理来实现快速而优雅的列表与搜索了呢，就等某灵加上谷歌图片识别了。同时优化了所有用到嗅探的csp。
* pg.20240523-2055.zip 提高某灵加载成功率
* pg.20240523-2034.zip 優化嗅探資源占用，降低内存消耗。修復某霛，因某霛把土盾換成了洋盾，因此不能使用指定代理，以及可能需要全局挂梯才能正常加載頁面。
* pg.20240523-1349.zip 修复不太灵
* pg.20240523-1000.zip 修复爱看机器人
* pg.20240523-0831.zip 修复不太灵列表和搜索。修复PP离线有时失败的问题。
* pg.20240522-2035.zip 迅雷/PikPak恢復轉存功能（之前是屏蔽了，因爲不轉存也能看），使用轉存播放可以看超過20分鐘的分享内容了。同時增加了“PP極速轉存播放”功能，可以先轉存再極速，實現最高播放速度。
* pg.20240522-1755.zip 修復PikPak登錄及分享問題，同時修復PP離綫。
* pg.20240522-1506.zip 修复不太灵搜索，不太灵改为全部嗅探方式，以防网站再次升级风控。修复PikPak分享无法观看问题，但自测使用PikPakGO直连方式播放比较吃力，用PP极速播放无问题。
* pg.20240521-1059.zip 指定代理支持直播类地址的指定代理（之前只能播10秒，然后等1分钟才能下一个10秒）
* pg.20240520-1503.zip 尝试解决磁力解析线程被杀问题
* pg.20240520-0944.zip 在“网盘及弹幕配置”中增加“是否使用内置存储来保存配置数据”功能，当开启时，使用应用内的数据目录保存token/cookie信息，不使用SD卡的TV目录。优化网盘初始化流程，防止错误配置的网盘csp影响tokenm.json加载。
* pg.20240519-1633.zip 修复某族某堂。磁力高速加速增加网速判断机制，前10秒速度低于500kB/s则切下一个加速方式，防止出现高速加速获取到token但速度太慢无法播的问题。
* pg.20240519-1107.zip 恢復高速加速，但目前高速加速不同種子的表現差異巨大，可能飛上天也可能趴在地，因此是否啓用高速加速取決於有緣人想看的資源是否高速有速度，請自行決定是否開啓高速加速。
* pg.20240517-1224.zip 磁力播放增加“是否打開匀速控制”功能，可以選擇關閉匀速控制，此時將全速下載磁力内容。
* pg.20240517-0724.zip 优化磁力内存占用，避免内存溢出。
* pg.20240516-2007.zip AI去广告兼容短剧。修复前两版被误删除的匀速控制功能。
* pg.20240516-1857.zip 优化X5探测方式。
* pg.20240516-1627.zip 優化磁力播放，減少間斷問題（普通加速時p2sp不給力依然可能卡頓）。增加“是否使用JAR播放磁力”的設置項，可以不刪除SO而直接使用殼上播放能力。修復磁力起播時檢測剩餘空間的一個小bug。修改X5偵測方法，修復殼上X5有框架但沒有實際代碼時導致的嗅探錯誤。今天（2024.05.16）高速加速上游盤點，請到設置中關閉高速加速，明日再打開
* pg.20240515-2059.zip 修复磁力开播剩余空间检查的bug。修复阿里 夸克 迅雷PP配置界面远程输入的bug 修复弹幕行数配置界面bug
* pg.20240515-2010.zip 磁力播放增加自动重建功能，在网盘及弹幕设置中，可以指定一个磁力缓存重建大小，当磁力缓存内容超过重建大小后，会删掉缓存自动重建，可以应对fat32的4G限制，该功能会在视频播放5分钟后开启，防止影响起播速度。该功能也可以用于避免存储被写满，例如存储剩余空间是8G，那么指定重建大小为7G，这样就会在磁力缓存使用了7G空间时自动删掉重建，防止占满整个存储卡死。
* pg.20240515-0007.zip 磁力播放時，去掉對剩餘空間的檢測，似乎對盒子或外置U盤的壓力有所降低。優化單磁力鏈時的解析速度。
* pg.20240514-2203.zip 优化磁力，高速/离线加速时，使用更短的超时时间以便加速失败能较快跳过。
* pg.20240514-1452.zip 音范丝优化磁力组织方式，防止TV上选择线路时导致连续无效加速。
* pg.20240514-1225.zip 增加音範絲。大量網盤的csp改爲并發加載，比如hdhive等等，不一一列舉，所有網盤csp都已改爲多源并發加載
* pg.20240514-1006.zip 优化磁力播放，当未登录PP时，直接跳过离线加速尝试。提高磁力解析速度。减少磁力自动清理对磁盘/闪存的压力。
* pg.20240513-2114.zip 大幅优化磁力播放，解决不太灵，美剧迷等单个视频源内大量磁力链导致播放困难的问题。优化阿里播放。
* pg.20240513-1704.zip 磁力分集改回整体排序（为了对付不太灵混乱的网页内容）
* pg.20240513-1035.zip 高速加速增加5秒超时控制，防止高速加速解析源问题导致播放卡住
* pg.20240512-1513.zip 阿里云盘的token输入界面，夸克的cookie，迅雷PP的captchatoken输入界面都支持http://ip:9978/proxy?do=input的方式输入内容了。csp_AppYsV2支持自动去广告（未测试）
* pg.20240512-1029.zip 磁力播放支持關閉普通加速，在網盤及彈幕配置中，磁力設置中，可以選擇關閉普通加速功能，但請注意，如果關閉了普通加速，卻沒有打開高速/離綫加速，那麽磁力將直接播放失敗。
* pg.20240512-1001.zip 磁力修复高速加速/离线加速/PP极速的同一个视频二次播放失败问题。优化磁力高速/离线/极速的起播速度
* pg.20240512-0847.zip 修复所有验证图片引用的csp的图片问题（包括爱看机器人）
* pg.20240512-0527.zip 修復PP搜索結果無法播放問題
* pg.20240511-2250.zip 磁力多個磁力鏈放到同一個源内時，排序優化，防止多集的劇集第一集擠在一起。
* pg.20240511-1807.zip 磁力無害化處理，網盤及彈幕設置中，增加“離綫播放使用PPGO”，該功能默認關閉，當打開此功能時，會使用PikPakGO直連方式播放磁力内容，完全不占用任何閃存空間，完全不用考慮限速問題和閃存損耗問題，是真正的曲率引擎。此項科技功能可以實現非人類的各種機動動作，油門刹車？不存在的，根本不需要油
* pg.20240511-1539.zip 优化磁力起播速度，优化离线内容二次播放起播速度。磁力飞行匀速控制模式下，不再彻底关闭网络，而是保留每秒1M左右的网速缓慢消耗。防止彻底断开后重连困难。
* pg.20240511-1241.zip 为提高某堂某族JXX的离线成功率，把他们都加入了Push全家桶，因此json配置项的ext第一位必须是lib/tokenm.json了哦。优化离线策略，10分钟内不会离线第二次，防止循环尝试离线。
* pg.20240511-1138.zip 优化磁力离线播放，解决离线容易失败问题。优化普通加速，普通加速不再限速，解决普通加速暂停后无法恢复问题。
* pg.20240511-0009.zip android6以下不加载任何jar内so，使用壳上磁力播放能力。
* pg.20240510-2351.zip 迅雷網盤和PIkPak網盤在網盤及彈幕設置中，可以選擇關閉極速播放功能，就可以只使用原來的直連方式播放。
* pg.20240510-2247.zip 鉴于PP盘尊贵收费用户的网盘容量10T，因此增加磁力离线是否自动清理的开关，当开关关闭时，每次离线加速任务都会保留在PP盘里，这样对于缓慢的离线任务，有缘人可以自己到“我的分享”里的PikPak盘我的分享里去直接观看。
* pg.20240510-2222.zip 磁力離綫加速從60秒超時改爲10秒超時。嘗試修復磁力二次播放失敗問題，修復磁力緩存路徑設置崩潰問題。改善磁力慢速播放時的播放成功率
* pg.20240510-1934.zip 网盘及弹幕配置中，磁力缓存路径设置自动列出系统中所有外部存储，直接选择即可。自测随便挂了个ntfs格式的U盘正常使用。
* pg.20240510-1842.zip 修复磁力自定义存储路径大写被强制转小写的bug。网盘及弹幕配置中所有输入框的地方都会列出上次配置的值。增加了http://ip:9978/proxy?do=input可以远程输入配置项，只要在网盘及弹幕配置中打开需要输入的输入框（例如磁力存储地址）然后在9978的那个界面中输入设置的值，所设置的值就会自动进入播放器上的配置界面，点确定即可。
* pg.20240510-1531.zip 磁力支持使用PP离线加速，使用该功能要求事先打开过任意带有PP的csp，比如网盘和弹幕设置。离线加速默认关闭，需要到网盘及弹幕设置中打开才能使用。该功能会用到PP盘的空间，因为PP免费用户只有6G空间，所以超过6G的磁力离线加速会失败，可买PP会员提高容量。
* pg.20240510-1313.zip 增加磁力播放高速加速功能開關，可以到網盤及彈幕配置中關閉高速加速，使用普通加速能力播放磁力。默認不打開高速加速能力。
* pg.20240510-0925.zip 磁力緩存路徑支持自定義，可以指定到外部存儲，在“網盤及彈幕”設置中設置。優化磁力匀速飛行能力，解決關閉後流量繼續跑問題。大幅提高所有網盤和磁力詳情頁加載速度。
* pg.20240509-2321.zip 修复磁力匀速飞行的一些bug
* pg.20240509-1819.zip 终于把被迅雷焊死的磁力油门给弄活动了，现在可以在播放期间也能匀速下载了，不会再疯狂消耗带宽，解决幼小的盒子无法承受迅雷摧残的问题。
* pg.20240508-1157.zip 優化SO加載邏輯，主加速SO和基礎加速SO分別控制，理論上可以減少播放器崩潰情況。因爲完全jar内實現磁力播放邏輯，所以把原來的各種低效率的反射掃描都去掉了，理論上運行會更快一些。
* pg.20240507-2110.zip 修改SO加載提示，只有加載成功才提示，加載失敗則自動回退到殼上播放能力，因此可以刪掉jar内所有so來實現回退到殼上磁力播放。在磁力或迅雷/PP播放期間如果用到了jar内加速，會有短暫的“加速中。。。”提示，以便確認是否用了jar内加速。增加了播放中即時檢查磁盤剩餘空間的功能，磁盤剩餘空間小於128M自動清空緩存，如果播放開始時磁盤空間已經小於128M則直接播放失敗。
* pg.20240507-1455.zip 不太灵和美剧迷检查是否启用了jar内加速，不加速则使用壳上解析。
* pg.20240507-1050.zip 修复SO远程加载bug
* pg.20240507-0034.zip 优化磁力播放，在能加速的情况下尽量加速，如果加速失败再使用标准方式播放。我愿称之为：饱和式播放
* pg.20240506-2159.zip 修复磁力播放，但磁力加速功能没有了，可能只能热门种子才有速度。为了同时支持PP极速和磁力播放，本次更新增加了4个so，所以包体又变大了哦。PP极速线路放到了迅雷网盘和PikPak网盘线路的第一位。
* pg.20240506-1518.zip 修复：加速SO加载失败时，其他网盘可能播放失败的bug
* pg.20240506-0901.zip 优化美剧迷(csp_Meijumi)播放线路，使用子目录方式把在线播、网盘、磁力分开，防止线路过多解析超时。优化PP极速播放效果
* pg.20240506-0813.zip libxl使用tokenm.json中的"libxl_url"单独配置
* pg.20240505-2304.zip 弹幕及网盘配置中增加了清除磁力加速SO的功能，便于主动清理SO旧文件，不用把整个播放器的数据清空了。
* pg.20240505-2133.zip 磁力已完全恢复（64/32 手机电视都支持），重置app（或清空app数据）后加载新jar实现加速SO更新。
* pg.20240505-1914.zip 修复64位版本的磁力播放，需要重置app（清空数据）才会使用新的SO加速。32位暂不支持，谁有各路下载器app的32位版本可以倾情提供一下。
* pg.20240505-1008.zip 修復所有迅雷/PP視頻源 的 PP極速播放功能
* pg.20240505-0858.zip so文件放入jar内部了，不用管lib的事兒了。
* pg.20240505-0841.zip 修復迅雷和PP推送時的PP極速播放不可用問題。
* pg.20240505-0010.zip PP极速播放在播放PP盘资源时，使用新的播放方式，理论上提速更快。
* pg.20240504-2351.zip 优化加速SO的加载逻辑，即使不配置tokenm.json也可以加载了。优化不太灵，改为子目录方式，每个磁力链接分别解析
* pg.20240504-2146.zip 不太灵的磁力链解析改回壳解析
* pg.20240504-1927.zip 優化加速邏輯，不再嘗試加載播放器中的so，減少崩潰幾率
* pg.20240504-1647.zip 优化迅雷网盘的“PP极速播放”线路
* pg.20240504-1559.zip 当我们迈出探索宇宙的第一步，就意味着我们的目标绝不是绕地飞行，而是征服星辰大海。迅雷云盘/PikPak已加入征服宇宙的舰队，在迅雷云盘及PP分享中，增加了“PP极速播放”线路，该线路不依赖tokenm.json中的内置代理配置，完全直连，所以如果要释放PP分享的速度，可能需要全局挂梯。
* pg.20240504-1051.zip bug的一小步，就是人类的一大步。
全播放器支持。本次更新因为带有神秘物质，所以包体较大，而且需要打开“网盘及弹幕配置”来激活神秘物质，打开"网盘及弹幕配置“后不用做任何操作，到播放器设置里重新加载一次配置来彻底激活神秘物质即可。so已支持gz格式放置
* pg.20240501-2226.zip 小bug修复
* pg.20240501-1045.zip 修复Eighteen
* pg.20240501-0952.zip 尝试解决部分盒子磁力播放问题
* pg.20240501-0026.zip 优化磁力播放，使用缓存对加速做了二次加速，解决磁力切换集数时的漏删情况。优化XBPQ，增加对磁力链接的自动修正处理。需要更新lib/XBPQ.jar
* pg.20240430-1845.zip 优化磁力播放，连续多集播放时，实时自动清理磁盘。解决内存较小的盒子播放超过剩余空间的磁力时，每次写满就卡顿的问题。
* pg.20240430-1551.zip 重新打开被误关的磁力飞行开关
* pg.20240430-0853.zip 修复磁力熊和Wo4K（只改了js配置）
* pg.20240429-1752.zip XBPQ已真正加入磁力飞行全家桶。优化磁力播放，解决偶尔卡顿问题。
* pg.20240429-1154.zip 解决磁力播放停止后 后台跑流量问题，刹车技术已出神入化。
* pg.20240429-0041.zip 修复部分磁力无法播放的错误。
* pg.20240428-2156.zip 刹车片优化
* pg.20240428-1649.zip 坐稳扶好，磁力真正起飞。。。
* pg.20240428-1438.zip 优化磁力播放，本次更新具有实验性质，主要解决冷链无速度问题，因为使用了一些特殊的加速方式，所以在从磁力内容退出后，可能播放器仍在跑流量，此时只需要播放任意非磁力内容就可以解决，当然杀掉后台也行。本次更新仅兼容OK版影视播放器，其他播放器可能会报错。
* pg.20240427-2238.zip 阿里转存预览不再使用NanoHTTPD.response返回内容，防止壳崩溃。
* pg.20240427-2135.zip 修复内置去广告代理对部分url处理错误（黑狐影院）
* pg.20240426-2316.zip 修复阿里转存预览无法播放问题
* pg.20240426-1434.zip 阿里预览画质改为转存预览
* pg.20240425-2035.zip 优化pikpak播放，提高对梯子的兼容性。
* pg.20240423-1903.zip 修复姐姐
* pg.20240423-1810.zip 彻底修复BtSearch（csp_BtSearch）
* pg.20240423-1144.zip 大幅提高webview嗅探稳定性，修复btsearch
* pg.20240422-2036.zip 修复TS文件没有播放时间的问题，修复一些采集源播放异常。
* pg.20240422-1844.zip 修复量子非凡等源m3u8处理错误
* pg.20240422-1653.zip 修复XBPQ及其他源嗅探时有时无法得到播放地址的问题
* pg.20240422-1145.zip 深度魔改XBPQ，增加了指定代理支持，使用方法：在XBPQ的csp的ext配置中，增加"页面代理":"127.0.0.1:10072" 或其他代理地址，就打开了XBPQ的指定代理功能。例子参考“文才|XBPQ”
* pg.20240420-2117.zip 优化AI自动广告过滤算法，现在可以过滤纯乱码形式的m3u8广告了。
* pg.20240420-1933.zip 修复中国高清网翻页问题
* pg.20240420-1344.zip 增加中国高清网（csp_Gaoqing），修复阿里播放的小bug
* pg.20240419-2205.zip 内置的魔改版XBPQ支持对“嗅探词“这个配置项特殊处理，通过使用嗅探词指定m3u8地址，可以让AI全自动过滤掉不是m3u8结尾的url的广告。
* pg.20240419-2104.zip 升级AI自动去广告逻辑，可以过滤片头硬广以及以前无法过滤的一些m3u8了呢。
* pg.20240419-0926.zip 内置代理改回okhttp优先，修复aliproxy的一些bug。优化wgcf初始化过程的bug
* pg.20240418-1948.zip 网络请求优化，优先使用go代理加载页面，因为发现okhttp在代理情况下似乎经常卡住，导致玩偶无法加载。本次更新可能会带来一些兼容性问题。
* pg.20240418-1108.zip 修复皮皮虾播放，修复wo4k搜索
* pg.20240417-2209.zip 增加玩偶4K(csp_Wo4k)
* pg.20240416-1412.zip wgcf支持了tlsHello的分段，针对10072启用，所以10072可以尝试直接用cfvless的tls配置了，但最好使用优选ip而不是优选域名，因为优选域名解析出来的结果会比较随机，可能是完全阻断的ip，这样tlsHello分段也过不去。优化图片浏览模式，现在可以稳定看图了。
* pg.20240416-1207.zip 修复/proxy?do=push的字幕推送bug
* pg.20240416-1105.zip 提高圖片瀏覽穩定性
* pg.20240415-1822.zip 修复某堂的图片浏览功能
* pg.20240414-2049.zip 增加推送字幕和弹幕的支持（来自OK吊炸天），因为不太灵的磁力源经常有牛逼的片子不带字幕，因此增加该项支持，访问方式：先播放电影，然后用浏览器打开 http://播放器的ip:9978/proxy?do=push，
输入电影名称搜索字幕，然后点击相应字幕源，最后选择字幕源里的单条字幕完成推送。
* pg.20240414-1058.zip csp_Push支持通过url指定代理来嗅探，例子：https://memojav.com/video/DLDSS-277?localproxy=127.0.0.1:10072&m3u8=1，
其中localproxy指定本地代理，m3u8=1表示仅嗅探m3u8的视频，防止有些网站故意输出一些广告视频干扰嗅探。顺便提高了很多嗅探源的嗅探成功率。
* pg.20240414-0901.zip 去掉一起看，wgcf.json的域名策略改为AsIs
* pg.20240413-1901.zip 修复盘友圈，修复聚合搜索卡顿。
* pg.20240413-1824.zip 修复jsm.json的一些proxy占位符配置错误
* pg.20240413-1728.zip 增加爱看机器人（csp_Ikanbot），支持指定代理
* pg.20240413-1636.zip 修复aliproxy对简化proxy地址处理错误，需要更新aliproxy.gz到lib目录，然后pikpak的proxy才可以使用简化地址形式。
* pg.20240413-0145.zip 优化嗅探，因为使用新的api获取嗅探信息，因此不支持android5.0以下系统。
* pg.20240412-2319.zip 修复wgcf.json配置错误，本次修改需要打开阿里系csp激活一次新配置。
* pg.20240412-1147.zip 修复低端影视搜索
* pg.20240412-1132.zip 修复低端影视分类读取错误
* pg.20240412-1118.zip 增加低端影视(csp_Ddys)，提高嗅探m3u8成功率。
* pg.20240411-2219.zip 内部指定代理的warp增加多线程支持，理论上能提高warp的速度和稳定性。去掉了geoip，因为有些源解析出的国内ip是错的。因为修改了wgcf.json，所以本次更新需要刷一次阿里系csp的首页
* pg.20240411-1710.zip 修复X5内核时嗅探有时报错问题，优化内部代理对m3u8的兼容性。增加了geoip.dat.gz，使用内部指定代理的有缘人需要把该文件放到lib目录下，并在tokenm.json中增加"wgcf_geoip_url":"./geoip.dat.gz",否则内部指定代理会运行失败。因为增加了新的geoip.dat.gz，因此本次更新需要找一个阿里系csp打开一次，例如“网盘与弹幕配置”
* pg.20240411-0038.zip 修复夸克分享中点击播放时，列表加载不全的bug
* pg.20240410-2122.zip 修复夸克分享列表错误。
* pg.20240410-1731.zip 超大幅度修改jar内嗅探逻辑，已彻底驯服那极难使用指代代理的WebView，现在可以负责任的说，嗅探视频的指定代理99%成功。
* pg.20240410-1057.zip 指定代理支持同时指定多个，格式为：proxy1|proxy2，中间用竖线分割，使用时，在首次需要该代理的场合，会检测哪个能通，使用首个能通的那个，之后1小时不再检测。
* pg.20240410-0813.zip 大幅度提高嗅探指定代理成功率。修复夸克分享内如果过多垃圾文件导致视频无法识别问题。
* pg.20240410-0725.zip 阿里云强制单线程。增加是否支持书籍的设置，在网盘及弹幕设置中。
* pg.20240409-1808.zip 修复网络错误。
* pg.20240409-1443.zip 修复直播源和采集源的配置文件生成错误。修改http请求方式，极大程度提高网络请求稳定性。使用CF节点也可以稳定欣赏了。
* pg.20240409-0947.zip 优化BtSearch，提高搜索速度
* pg.20240409-0926.zip 修复团长资源(csp_TZFile)
* pg.20240408-2250.zip 解决一个长期的代理配置bug，现在多个不同的代理可以一起工作互不干扰了，因此PikPak也可以用内部指定代理正常使用了呢！
* pg.20240408-1747.zip 修复内部指定代理bug
* pg.20240408-1713.zip 修复内部指定代理的巨大bug，内部代理使用免费warp和免费cfworker的组合10074端口可以高速稳定的提供服务了，其中cfworker的vless无需任何优选。
* pg.20240408-1133.zip 修复几个嗅探源的指定代理简化模式支持不完善问题。因为xray.gz不经常变动，所以从包内移除，如果需要内部代理的话从以前的包把xray.gz放入lib目录即可。
* pg.20240407-2211.zip 简化代理配置，如果是socks5代理，可以直接写IP端口，省去socks5://，配置中的海外看设置了内部指定代理方式欣赏，其他采集站仿照样子改写即可。
{
                        "key": "haiwaikan",
                        "name": "海外看",
                        "type": 1,
                        "api": "http://127.0.0.1:10079/p/0/127.0.0.1:10074/https://haiwaikan.com/api.php/provide/vod?",
                        "playUrl": "json:http://127.0.0.1:10079/parse/?thread=0&proxy=127.0.0.1:10074&url=",
                        "searchable": 1,
* pg.20240407-1843.zip 增加wgf_vless_network设置，默认是ws，可以改为tcp
* pg.20240407-1824.zip 增加wgcf_vless_tls设置，如果是true，就是在传输层打开tls，否则就是关闭tls，原来的端口尾号奇偶判断不再生效。
* pg.20240407-1602.zip 鉴于cfworkervless必须裸奔才好用的这个条件，对指定代理做了重大升级，增加了10073,10074端口，分别对应WarpOverWarp和VlessOverWarp，其中10074端口的VlessOverWarp完美解决了vless裸奔问题，也不需要对vless做优选了，其稳定性无与伦比。测试看泥巴这种m3u8是毫无问题的。对于10073的WarpOverWarp因为要求两个warp不能同一个私钥，因此增加了wgcf_key2用来配置第二个warp私钥，用10073的WOW模式，可以直接获得美国ip，理论上也是可以直接看泥巴之类的，就是速度慢点儿。另外增加了wgcf_vless_protocol字段，如果写为vmess就会自动使用auto加密的vmess连接，此时端口号依然是偶数结尾是http，奇数结尾是tls，可以使用自己vps的vmess配置。vmess方式下，optname对应实际地址和端口号，如果开在80端口不可省略80，wgcf_vless_worker随便写。本次更新不再依赖阿里云csp，但首次运行依然要用阿里云的csp激活一次。之后运行就不再需要阿里云csp辅助。
* pg.20240407-0947.zip wgcf支持非tls连接，optname如果加入的端口号是奇数结尾并且小于10000，则不强制tls，否则强制tls。修复大量在线播的m3u8处理错误。优化自动广告过滤算法。
* pg.20240406-1812.zip wgcf_vless_optname支持带端口号，也就是说可以配置完全vps自建的vless节点了。
* pg.20240406-1638.zip 修复csp_Wogg自动过盾的bug，增加vless配置方式，wgcf_vless_id对应id，wgcf_vless_optname对应优选ip的域名或ip， wgcf_vless_worker对应自己申请的cf worker（需要部署vless脚本），监听端口10072。socks5://127.0.0.1:10072，可以用于识别国家ip的一些源。
* pg.20240406-1034.zip 修复csp_Wogg的过滤器加载bug。并把默认打开的本地指定代理去掉了，有缘人自己配置吧。socks5://127.0.0.1:10071
* pg.20240406-1011.zip 增加本地指定代理，通过tokenm.json配置wgcf_key,wgcf_ipport字段，分别对应用户自己申请的Warp账号的privateKey和自己优选的warp地址，csp_Wogg,csp_Wobg已默认使用这个本地指定代理127.0.0.1:10071，理论上其他需要指定代理的源也可以使用这个指定代理。因为wogg的CF盾有时会误识别来源IP，把WARP的中国IP也当成国外，因此在csp_Wogg也加了自动过盾处理。
* pg.20240405-1337.zip 修复csp_Wobg无法使用筛选的问题。
* pg.20240405-1011.zip jar内的嗅探改为自动检测壳上是否有X5内核，若有则使用X5，若没有则使用系统webview
* pg.20240402-1845.zip 修复部分在线播自动去广告导致播放控制界面消失问题，需要更新魔改版XBPQ.jar。webview改为腾讯版本，理论上速度能更快点儿，兼容低端盒子。
* pg.20240401-0904.zip 修复新视觉，优化所有嗅探的内存占用，删掉大量看着不顺眼也用不上的csp
* pg.20240331-2059.zip 优化广告过滤逻辑，兼容一起看App更多广告类型。
* pg.20240331-1447.zip 广告过滤算法升级，极大提高精准度，既不错杀一个，也不放过一个，外科手术式精准打击。增加电影先生（基于XBPQ）
* pg.20240331-1203.zip XBPQ魔改更新，嗅探方式下的.m3u8文件已加入AI全自动广告过滤豪华全家桶。
* pg.20240331-0702.zip 改用300k版本的XBPQ。增加广告过滤结果提示。
* pg.20240330-2130.zip 加入了魔改后的XBPQ.jar，会自动针对.m3u8文件过滤广告。配置方式参考jsm.json里XBPQ字样的源。
* pg.20240330-1225.zip 优化广告识别算法，增加对“一起看App”源的广告识别。
* pg.20240330-0900.zip 修复部分m3u8广告过滤不彻底问题。尝试修复弹幕加载失败问题。
* pg.20240330-0712.zip 修复全自动去广告后的m3u8时间戳异常。
* pg.20240330-0151.zip 深度优化自动过滤广告算法，大幅提高运算效率，精准命中广告，已支持暴风自动过滤。
* pg.20240329-1841.zip csp_Push支持对m3u8自动去广告。
* pg.20240329-1748.zip type:1的源只需要配置"playUrl": "json:http://127.0.0.1:10079/parse/?thread=0&proxy=&url=", 即可实现全自动去广告，暴风、索尼、快帆、量子、非凡、海外看 均已加入全自动去广告全家桶，无需任何壳上配置。
* pg.20240329-1636.zip 修复内部代理在EXO播放器下的bug（一起看等csp都正常了），修复美剧迷超时问题。
* pg.20240329-1100.zip 天天，一起看，星星，泥巴等csp也加入了自动过滤广告功能。
* pg.20240329-0930.zip 优化广告过滤效率，减少50%的计算量，大幅提高在线源兼容性。jar内所有有可能用到在线播的源都自动过滤广告了。
* pg.20240328-2010.zip 优化m3u8全自动去广告算法，盒子也能正常运算了，大幅提高广告过滤成功率，新视觉或所有指定代理情况下皆可测试。
* pg.20240328-1613.zip 修复新视觉部分在线播指定代理情况下无法播放问题。另外对新视觉的在线播视频源使用了全自动的广告去除策略，AI驱动，对非凡量子源有特效，无需任何配置即可过滤广告。提高了新视觉搜索成功率。
* pg.20240328-0748.zip 修复新视觉搜索(csp_Xinshijue)
* pg.20240327-0908.zip 修复csp_Wobg翻页问题，增加玩你老哥
* pg.20240326-1126.zip 修复csp_YunPanOne，需要指定代理。
磁力狗设置只返回大于400兆搜索结果，btsow大于300兆，btsearch大于200兆
* pg.20240326-1032.zip 增加云盘资源(csp_YunPan)，可能需要指定代理才能访问。
* pg.20240325-1659.zip 修復迅雷雲盤登錄窗口
* pg.20240325-0950.zip 大幅度优化夸克扫码登录流程，不再使用WebView，对低端电视盒子也可以正常登录，且可以随意切换账号。
* pg.20240324-2007.zip 增加影搜(csp_YingSo)
* pg.20240324-1656.zip 修复网盘排序错误
* pg.20240324-1109.zip 增加csp_BtSow，需自行添加配置。
* pg.20240324-1049.zip 磁力狗支持打开外部播放器，修复网盘排序问题。
* pg.20240324-0921.zip 增加BtSearch(csp_BtSearch）磁力搜索。
* pg.20240324-0744.zip 修复磁力狗搜索结果出现翻页连接问题
* pg.20240323-2328.zip 大幅优化美剧迷磁力分组
* pg.20240323-1442.zip 新增磁力狗(csp_Clg)，该源内容比较杂，谨慎使用
* pg.20240323-0757.zip 修复腾讯文档表格翻页问题
* pg.20240322-1923.zip 忘了更新什么。
* pg.20240320-1020.zip 再次修复我的迅雷分享和我的PikPak分享无法进入子目录问题。增加对腾讯文档的支持。具体例子参考lib/pushshare.txt
* pg.20240320-0921.zip 修复我的迅雷分享和我的pikpak分享无法显示问题
* pg.20240319-1200.zip 修复Push类csp的tokenm.json被多次加载问题。部分csp增加图片浏览模式
* pg.20240317-2141.zip 修复盘友圈(csp_Panyq)
* pg.20240316-0658.zip 修复美剧迷
* pg.20240315-1925.zip 修复小盘盘在指定代理情况下详情页加载失败问题。
* pg.20240314-1901.zip 修复部分在线播源使用指定代理时容易播放失败的问题。
* pg.20240313-2226.zip 优化csp_Libvio，大幅提高加载成功率，在线播放到第一位。优化csp_Meijumi，在线播放到第一位。优化csp_Moli，提高在线播成功率。
* pg.20240313-1742.zip csp_PushShare，支持对磁力链接分类，在索引文件的第三段。具体参考lib/pushshare.txt
* pg.20240313-1359.zip 美剧迷(csp_Meijumi)支持在线播放，修复磁力排序问题。libvio(csp_Libvio)支持在线播放。哔滴影视(csp_Bdys01)支持磁力。删除几个无效的csp。
* pg.20240312-2314.zip 修复不太灵的搜索
* pg.20240312-2242.zip 修复不太灵(csp_Bt0)内容页突然为空问题，修复所有外部打开磁力情况下影视丢失集数名称问题。
* pg.20240310-1830.zip csp_PushShare支持搜索。
* pg.20240310-1803.zip 修复csp_PushShare的push资源无法翻页问题。磁力链接支持多个地址用逗号分隔。磁力资源不写名称字段也可以工作了。
* pg.20240310-1653.zip 增加csp_PushShare，可以把所有类型的分享资源聚合在一起，具体例子参考lib/pushshare.txt。csp_Push支持磁力使用外部播放器打开，这样所有js源的磁力也能愉快外部播放了。
* pg.20240310-1508.zip 更多磁力源支持系統打開方式，包括csp_JavDB,csp_JavBus,csp_Taohuazu
* pg.20240310-1016.zip 磁力鏈接支持外部打開，方法：在“網盤及彈幕設置”中，找到”磁力設置”，打開“使用外部播放器”，就可以用外部播放器高速播放所有磁力内容。
* pg.20240309-2002.zip 提高csp_Netflav的直连播放成功率。
* pg.20240309-1929.zip 各网盘的分享源中点击apk或图书资源时，直接精确定位到该资源，不再播放整个目录。
* pg.20240309-1503.zip 增加csp_Netflav
* pg.20240308-1133.zip 修复csp_Taohuazu
* pg.20240308-0846.zip 增加小盘盘(csp_Xpanpan)
* pg.20240307-0122.zip 修复盘友圈搜索结果标题异常
* pg.20240306-1145.zip 增加盘友圈(csp_Panyq)
* pg.20240305-2321.zip 修复阿里云字幕和书籍下载使用转存方式。
* pg.20240305-2116.zip 修复csp_Moli配置了指定代理后过滤器加载失败问题。修改tokentemplate.json里的vip_thread_limit从0到32，解决转存原画失败问题。
* pg.20240304-2333.zip 画质顺序用户直接输入时，强制转小写。
修复阿里和夸克初始化过程一处错误。
* pg.20240304-1906.zip 修复csp_Iktv点播异常
* pg.20240304-1801.zip 增加一些白嫖内容，感谢牛二、月月等大佬
* pg.20240304-1502.zip 因阿里限制了分享方式下載，所以默認去掉了極速GO原畫。
* pg.20240303-2120.zip 修复csp_Moli的首页推荐和翻页问题。
* pg.20240303-1936.zip 增加csp_Moli（HDmoli），第一次实现了网盘和在线播的混合csp。
* pg.20240302-1254.zip 阿里云分享支持self命名的我的网盘，修复迅雷和PikPak的我的网盘无法播放问题。
* pg.20240301-1934.zip 再次修復csp_TTian
* pg.20240301-1328.zip 阿里、夸克、迅雷、PikPak網盤都支持“我的網盤“，shareid使用"self"即可。在”我的網盤“内，可以直接點擊apk下載安裝，用於影視内通過網盤直接更新自己或安裝其他apk。修復csp_TTian，修復csp_Eighteen，修復美劇迷。
* pg.20240229-1947.zip 夸克增加“我的”支持，分享id设为self可看自己网盘内容，同步FongMi的WebDAV修改（播放器注入参数转Header）
* pg.20240229-0914.zip 
* pg.20240228-2150.zip {"key":"Taohuazu","name":"桃花族","type":3,"api":"csp_Taohuazu","searchable":1,"quickSearch":1, "changeable":1, "filterable":0, "timeout":60, "ext":"http://thze.cc/$$$socks5://192.168.101.1:1080"},
* pg.20240228-1549.zip 
