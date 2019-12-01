# 目录

- [目录](#%e7%9b%ae%e5%bd%95)
- [相关文档](#%e7%9b%b8%e5%85%b3%e6%96%87%e6%a1%a3)
  - [用例图](#%e7%94%a8%e4%be%8b%e5%9b%be)
    - [学生](#%e5%ad%a6%e7%94%9f)
    - [社长](#%e7%a4%be%e9%95%bf)
    - [管理员](#%e7%ae%a1%e7%90%86%e5%91%98)
    - [用户](#%e7%94%a8%e6%88%b7)
  - [时序图](#%e6%97%b6%e5%ba%8f%e5%9b%be)
    - [学生](#%e5%ad%a6%e7%94%9f-1)
      - [申请参加活动](#%e7%94%b3%e8%af%b7%e5%8f%82%e5%8a%a0%e6%b4%bb%e5%8a%a8)
      - [申请参加社团](#%e7%94%b3%e8%af%b7%e5%8f%82%e5%8a%a0%e7%a4%be%e5%9b%a2)
      - [申请组成社团](#%e7%94%b3%e8%af%b7%e7%bb%84%e6%88%90%e7%a4%be%e5%9b%a2)
      - [查看社团信息](#%e6%9f%a5%e7%9c%8b%e7%a4%be%e5%9b%a2%e4%bf%a1%e6%81%af)
      - [查看活动信息](#%e6%9f%a5%e7%9c%8b%e6%b4%bb%e5%8a%a8%e4%bf%a1%e6%81%af)
    - [社长](#%e7%a4%be%e9%95%bf-1)
      - [申请活动](#%e7%94%b3%e8%af%b7%e6%b4%bb%e5%8a%a8)
      - [发布公告](#%e5%8f%91%e5%b8%83%e5%85%ac%e5%91%8a)
      - [批准参加活动](#%e6%89%b9%e5%87%86%e5%8f%82%e5%8a%a0%e6%b4%bb%e5%8a%a8)
    - [管理员：](#%e7%ae%a1%e7%90%86%e5%91%98)
      - [批准换届申请](#%e6%89%b9%e5%87%86%e6%8d%a2%e5%b1%8a%e7%94%b3%e8%af%b7)
      - [批准申请活动](#%e6%89%b9%e5%87%86%e7%94%b3%e8%af%b7%e6%b4%bb%e5%8a%a8)
  - [成员：](#%e6%88%90%e5%91%98)
      - [提交职位申请](#%e6%8f%90%e4%ba%a4%e8%81%8c%e4%bd%8d%e7%94%b3%e8%af%b7)
  - [类图](#%e7%b1%bb%e5%9b%be)
    - [1.UserManager （用户管理类）](#1usermanager-%e7%94%a8%e6%88%b7%e7%ae%a1%e7%90%86%e7%b1%bb)
    - [2.AssociationManager （社团管理类）](#2associationmanager-%e7%a4%be%e5%9b%a2%e7%ae%a1%e7%90%86%e7%b1%bb)
    - [3.AssApplyManager （社团申请操作类）](#3assapplymanager-%e7%a4%be%e5%9b%a2%e7%94%b3%e8%af%b7%e6%93%8d%e4%bd%9c%e7%b1%bb)
    - [4.AnnouncementsManager （通知管理类）](#4announcementsmanager-%e9%80%9a%e7%9f%a5%e7%ae%a1%e7%90%86%e7%b1%bb)
    - [5.ActivityManager (活动管理类)](#5activitymanager-%e6%b4%bb%e5%8a%a8%e7%ae%a1%e7%90%86%e7%b1%bb)
    - [6.FinancialManager （财务管理）](#6financialmanager-%e8%b4%a2%e5%8a%a1%e7%ae%a1%e7%90%86)
- [分工](#%e5%88%86%e5%b7%a5)

# 相关文档


需求文档：[需求](https://www.cnblogs.com/klchen/p/11789040.html)

第一次例会报告： [例会报告](https://github.com/schedule-front/EveryWeekRePort/blob/master/%E4%BE%8B%E4%BC%9A/%E7%AC%AC%E4%B8%80%E6%AC%A1%E4%BE%8B%E4%BC%9A.md)

阶段性总结一: [总结](https://github.com/schedule-front/EveryWeekRePort/blob/master/week2/weeksummary.md)

文档预览(可能需要梯子): [GITBOOK](https://klchen.gitbook.io/everyweekreport/) 


## 用例图

### 学生

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/C_Stu.png)

### 社长

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/C-pre.png)

### 管理员

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/C_ad.png)

### 用户

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/C_User.png)

## 时序图

### 学生

#### 申请参加活动

非社团成员需提交申请，等待社长审批才可参加活动

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/ApplyForActivities.png)

#### 申请参加社团

非社团成员需提交申请，等待社长审批才可参加社团

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/Stu_ApplyAssociation.png)


#### 申请组成社团

非社团成员需提交资质证明，可以向管理员提交社团组建申请

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/Stu_ApplyForFormAssociation.png)

#### 查看社团信息

社员及非社员，有不同权限查看，但管理员全体公告，所有学生均可查看

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/Stu_AssociationInfo.png)

#### 查看活动信息

学生登陆后即可在社团界面查看

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/stu_ActivityInfo.png)

### 社长

#### 申请活动

社长向管理员申请活动

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/pre_ApplyActivity.png)

#### 发布公告

社长发布公告，可以选择是社员可见还是全体学生可见

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/pre_Notice.png)

#### 批准参加活动

社长具有批准非本社成员的参加活动请求权限

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/pre_ApproveApplyActivity.png)

### 管理员：

#### 批准换届申请

管理员批准社长提交的换届申请

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/AffirmJobApplication.png)

#### 批准申请活动


管理员批准社长提交的活动

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/Admin_ApproveApplicationForAssociation.png)

## 成员：

#### 提交职位申请

所有社团人员都可以参与，但是只有社长能提交换届申请

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/Member_JobApplication.png)


## 类图

![](https://github.com/schedule-front/EveryWeekRePort/raw/master/week2/pic/ClassPic.png)

### 1.UserManager （用户管理类）

* getRole(): 根据user表-rid属性，从Role表获取用户角色信息
* getPermission():根据角色信息从permission表获取用户权限信息
* login():验证账号密码登陆，提供token
* updateHeadImg():上传新的头像
* modifyInfo():修改个人信息
* modifyPasswd():修改密码

### 2.AssociationManager （社团管理类）

* changePreApply(): 申请社长换届
* passPreApply(): 同意换届申请
* denyPreApply(): 拒绝换届申请
* quitAss(): 退出社团
* uploadLogo():上传社团logo
* modifyAssInfo();修改社团信息
* deleteMember():踢出社员
* searchAss():搜索社团
* addAss():管理员操作，添加社团
* deleteAss():管理员操作，删除社团
  
### 3.AssApplyManager （社团申请操作类）

* postApply():发起加入社团申请
* deleteApply(): 删除申请
* modifyApply(): 修改申请
* checkStatus(): 查看申请状态
* passApply(): 社团管理者同意申请
* denyApply(): 社团管理者拒绝申请

### 4.AnnouncementsManager （通知管理类）

* getAnn():获取通知
* postAssAnn(): 社团管理者发起社团通知
* postSysAnn()：系统管理员发起系统通知
* deleteAnn(): 删除通知
* modifyAnn(): 修改通知

### 5.ActivityManager (活动管理类)

* checkAct(): 查看活动
* checkApplyStatus(): 查看活动申请结果
* addActApply(): 提出活动申请
* deleteActApply(): 删除活动申请
* modifyActApply(): 修改活动申请
* passActApply(): 系统管理员同意活动申请
* denyActApply(): 系统管理员拒绝活动申请

### 6.FinancialManager  （财务管理）

* addFinancial(): 提交财务报表
* passFin(): 财务报表审核通过
* denyFin(): 财务报表审核拒绝
* checkStatus(): 查看财务报表状态



# 分工

|学号 | 姓名  | 分工|
|---- |-------| -----|
|31701079 | 沈臻阳 | 文档编写|
|31701068 | 曹隆翔 | 文档编写|
|31701069 | 陈凯隆 | 时序图，用例图，文档编写|
|31701180 | 金旻儒 | 用例图，类图|