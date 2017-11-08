README
===========================
该文件用来说明新版股吧文件frontend的相关内容

****
	
|Author|ztq|
|---|---
|E-mail| tianqi1@eastmoney.com


# 主文件在page中，包括list.html 和 list.js 部分
    list.html 为显示页面，测试页面要再list_2017.aspx进行修改，并提交到堡垒机中
    list.js  为主页面的逻辑部分。
    
# 界面的每个部分分成模块，分布在文件夹module中

## body文件中包括 正文的表单  
     listHeader : 为内容页面的头部部分；
     listFooter: 为内容页面的尾部，主要是页码部分逻辑；
     publishnew: 发表新主题的整个界面样式，以及问董秘部分逻辑；
     editor ：发表新主题的编辑器，基于百度umeditor；

## footer文件为整个页面的底部模块 

## header文件为整个页面的头部模块

## right文件为整个页面的右部模块
     ad: 广告模块
     belongs: 所属概念模块
     bkdata: 所属行业涨跌幅模块
     dapan: 大盘模块
     hottopic: 热门话题模块
     newstockinfo: 新股后边行情模块
     reportTab: 公告模块
     rightZaiKan: 大家都在看模块
     searchInfo: 查行情 查资金流 搜索模块
     somegbtab: 沪深右边的行情模块

## top文件为整个内容模块的顶部模块      
      gbsearch：顶部的搜索模块
      history: 历史浏览记录模块
      location: 当前股吧的路径模块
      scrollheader: 顶部悬浮模块
      somegbmaininfo: 当前股吧的主要信息，包括特色数据，f10档案等
      somegbinfoheaderOne: 当前股吧的吧名，帖子数和相关话题
    
## common 文件中包括弹出框      
      hint: error 等提醒模块的弹出框通用模板
      modal：登录框和验证码模块的较大的弹出框通用模块
      shiming: 实名制弹出框模块
      tooltipster: jquery 的tooltipster的插件，用于悬浮弹出框
      vcode: 验证码模块逻辑

## hepler 文件为通用的逻辑模块      
      helper.js: 所有hepler文件的汇总
      ajax_upload.js: 用于为editor服务，用于上传图片，上传视频等功能
      cookie.js: cookie 的简单获取和操作
      errorCode.js: 验证器(目前还没有用到）
      follow.js: 关注和取消关注 股票和人 的逻辑
      influence.js: 用户影响力逻辑
      jsplugin.js: 用于实现背景的闪烁
      net.js: ajax, jsonp 等请求的封装
      observe.js: 观察者模式，目前用于editor.js 中
      popmsg.js: 悬浮框界面及相关逻辑
      stock.js: 判断当前的股票类型
      storage.js: 判断是否在localstorage 还是在 cookie 中，并进行处理
      text.js: 对文本进行相应的处理
      time.js: 时间字符串处理 其中 parseISO8601 为了兼容性ie7
      url.js: 对url 进行处理（目前还没有用到）
      user.js: 获取用户信息
      validator.js: 验证器(目前还没有用到)

# 运行代码
      latte debug 运行代码，进行本地测试
      latte release 运行代码，将release文件中的list.js， img文件和list.css 传入堡垒机
      latte sprite 获取图片精灵 图片在sprite 文件夹中，生成的代码在sprite_common.css 文件中 


