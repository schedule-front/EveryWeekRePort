# 往期报告

[每周进展](https://github.com/schedule-front/EveryWeekRePort)

[社团管理系统需求分析 第一组](https://www.cnblogs.com/klchen/p/11789040.html)

[第二次总结报告](https://www.cnblogs.com/klchen/p/11886790.html)

[社团管理系统设计图 第一组](https://www.cnblogs.com/klchen/p/11886791.html)

[接口文档](https://www.showdoc.cc/591919243440236)

# 目录
- [往期报告](#%e5%be%80%e6%9c%9f%e6%8a%a5%e5%91%8a)
- [目录](#%e7%9b%ae%e5%bd%95)
- [前端页面展示](#%e5%89%8d%e7%ab%af%e9%a1%b5%e9%9d%a2%e5%b1%95%e7%a4%ba)
  - [登录界面](#%e7%99%bb%e5%bd%95%e7%95%8c%e9%9d%a2)
  - [主页面](#%e4%b8%bb%e9%a1%b5%e9%9d%a2)
  - [社团浏览页面](#%e7%a4%be%e5%9b%a2%e6%b5%8f%e8%a7%88%e9%a1%b5%e9%9d%a2)
  - [社团详情页面](#%e7%a4%be%e5%9b%a2%e8%af%a6%e6%83%85%e9%a1%b5%e9%9d%a2)
  - [社团加入申请页面](#%e7%a4%be%e5%9b%a2%e5%8a%a0%e5%85%a5%e7%94%b3%e8%af%b7%e9%a1%b5%e9%9d%a2)
  - [社团加入申请审批页面](#%e7%a4%be%e5%9b%a2%e5%8a%a0%e5%85%a5%e7%94%b3%e8%af%b7%e5%ae%a1%e6%89%b9%e9%a1%b5%e9%9d%a2)
  - [活动浏览/通知页面](#%e6%b4%bb%e5%8a%a8%e6%b5%8f%e8%a7%88%e9%80%9a%e7%9f%a5%e9%a1%b5%e9%9d%a2)
  - [活动申请页面](#%e6%b4%bb%e5%8a%a8%e7%94%b3%e8%af%b7%e9%a1%b5%e9%9d%a2)
  - [活动审核表单](#%e6%b4%bb%e5%8a%a8%e5%ae%a1%e6%a0%b8%e8%a1%a8%e5%8d%95)
  - [活动审批详情页面](#%e6%b4%bb%e5%8a%a8%e5%ae%a1%e6%89%b9%e8%af%a6%e6%83%85%e9%a1%b5%e9%9d%a2)
  - [通知详情页面](#%e9%80%9a%e7%9f%a5%e8%af%a6%e6%83%85%e9%a1%b5%e9%9d%a2)
  - [通知管理页面](#%e9%80%9a%e7%9f%a5%e7%ae%a1%e7%90%86%e9%a1%b5%e9%9d%a2)
  - [不同权限用户的页面](#%e4%b8%8d%e5%90%8c%e6%9d%83%e9%99%90%e7%94%a8%e6%88%b7%e7%9a%84%e9%a1%b5%e9%9d%a2)
- [分工与计划](#%e5%88%86%e5%b7%a5%e4%b8%8e%e8%ae%a1%e5%88%92)
  - [分工](#%e5%88%86%e5%b7%a5)
  - [本周分工](#%e6%9c%ac%e5%91%a8%e5%88%86%e5%b7%a5)
  - [下周计划](#%e4%b8%8b%e5%91%a8%e8%ae%a1%e5%88%92)


# 前端页面展示

## 登录界面

![LoginPage](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/loginView.png)

## 主页面

![MainPage](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/MainPage.png)

* 登陆后跳转至主界面
* 主页面右上方为个人信息
* 侧边栏为各个模块的跳转界面
* 左上方的模块记录访问历史记录，方便使用

## 社团浏览页面

![TeamView](https://github.com/schedule-front/EveryWeekRePort/blob/master/week4/img/AllClub.png?raw=true)

* 上侧为人气社团的推荐展示滚动栏
* 下方为所有社团的展示
* 点击可进入社团的详细展示页面
* 通过分页控制了一页所展示的社团数量

## 社团详情页面

![TeamDetail](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/ClubDetails.png)

* 左上角展示了社团的名称、社长以及相关评分
* 左下角展示了社团的相关荣誉情况
* 右上角和右下角分别展示了社团的简介和相关活动开展的情况
* 学生可以在此页面申请加入对应的社团

## 社团加入申请页面

![EnterApplyPage](https://github.com/schedule-front/EveryWeekRePort/blob/master/week4/img/TeamSubmit.png?raw=true)

* 个人信息会根据你的个人信息自动填充
* 对部分输入框增加了字数统计功能
     
## 社团加入申请审批页面

![EnterReviewPage](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/ApplyA.png)

* 该页面仅有相关社团的社长可见
* 该页面的学生提交信息均无法修改
* 社长可以选择同意或拒绝未被审批过的申请

## 活动浏览/通知页面

![ActivityView](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/allAnnouncements.png)

* 每条活动信息都包含了申办社团、活动标题、活动日期等基本信息
* 可以通过点击进入相关活动的详细展示页面

## 活动申请页面

![ActivityApply](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/ActivityCrt.png)

* 该页面仅有社长可见
* 申请信息包含了必要的内容

## 活动审核表单

![ActList](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/ActivityList.png)

* 该页面仅有管理员可见
* 该页面包含了活动的基本信息
* 活动的审批状态颜色直观形象
      
## 活动审批详情页面

![ActivityReview](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/ApplyB.png)

* 该页面仅有管理员可见
* 该页面所有信息均无法修改
* 管理员可以选择同意或拒绝未被审批过的申请

## 通知详情页面

![NoticeDetail](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/noticeDetail.png)

## 通知管理页面

![NoticeManager](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/noticeManager.png)

* 该页面仅有社长可见
* 该页面包含了管理通知所需的绝大部分信息

## 不同权限用户的页面
   
![A](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/RoleA.png)
   
* 普通学生页面
   
![B](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/RoleB.png)
   
* 社长页面
   
![C](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week4/img/RoleC.png)
   
* 管理员页面


# 分工与计划

## 分工

| 姓名   | 具体分工                                               |
| ------ | ------------------------------------------------------ |
| 金旻儒 | 后端，提供了各类基本展示与提交的接口、并实现前后端连接 |
| 陈凯隆 | 后端，提供了各个数据库基本测试                         |
| 曹隆翔 | 前端，UI设计、接口连接测试                             |
| 沈臻阳 | 前端，UI设计、路由设计、UI美化                         |


## 本周分工

| 姓名   | 具体分工                                                                       |
| ------ | ------------------------------------------------------------------------------ |
| 金旻儒 | 后端接口设计开发（java）、前后端连接测试、Shiro验证                            |  |
| 陈凯隆 | 接口与数据库连接测试，通过连接表查询测试                                       |
| 曹隆翔 | 完成了大部分前端页面的设计、并完成了一部分前端页面与后端接口进行数据传输的功能 |
| 沈臻阳 | 完成了部分前端页面的设计、完成了用户权限的动态路由，文档编写                   |


## 下周计划


| 姓名   | 具体分工                                                   |
| ------ | ---------------------------------------------------------- |
| 金旻儒 | 完成各类审批、管理相关的API、并与前端连接                  |  |
| 陈凯隆 | 完成剩下复杂数据库的接口测试及实现                         |
| 曹隆翔 | 完成总体前端页面设计、与后端所有接口进行连接               |
| 沈臻阳 | 完成前端优化、增加部分附加功能、完成后端接口连接 |

   
