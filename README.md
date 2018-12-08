# 小程序审核发布经验

## 审核时间
小程序的审核在1小时到N天不等。官方说法是不超过7个工作日，一般在3天内会有结果。（但也有用户反馈超过7个工作日仍未审核。）
审核过程中可以撤回。除非有严重Bug，不建议撤回。因为重新提交，可能需要重新“排队”。
周末、节假日，微信审核团队会安排少量同事值班。（运气好的话，周末提审，也能当天通过。）
所以只要有一个可发布的版本，尽早提交审核。

## 注册小程序的主体
个人和企业均可注册小程序。但是很多类目未对个人开放，限制太多。如果小程序的服务类目不在个人允许的范围内，建议想办法使用企业主体（如注册个体工商户）。

例如使用个人身份注册小程序，发表文章（如博客），一般会认为涉及资讯而被拒绝（因为资讯类未开放给个人）。除非技术教程类的文章，可以勉强通过，但容易被误判。

## 常见被拒绝情形

### 诱导关注、诱导分享朋友圈
小程序拒绝之万能法宝1，凡涉及到关注公众号、分享到朋友圈，均可能被封掉相应接口。对于“分享到朋友圈”，官方建议不要出现“朋友圈”字样或图标，可改为“保存图片”。（实际上目前也只能保存图片到系统相册，然后再分享到朋友圈。）

生成的分享图片包含二维码或小程序码，可能会被拒绝通过（官方说法是涉及平台未允许的内容）。

### 虚拟支付
小程序拒绝之万能法宝2，凡非实物销售均可列入此范围。如付费购买音视频内容、付费购买教育课程、付费升级会员等。

### 未取得腾讯授权，不可以借助其他小程序或app实现自身功能
如优惠券、导购类小程序。官方的答复是“领取优惠券需要复制券地址前往淘宝才算真正领取成功，属于借助其他APP实现自身功能体验”。此类小程序很大概率会被审核不通过。

### 需补充社交-笔记类目
涉及可编辑、转发的小程序，涉及用户自定义内容及分享的小程序。如果小程序名称中含有“社区”字样，而小程序内容并无社区产品，多半会要求提供社区相关资质，因此起名也要注意。

### 需补充社交-社区/论坛类目
涉及UGC内容，可进行回复互动，如可发贴交流的小程序。

### 需补充文娱-视频类目
涉及在线视频观看的小程序。

### 可用性和完整性不符合规则
小程序无具体运营内容，无法正常体验小程序。很可能是程序Bug所致，新用户（或者审核人员）打开时，不显示内容或者内容过少。建议多测试，模拟新用户或者用新的微信账号测试。同时确保提交审核的版本，有一定内容，不要出现大块的空白。建议不要显示“即将上线”的字样，等开发好了再显示该功能。

### 关于电商平台与商家自营类目
如果小程序涉及商家入驻，为商家提供开店服务，必须选择电商平台。

### 无法被搜索
部分包含恶意或风险信息的小程序（如涉嫌混淆官方产品名称、色情低俗、欺诈等），可能不能被搜索出。如“郑州推拿按摩理疗”无法被搜索，但“郑州推拿”则可以。

### 小程序实际所提供的服务属于尚未开放的服务类目
未开放的服务有很多。这里主要是指偏门的服务，如寺院（线上供佛）服务。

### 小程序服务涉及可编辑、发布内容，属个人未开放类目
以个人为主体开发的小程序，目前限制太多，基本上只能做信息查询类小程序。

### 涉及xxx，请补充xxx相关类目
但是在小程序后台设置中的服务类目已经添加了xxx类目。其实还需要在提交审核时，配置功能页面，选择相应的服务类目。可以多配置几个功能页面，将设置中的服务类目全部涵盖。

## 注意事项

多测试，减少 Bug 数量，杜绝严重 Bug。在审核周期较长的情况下，减少提交审核的次数；在审核周期较短的情况下，提高提交审核的次数。

不要和别人比。别人的类似小程序能上架，你的不一定能上，原因没有。开发者要做好心理准备。

申请附近的小程序，证件号码必须完全正确，包括字母的大小写。如易混淆的阿拉伯数字“0”与英文字母“O”。

同一时间提交的小程序，不一定同一时间审核。具体审核的顺序尚不明确。

前面几次审核通过，不代表下一次审核能通过，哪怕只是改了一个Bug。因为后续审核可能发现新的“违规”问题。

文娱、社交类小程序一般会进入二次审核，由当地主管部门（网信办）审核，时间一周左右（也有用户反馈等待1个月仍未审核）。如长时间（1个月以上）仍未审核，只能联系当地主管部门，或者考虑重新提交审核。

小程序中不要出现色情、低俗内容，否则被用户举报后，容易被暂停服务。

不要在提交审核的小程序中使用测试数据，如页面上存在明显的“测试”字样。

名称中含有特殊行业名词，若没有选择相应类目，很可能会被拒绝。如名称中有“保险”二字，会要求你提供保险行业的资质。特殊名称还有：社区。

涉及区块链、贷款、彩票（只能做彩票开奖结果查询，但容易被误判）、色情低俗、代购、网赚、优惠券的小程序，基本通不过。赞赏小程序可能会被拒绝，原因是属于尚未开放的服务类目。

服务类目，尽量在创建小程序时一次性选择全面。因为后面再增加服务类目，可能需要审核，审核时间不等。

不要在页面提供二维码，供用户下载 App，否则可能会被视为“诱导下载”。

红包类小程序必须选择“社交红包”类目，且需要“增值业务电信许可证”。

涉及到UGC（用户产生内容），最好建立审核机制与关键词屏蔽功能。

小程序审核通过后，应该尽早发布。如果审核通过后，未发布，此时再提交审核，之前审核通过后的版本可能会消失。

通过第三方平台提交代码，有提交数量的限制（7天内100个左右）。当接口返回 85085 submit audit reach limit, please try later hint，表示第三方平台近7天提交审核的小程序数量过多，请耐心等待审核完毕后再次提交。为此，一些第三方平台采用半自动提交。需要在小程序管理后台取消第三方授权，通过第三方平台上传代码，再到小程序管理后台手动提交审核。

## 技巧

### 版本升级
后端应做到后向兼容，至少需要兼容2个版本，线上版本和待提交审核的版本。先发布后端，测试一遍线上版本，确保线上版本在新版小程序提审期间，仍然可用。

严格来讲，要确保所有旧版本的接口可用，因为时间较早之前的用户打开小程序，很可能是旧的版本。详见版本[更新机制](https://developers.weixin.qq.com/miniprogram/dev/framework/operating-mechanism.html "微信小程序版本升级机制")。

若提交审核几天后仍然处在审核中，除发现重大 Bug 外，尽量不要撤回。既然已等待几天，不妨再等两天。一般七天内肯定会审核。

关于企业认证中给腾讯账号小额打款，腾讯公司的小额打款账号为招商银行25位账号，若不支持，则不要选择这种方式认证。

## 审核人员的设备与环境

- 测试环境wifi/4G，Andriod 5.1，微信6.6.7，OPPO R9tm
- 测试环境wifi/4G，Andriod 6.0.1，微信6.6.6，OPPO R9tm
- 测试环境wifi，   Andriod 6.0.1，微信6.6.5，OPPO R9s
- 测试环境wifi/4G，Andriod 6.0.1， 微信6.6.5，OPPO R9s plus
- 测试环境wifi，   Android 5.1.1，6，微信6.6.5，OPPO R7 PlusM
- 测试环境wifi/4G，Andriod 7.1.1，微信6.6.5，VIVO X9
- 测试环境wifi,Andriod 7.0，微信6.6.5，Honor V9
- 测试环境wifi，Iphone 11.2.6，微信6.6.5，Iphone SE
- 测试环境wifi，IOS11.3.1，微信6.6.7/微信6.6.5，iPhone6
- 测试环境wifi，Andriod 6.0.1，微信6.6.5，LEX726
- 测试环境wifi，Andriod 7.1.2，微信6.6.7，红米5 Plus

可以根据情况，选择以上手机作为测试机。

## 赚取收入

开通流量主，在小程序中展示微信提供的广告，即可赚取收入。

- 2018-03-26 小程序流量主内测邀请（平均日活3000+的小程序）
- 2018-07-09 小程序流量主全面开放（累计用户数达到1000即可申请）

广告形式为CPC（按点击付费），每次点击产生的收入不等，大致范围为0.1元~2元（取决于广告主的定价）。

第一次提审带广告的小程序，需要等待微信对广告的审核，审核通过前，正式版小程序不会显示广告。

微信小程序官方邮件地址：MiniProgram#tencent.com （将#换成@）

如有疑问，或得发现错误，请评论反馈。

更新时间：2018/12/5
