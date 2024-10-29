# 魔众资源导航系统

魔众资源导航系统提供一个可以快速构建在线资源导航网站的源码系统，支持私有化部署。

## 运行环境


```
操作系统
Linux/Unix 或&nbsp;&nbsp;Windows
软件环境
Laravel 5.1的运行环境
Apache/Nginx , PHP 5.5.9+ / PHP 7.0 , MySQL 5.0+
```

## 系统截图



## 版本迭代



### V2.1.0

**发布时间**：2024-10-04

- [新功能] 项目静态资源文件增加 .nvmrc 文件，方便开发者使用 nvm 管理 node 版本
- [新功能] Grid 增加 hookPreQuery 支持数据查询前的钩子处理
- [新功能] 昨日交易数据，快捷支付链接优化
- [新功能] ComplexFields 组件支持图片链接字段类型
- [新功能] 图片可视化设计增加图片占位符显示
- [新功能] 模型查询条件支持自定义过滤功能 ModelUtil::queryRemoveCondition
- [新功能] 图片上传新增支持 svg 格式文件
- [新功能] 用户登录传输用户密码加密
- [新功能] 前端加密基础库
- [新功能] ComplexFieldsList 组件支持 textarea 输入
- [系统优化] 爬虫机器人检测规则优化，支持更多机器人识别
- [系统优化] 导航网站箭头样式对齐问题修复
- [系统优化] 后台排序功能优化
- [系统优化] 自定义字段序列化为空时异常处理
- [系统优化] 链接生成参数合并过滤异常的 amp; 字段
- [系统优化] 图片上传增加处理提示，避免出现无状态情况
- [系统优化] 图片可视化设计库尺寸缩放问题优化
- [系统优化] 多语言获取方法优化，提高性能支持
- [系统优化] 后台菜单注册闭包检测
- [系统优化] 多语言语言检测获取功能优化
- [Bug修复] data-tab-open 打开页面菜单栏高亮不消失问题
- [Bug修复] 日志文件为空时，日志查看界面显示异常问题
- [Bug修复] 头像裁剪保存页面样式优化，图标不显示修复
- [Bug修复] 图片选择直接弹出相机问题
- [Bug修复] 图片、文件选择窗口初始化快速点击自定义输入时自动跳转文件库 Tab 问题



### V2.0.0

**发布时间**：2024-08-20

- [新功能] 用户文件、图片上传支持前端直传云存储（需要安装模块支持）
- [新功能] Grid 批量操作弹窗支持自定义大小 ( data-dialog-width、data-dialog-width 属性)
- [新功能] 参数占位处理工具类 ParamUtil ，支持处理参数占位符
- [新功能] Json 组件 API 数据配置显示优化
- [新功能] Grid 表格操作支持底部操作区域（方法 footOperatePrepend）
- [新功能] RandomImageProvider 逻辑升级重构，支持更丰富的随机图片生成
- [新功能] CheckBox 组件支持表单最小宽度设置，支持更多选项传入方式
- [新功能] URL安全的 Base64 编码和解码方法
- [系统优化] Grid 中批量操作快捷监听优化 data-batch-dialog-operate
- [系统优化] 多语言 i18n 渲染方式优化
- [系统优化] 用户登录事件 MemberUserLoginedEvent 参数异常问题
- [系统优化] CurlUtil 请求头格式校验，避免错误传参导致的异常
- [系统优化] Grid 快捷编辑请求失败，页面自动刷新回复原状态
- [系统优化] 后台首页 Dashboard 报表格式优化
- [系统优化] FileUtil 生成随机文件路径后缀为空时路径拼接方式优化
- [系统优化] 模型字段数据库报错文案转换优化，自动识别长度超长问题
- [Bug修复] 富文本编辑器高度自适应概率性失效问题
- [Bug修复] MultiSelect 组件数据回显异常修复
- [Bug修复] uni-app 打包脚本在 windows 环境下运行异常问题
- [Bug修复] CurlUtil 中 GET 请求方法大小写引起的异常问题
- [Bug修复] 后台用户管理开启手机邮箱时，空字段唯一索引冲突问题
- [Bug修复] 多语言 LM 方法参数不生效问题
- [Bug修复] Laravel9 中 sql_mode 的 only_full_group_by 问题
- [Bug修复] 几处 collection 不兼容问题



### V1.9.0

**发布时间**：2024-07-10

- [新功能] 后台快速选择用户 AdminMemberSelector 组件
- [新功能] 后台标准返回 redirect 支持静默跳转
- [新功能] 命令超时运行函数
- [新功能] 优化 Nav 组件，支持链式调用，支持弹窗打开
- [新功能] 后台安全提醒修改密码链接不存在问题
- [新功能] 增加命令执行函数和数组多键值排序方法
- [新功能] 文件流式下载工具类，加密方式默认使用安全 Key
- [新功能] 用户上传数据表模型表
- [新功能] Grid、Form、Detail 支持自定义 view 和 viewData
- [新功能] 后台支持自定义样式文件 modstart.admin.styles
- [新功能] Hidden 组件支持序列化类型，避免入库异常
- [新功能] 模型操作增加 insertIfNotExists 方法，支持快捷插入数据
- [新功能] ValueUtil 和 ArrayUtil.firstValidValue 方法，支持获取第一个有效值
- [新功能] Provider 和 Biz 增加 listAllEnabled 方法，支持查询所有启用数据
- [新功能] Grid 增改差页面支持标题自定义，使用 pageTitleAdd、pageTitleEdit、pageTitleShow 属性
- [新功能] WebUploader 内置 JS 组件升级
- [新功能] 可完全自定义上传功能定制的特性 UploadScript Hook
- [系统优化] code组件重复编码问题
- [系统优化] 支付中心新增退款事件 OrderRefundedEvent
- [系统优化] 网站统计报表实时查询数据库插入冲突问题
- [系统优化] 记录是否存在方法优化
- [系统优化] 在 Linux 系统下，artisan 命令运行用户检测，避免 root 运行引起的权限问题
- [系统优化] LockUtil 加锁方法优化
- [系统优化] 时间辅助函数方法优化
- [系统优化] 超长表格 loading 效果不可见问题
- [系统优化] 临时文件清理调度默认调整到后台运行
- [系统优化] Code 换行符默认替换为 \n 问题
- [系统优化] Grid 增加按钮默认使用 titleAdd 属性
- [系统优化] Grid 列表错误异常渲染优化
- [系统优化] 图片处理工具类水印处理方法增加图片类型检查
- [系统优化] 并发访问原子类性能优化
- [系统优化] JsonKeyValue 字段显示优化
- [系统优化] EChart 折线图样式优化
- [系统优化] AgentUtil 工具类新增浏览器版本判断，方便不同场景兼容
- [系统优化] Response 下载方法浏览器兼容优化
- [系统优化] 代码清理和重构优化
- [系统优化] 搜索蜘蛛检测工具类优化
- [系统优化] 统计代码条件判断后置，系统性能优化
- [系统优化] 组件 JsonIdItems 数据预览接口返回兼容 .records 格式
- [系统优化] 组件 Image、File、Video、Audio 支持一键恢复默认值
- [系统优化] Json 组件 API 模式支持处理响应内容
- [系统优化] 轮播类型添加修改是否为空判断
- [系统优化] BizTrait 增加 first 和 firstName 方法，支持查询第一条数据
- [Bug修复] 手机快速注册登录密码设置控件不是password修复
- [Bug修复] Laravel9下关联模型数据异常问题
- [Bug修复] 已登录绑定授权信息，开启自动绑定账户时，绑定账户异常问题
- [Bug修复] 后台自动跳转到第一个有权限菜单异常问题
- [Bug修复] 用户注册弹窗异常验证码发送异常问题



### V1.8.0

**发布时间**：2024-05-26

- [新功能] KeyPoolManager 支持通用多个 Key 轮询快速开发
- [新功能] 通用导航增加变量自动替换支持
- [新功能] Echarts 组件重构，支持饼图和散点图
- [新功能] 后台左侧菜单支持鼠标滚动拖拽，方便管理超长菜单
- [新功能] 后台登录背景默认使用系统自带背景
- [新功能] 为所有组件新增 data-field 属性，方便获取组件数据
- [新功能] 用户过期时间精确到时分秒，支持更精确的过期时间控制
- [新功能] 开发者工具模块新建操作优化，支持多种预定义模板代码
- [新功能] 日志界面重构，全新日志查看体验
- [新功能] 图标增加 eye-close
- [新功能] 链接选择弹窗增加默认类型过滤
- [新功能] 后台左上角标题支持自定义，修改 modstart.php 中 admin.title 配置
- [新功能] JS 库新增 MS.util.sprintf 方法
- [新功能] Code组件编辑默认调整为代码编辑器，支持多种语言设置
- [新功能] Vue文件Widget支持style，支持自定义样式
- [系统优化] modstart_config 缓存失效问题优化
- [系统优化] 后台多标签切换浏览器页面标题显示优化
- [系统优化] 内容为空样式间隙大小优化
- [系统优化] 异常上报内容显示优化
- [系统优化] 后台首页概况无权限时，尝试跳转第一个有权限的页面
- [系统优化] 注册登录文案提示优化
- [系统优化] 用户移动端微信授权登录页面跳转问题
- [系统优化] bool值表单联动判断
- [系统优化] 文件库文件删除脏数据异常问题
- [系统优化] 组件jsonKeyValue列表和详情显示优化
- [系统优化] GridFilter增加hidden属性，支持自定义条件回调
- [系统优化] CurlUtil 请求头 referer 默认值调整为空
- [系统优化] 事件触发工具类参数优化
- [Bug修复] 模块管理配置缓存失效问题
- [Bug修复] 非模型字段在复制和编辑时填充异常问题



### V1.7.0

**发布时间**：2024-04-08

- [新功能] 默认图标增加抖音图标（iconfont icon-douyin）
- [新功能] JS 库增强 MS.ui.elementMover，支持元素动态移动效果
- [新功能] Decimal 组件增加 unit、unitPosition 属性，支持单位显示
- [新功能] 用户积分新增冻结、提交、取消三阶段操作功能
- [新功能] 用户积分流水增加其他信息，支持冻结交易、管理员变更等信息展示
- [新功能] 用户积分后台操作支持记录管理员 ID
- [新功能] 后台用户钱包流水增加其他信息，可记录后台管理员变更信息
- [新功能] 用户前台积分冻结记录显示功能
- [新功能] 图片上传是否压缩可通过配置文件配置（默认开启压缩）
- [新功能] 富文本编辑器迷你版增加 markdown 内容导入功能
- [新功能] Curl 工具类请求增加 writeFunctionCallback 参数，支持流式请求
- [新功能] JS 库增加 markdown 操作工具类，支持 markdown 转 html
- [新功能] 系统全局消息提示 UI 全新优化
- [新功能] JS 库增加【ijs】类型字符串，支持默认可执行代码
- [新功能] 分类快捷操作工具类 CategoryUtil
- [新功能] 支付结算页面增加说明标题和内容
- [新功能] 财务概况增加最近7日和30日收款金额统计
- [新功能] Display 组件 asLink 参数支持回调模式，支持自定义链接
- [新功能] 首页增加今日收款金额统计报表
- [新功能] 桌面快捷应用，支持将网页快捷方式添加到桌面（安装 DesktopApp）
- [新功能] 管理登录背景 AdminLoginBackground
- [新功能] 后台登录提示 AdminLoginNotice 功能
- [新功能] 日志查看器 LogViewer 功能
- [新功能] 随机用户头像 MemberRandomAvatarTecmz 功能
- [新功能] 网页复制追加文字 CopyAppender 功能
- [新功能] 升级 XGPlayer 库，更好支持 HLS 视频播放
- [新功能] 支付结算工具类增加详细日志，方便问题排查
- [新功能] 后台白色清爽主题，可通过设置 ADMIN_THEME=default 切换后台主题
- [新功能] 后台用户列表支持一键登录，方便管理员快速登录用户中心（默认关闭，需要在模块管理中开启）
- [新功能] Time组件增加秒存储方式，方便存储时间精确到秒
- [新功能] 邮件发送成功与否增加判断
- [新功能] AdminConfigBuilder 增加 pageAppend 方法，方便在页面中追加内容
- [新功能] AdminConfigBuilder 增加 hookFormWrap 方法，方便自定义组建表单
- [新功能] 运营报表-用户数据页面，支持统计报表和每日明细
- [新功能] 后台支持 Widget 动态请求，方便开发者自定义页面内容
- [新功能] 时间工具增加日期范围限定功能
- [新功能] 搜索 like 关键词转义方法，模糊搜索时不再受特殊字符影响
- [新功能] 运营报表-网站访问页面，合并设置和详细页面
- [新功能] Text 新增 asLink 方法，支持内容以链接形式展示
- [新功能] 支持 modstart:module-list 命令，列出当前系统已安装、系统配置模块
- [系统优化] 搜索引擎蜘蛛检测库优化
- [系统优化] 后台登录界面自适应不同设备，界面升级
- [系统优化] 模块管理模块缓存优化，模块存在真实性判断
- [系统优化] 后台登录界面左侧宽度自动增加样式问题，标题边距调整
- [系统优化] GridFilter 筛选 range 查找逻辑优化
- [系统优化] 后台管理首页服务器信息显示优化
- [系统优化] 后台首页概况页面重构完成
- [系统优化] 后台报表数据最后一个元素水平间隙优化
- [Bug修复] 开启图片压缩，图片压缩失败的情况下继续上传
- [Bug修复] 多语言部分书写错误
- [Bug修复] 默认用户开通积分赠送不生效问题修复
- [Bug修复] 文档下载名称非法字符替换优化
- [Bug修复] 用户已安装模块概率性出现不能识别问题
- [Bug修复] 用户名字符长度提示文案异常问题
- [Bug修复] i18n 语言包文字书写错误纠正



### V1.6.0

**发布时间**：2024-02-27

- [新功能] NumberRange 组件支持，用于输入数字范围
- [新功能] 用户自动注册前缀可设置，优化用户显示逻辑
- [新功能] AdminConfigBuilder 增加配置保存检查回调函数，支持配置与检查
- [新功能] 队列调度支持work-max-jobs属性，支持进程批量处理
- [新功能] 用户删除事件触发 MemberUserDeletedEvent
- [新功能] 进程运行命令runInNewProcess，支持进程隔离运行
- [新功能] 时间工具类增加tomorrowDate方法
- [新功能] UEditorPlus 版本到 3.8.0
- [新功能] Form 表单组件增加 hookResponse 属性，支持自定义返回数据
- [新功能] 文件上传事件增加参数，用于区别用户、后台等文件上传类型
- [新功能] Select 组件增加 gridEditable 属性，支持表格编辑模式
- [新功能] Redis 增加 isEnableSuccess 判断是否启用成功
- [系统优化] 授权登录默认注册为用户昵称（昵称不可作为登录用户名）
- [系统优化] 动画样式类优化
- [系统优化] 异常错误日志 URL 获取优化，提高定位效率
- [Bug修复] 用户删除自动清除授权登录信息



### V1.5.0

**发布时间**：2024-01-16

- [新功能] 有移动端链接时，后台链接选择自动识别电脑端和移动端筛选
- [新功能] ComplexFieldsList 组件支持链接和颜色选择
- [新功能] 用户文件上传增加type字段，区分文件类型
- [新功能] CurlUtil::mockUserAgent 支持模拟真实UA
- [新功能] 图片水印工具类全面优化，支持文字单行、文字多行、图片单个、图片多个
- [新功能] 用户密码增加强度校验，支持不限、字母数字、长度限制
- [新功能] 用户授权自动绑定开关，支持授权后立即登录
- [新功能] Values 组件新增 countFixed 属性，固定显示数量
- [新功能] 后台框架页面增加禁止搜索引擎爬取 meta 标签
- [新功能] 地址智能解析 AddressParseProvider
- [新功能] Request::mergeQueries 合并请求参数按参数名称排序，避免同业不同链问题
- [新功能] Form 支持原生 Response 直接返回，便于处理文件下载等表单
- [新功能] 用户授权登录时如果手机/邮箱已存在，直接关联已有用户
- [新功能] 增加用户账号申诉功能，支持用户自助找回账号、账号禁用申诉等用途
- [新功能] 请求输入 getBase64File 自动检测 Base64 文件前缀
- [新功能] 用户后台授权登录详细数据列表支持弹窗查看
- [系统优化] 系统图标样式统一优化
- [系统优化] RedisQueue一处多进程调度性能问题
- [系统优化] UEditor 图片抓取特殊 URL 文件类型判断优化，新增真实 UserAgent
- [系统优化] 组件when方法数据类型优化
- [系统优化] 用户账号管理界面按钮均调整为圆角样式
- [系统优化] AES加密函数解密异常时错误优化
- [Bug修复] 一处LayUI树tree多选问题
- [Bug修复] 后台 Job 执行时候，资源全路径修正问题
- [Bug修复] 一处图片分片上传异常问题
- [Bug修复] 概率性用户VIP时间异常问题



### V1.4.0

**发布时间**：2023-12-11

- [新功能] 临时上传文件data_temp自动清除调度任务
- [新功能] 后台支持多语言切换，默认关闭，需修改配置文件自行开启
- [新功能] Number 组件增加 min、max、step 属性
- [新功能] 轮播图获取支持近图片过滤方法
- [新功能] 网站模板可自定义设置弹窗，主题可自定义参数设置
- [新功能] 布局视图页面全局增加 headPrepend section
- [新功能] 前台右上角菜单增加用户中心下拉菜单
- [新功能] 模块资源软链接命令 modstart:module-link-asset
- [新功能] 文件上传管理页面支持图标显示，支持顺序选择
- [新功能] DataRefProvider 提供文件引用提供者模块
- [新功能] LayUI 升级到最新版
- [新功能] Tree 组件增加选项是否独立模式 independentEnable
- [新功能] 短信验证注册时可支持同时设置登录密码
- [新功能] 系统命令行安装和界面安装方式文档支持
- [新功能] 财务中心&rarr;全部订单新增&quot;业务订单ID&quot;筛选条件
- [新功能] 富文本支持文档一键导入，支持Word文档（docx）、Markdown文档（md）
- [系统优化] 临时文件删除文件不存在时候删除失败修复
- [系统优化] 后台多Tab菜单点击显示优化问题
- [系统优化] 后台登录页面自动检测框架嵌套并刷新
- [系统优化] 错误页面返回状态码404、403优化
- [系统优化] 系统响应默认处理函数优化处理方式
- [系统优化] 模块安装解压超时时间调整为 600 秒
- [系统优化] 前端 MS.dialog 在 layer 未加载时降级为原生
- [系统优化] Robot 蜘蛛检测 UserAgent 完善
- [系统优化] 数据表单 Grid 常规模式和简单模式底层重构完成
- [系统优化] 用户管理后台用户注册登录设置页面文案优化
- [系统优化] 用户VIP页面条目是否可视移动端接口优化
- [Bug修复] PageHtmlUtil::render 增加自定义分页渲染函数参数
- [Bug修复] 用户积分记录更新异常问题修复



### V1.3.0

**发布时间**：2023-10-30

- [新功能] 内核升级为3.8.0
- [新功能] 用户首页面板配置 MemberHomePanel
- [新功能] CRUDUtil新增scope获取，copyId新增默认值
- [新功能] 支持公共图片库（需安装DataGallery支持）
- [新功能] ENCRYPT_KEY默认系统数据加密密钥
- [新功能] 后台安全新增默认Key检测
- [新功能] 内外网链接节流映射配置
- [新功能] 统一错误处理增加特定状态码错误页面
- [新功能] ComplexFieldsList 组件增加 select 类型
- [系统优化] 后台管理安全公告位置调整
- [系统优化] 后台 data-tab-open 打开菜单自动定位
- [系统优化] 已过期的用户VIP，自动更新为普通用户
- [系统优化] 403错误页面样式升级调整
- [系统优化] 客服条样式调整优化
- [系统优化] 视频 Banner 概率不播放问题
- [Bug修复] 富文本字体设置不生效问题修复
- [Bug修复] 后台用户数据统计异常问题修复



### V1.2.0

**发布时间**：2023-10-05

- [新功能] 动态页面支付支付方式新增AlipayWeb
- [新功能] 同时增加多个数据库表备注方法
- [新功能] 支持MS.ui.state库方法，历史状态管理
- [新功能] 富文本公式编辑默认替换为LatexEasy
- [新功能] 手机端Banner支持视频背景显示
- [新功能] Grid文本组件支持快捷编辑
- [新功能] Grid快捷编辑gridEditable支持函数回调方式
- [新功能] UEditorPlus升级v3.4.0
- [新功能] MS.Util.browser 浏览器判断工具类
- [新功能] 文件上传Vue组件新增Flat模式和addFile方法
- [新功能] 友情链接支持独立页面 /partner 访问
- [新功能] 用户注册成功站内信和欢迎邮件
- [新功能] MemberAuthProvider支持自定义账号对接方式
- [新功能] SiteUrlProvider增加按业务变更方法
- [新功能] 富文本增加MP3文件等音频内容
- [新功能] ImageSelector支持show-preview-url参数，图片预览是否显示链接
- [新功能] 移动端增加c-rich-html组件，支持多端富文本兼容显示
- [系统优化] 多语言翻译功能逻辑和多语言函数
- [系统优化] 示例域名修改为 example.com
- [系统优化] 面包屑分隔符样式优化
- [系统优化] 支付回调非法请求日志记录和错误提示优化
- [系统优化] 样式sm、md、lg、xl尺寸优化
- [系统优化] 图片类组件预览修改为contain模式
- [系统优化] VIP开通快捷支付概率性异常问题
- [系统优化] 表单提交时交互验证未完成逻辑优化
- [系统优化] 富文本编辑公式编辑组件重复去除
- [系统优化] 富文本HTML过滤新增div标签
- [系统优化] 后台注册登录链接生成使用非路由生成
- [系统优化] 树状结构Select显示优化
- [系统优化] AES加密解密方法优化，支持更多模式
- [系统优化] 表单快速编辑功能优化
- [Bug修复] 数字组件为0时默认值显示异常问题
- [Bug修复] 图片上传自动纠正方向和大小异常格式修复
- [Bug修复] 数组随机获取异常问题修复



### V1.1.0

**发布时间**：2023-08-12

- [新功能] 手机、邮箱验证码校验失效日志
- [新功能] Json组件支持API请求通用配置模式 jsonMode(Json::MODE_API)
- [新功能] Form排序新增scope过滤
- [新功能] Form支持排序集合增加到头和尾sortAddPosition配置
- [新功能] MS.eventManager对象，方便页面事件管理
- [新功能] 用户注册、登录、找回密码等页面增加canonical优化爬虫路径
- [新功能] 增加TRACK_LONG_SQL_THRESHOLD配置可配置慢查询阈值，默认5000ms
- [新功能] 网站访问记录增加忽略爬虫开关功能，避免记录无效访问记录
- [新功能] FileUtil新增MIME转文件后缀方法
- [新功能] CurlUtil新增返回headerMap数据
- [新功能] GridFilter中like条件新增wordSplit模式，默认中文会分为单字查询，安装WordSpliter可对中文分词
- [新功能] StrUtil增加wordSplit通用分词功能
- [新功能] GridFilter下拉组件全部（All）选项是否显示可配置
- [新功能] BizException支持自定义特定异常视图
- [新功能] ComplexFields组件新增tip提示文字选项
- [新功能] DynamicFields增加多行文本框组件
- [新功能] VIP页面用户开通VIP增加快捷扫码支付
- [新功能] 会员VIP充值页面新增弹窗模式
- [新功能] 客服功能新增弹窗页面，二维码信息尺寸优化
- [新功能] 支付中心快速订单自动清理功能
- [新功能] Checkbox组件支持when条件模式
- [新功能] ComplexFields组件支持slider输入子项
- [新功能] 系统默认绘图字体调整为阿里巴巴普惠体
- [新功能] 系统默认FontProvider
- [新功能] 内置Markdown编辑器修改为ToastUI
- [新功能] 升级webuploader，引入图片上传全局压缩功能
- [系统优化] 图片上传、视频上传、文件上传、音频上传组件重构
- [系统优化] 模块设置页面增加开发配置提醒，避免随意设置导致的功能异常
- [系统优化] xForwardedHostVisitRedirect配置防止CDN域名多URL访问
- [系统优化] 后台菜单搜索父级包含关键词时自动显示子项
- [系统优化] 后台管理多标签页面背景和Loading效果
- [系统优化] 按钮样式边框兼容性优化
- [系统优化] 系统主题色自动切换样式优化
- [系统优化] 快捷扫码支付界面显示优化
- [系统优化] 数据表格新增弹窗到标签返回列表自动刷新
- [系统优化] 表单输入组件边距样式优化
- [系统优化] 顶部菜单用户中心增加退出按钮下拉菜单
- [系统优化] 安装向导伪静态测试浏览器缓存问题
- [系统优化] 模块市场、系统升级登录表单提交交互优化
- [Bug修复] Number、Text组件默认值不生效问题
- [Bug修复] Tags组件数据表格显示异常问题
- [Bug修复] 用户授权登录头像后缀概率性获取异常问题修复
- [Bug修复] 上传文件概率性进度条不显示问题
- [Bug修复] Tree组件默认值显示异常问题
- [Bug修复] 二维码生成类中文字符异常问题修复
- [Bug修复] 组件Tags查看模式空值异常问题



### V1.0.0

**发布时间**：2023-06-28

- [新功能] 多应用导航系统


## 演示地址

[http://links.demo.tecmz.com](http://links.demo.tecmz.com)

## 下载试用

[http://tecmz.com/product/links](http://tecmz.com/product/links)