# 社团管理系统需求分析

<!-- TOC -->

- [社团管理系统需求分析](#社团管理系统需求分析)
- [亮点](#亮点)
    - [一、项目分工](#一项目分工)
    - [二、项目背景](#二项目背景)
    - [三、系统简介](#三系统简介)
    - [四、项目需求](#四项目需求)
        - [社长：](#社长)
        - [学生：](#学生)
        - [社员：（同时具有学生这个角色包含的需求）](#社员同时具有学生这个角色包含的需求)
        - [系统管理员（学校方）](#系统管理员学校方)
    - [五、数据流图](#五数据流图)
    - [六、项目原型](#六项目原型)
    - [七、项目技术](#七项目技术)
- [前后端接口定义模块](#前后端接口定义模块)
    - [基本说明](#基本说明)
    - [User/Admin](#useradmin)
        - [java类](#java类)
        - [表结构](#表结构)
        - [注册](#注册)
            - [请求](#请求)
            - [JSON格式](#json格式)
        - [登陆](#登陆)
            - [请求](#请求-1)
        - [找回密码](#找回密码)
    - [Association](#association)
        - [java类](#java类-1)
        - [表结构](#表结构-1)
    - [Announcements](#announcements)
        - [java类](#java类-2)
        - [表结构](#表结构-2)

<!-- /TOC -->

# 亮点

1. 用github管理每周报告及项目文档 [EveryWeekRePort](https://github.com/schedule-front/EveryWeekRePort)
2. 墨刀原型
   1. [web端原型](https://free.modao.cc/app/6cd60f302a30c3d032772f10b80555602fc9fd0c/embed)
    2. [app端原型](https://free.modao.cc/app/nblmz4zia8k2iw45l4dvmwtewjw2s/embed)
   

## 一、项目分工
|学号 | 姓名  | 分工|
|---- |-------| -----|
|31701079 | 沈臻阳 | 网页端前端|
|31701068 | 曹隆翔 | 移动端前端|
|31701069 | 陈凯隆 | 后端开发|
|31701180 | 金旻儒 | 后端开发|

## 二、项目背景

在当代大学生的日常生活中，社团是必不可少的一个部分。在社团中你不仅可以参加各式各样的活动，也可以结交许多志同道合的朋友。每个学校都有数量众多的社团，有以兴趣为主题开设的社团，也有类似学生会之类的学生管理组织。如果仅仅是通过纸质文档进行管理的话，不但需要耗费大量的人力和资源，也会给管理造成不便。为了提升社团组织者对社团管理的便利性，我们小组选择社团管理这一主题，开发一款便于社团管理的系统。

## 三、系统简介
该系统是以便利社团管理者对社团的管理为目标的项目，该系统集社团管理、社团纳新、活动组织申报等功能于一体，为社团的管理者与学生提供了一个数字化管理平台。

## 四、项目需求

### 社长：

  1. 社长可填写活动申请（时间、场地、人数、经费），活动申请交由系统管理员（即学校方）进行审批，学校方审批通过即可举办活动发布公告（包括纳新），若申请未通过可对原有申请表进行修改，重新提交。社长也可对已提交但未审批的申请进行撤销操作。

  2. 社长可发布公告（时间、地点、人数、活动详情），公告可面向不同范围人群（全校学生、社员）进行发布，公告与活动存在关联。

  3. 社长可对社员进行职位任命，可审批社员提交的职位申请。

  4. 社长可对学生提交的社团加入申请进行审批。

  5. 社员向学校方提交换届申请，学校方对申请进行审批。

### 学生：

  1. 学生可以通过该系统浏览各个社团的信息（成立时间、社团星级、获得荣誉、社团管理层信息）。

  2. 学生可以选择感兴趣的社团，对其提交社团加入申请，等待社长审批，学生可加入多个社团。

  3. 学生可查看所有社团举办的面向全校的活动，并可以选择感兴趣的活动参加。

  4. 学生可以向系统管理员提交社团创建申请（需提供资质证明），等待管理员进行审批。

### 社员：（同时具有学生这个角色包含的需求）

  1. 社员可以查看社团发布的内部公告。

  2. 社员可以填写职务申请（财务管理、宣传部门、活动组织部门），交由社长进行审批操作。

  3. 不同职位的社员可以对社团内部不同的事务进行管理，职位由社长任免。

  4. 社员可免申请加入所在社团举办的活动。

  5. 社员可以提交退社申请，等待社长审批。

  6. 财务社员能查看社团经费内容。需审核社长提交的活动，并填写对应活动的经费表。

### 系统管理员（学校方）

  1. 系统管理员可审批社长提交的活动申请（时间、场地、人数、经费）。

  2. 系统管理员可对所有社团的信息进行管理修改（增删改）。

  3. 系统管理员可审批社团内部的人事变动（社长换届）。

  4. 系统管理员可对学生提交的建社申请进行审批。

  5. 系统管理员可以审核社团财务报表，并对此做出通知。

  6. 系统管理员可以发布对社团管理的公告，如社团财务申请表提交截至时间。

## 五、数据流图

![](https://raw.githubusercontent.com/schedule-front/EveryWeekRePort/master/week1/picture/datastream.png)

## 六、项目原型

[web端原型](https://free.modao.cc/app/6cd60f302a30c3d032772f10b80555602fc9fd0c/embed)

[app端原型](https://free.modao.cc/app/nblmz4zia8k2iw45l4dvmwtewjw2s/embed)


<embed src="https://free.modao.cc/app/nblmz4zia8k2iw45l4dvmwtewjw2s/embed" width="515" height="968" allowTransparency="true" frameborder="0"></embed>

## 七、项目技术

|模块|app|web|后端|
|-|-|-|-|
||webapp|vue|redis+springboot|

# 前后端接口定义模块


## 基本说明

1. 使用正则表达式检测

## User/Admin

### java类

```java
public class User implements Serializable {
    private String id;
    private String password;
    private String nickName;
    private String name;
    private String eMail;
    private String phone;
    private String type;
    //省略getter setter
}

```

### 表结构

| 名字 | java类型 | 格式(正则表达式) |说明|
| ---- | ---- | ---|-|
|uid|String| 317\d{5}||
|password|String|^(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,10}$|强密码(必须包含大小写字母和数字的组合，可以使用特殊字符，长度在8-10之间)：|
|name|String|||
|eMail|string|^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$|考虑通过邮件通知|
|phone|string| ^(13[0-9]\|14[5\|7]\|15[0\|1\|2\|3\|5\|6\|7\|8\|9]\|18[0\|1\|2\|3\|5\|6\|7\|8\|9])\d{8}$ |电话号码正则表达式（支持手机号码，3-4位区号，7-8位直播号码，1－4位分机号）|
|QQ|string|[1-9][0-9]{4,}|腾讯QQ号： 腾讯QQ号从10000开始)|

### 注册

#### 请求 

/user/register

####  JSON格式

| 名字 |说明 |
| ---- |-|
|uid|判断是否重复|
|password|加密传输|
|name||
|eMail||
|phone||
|QQ||
|CAPTCHA||

### 登陆

#### 请求 

/user/login

| 名字 |说明 |
| ---- |-|
|uid|判断是否存在|
|password|加密传输|
|CAPTCHA||

### 找回密码

| 名字 |说明 |
| ---- |-|
|uid|判断是否存在|
|eMail|提示部分,服务端校验是否一致,一致就向邮箱发送连接(待定)|


## Association

### java类

```java
public class Association implements Serializable {
    private String name;
    private Map<String,String> duitesId;
    private List<String> members;
    private List<String> announcements;
}
```

### 表结构

| 名字 | java类型 | 格式(正则表达式) |说明|
| ---- | ---- | ---|-|
|name|String| ||
|duitesId|Map<String,String>|||
|members|List<String>||存取成员id|
|announcements| List\<String\> |||

## Announcements

### java类

```java
public class Announcements implements Serializable {
    private String id;
    private String date;
    private String content;
    private String title;
    private List<String> announcements;
}
```

### 表结构

| 名字 | java类型 | 格式(正则表达式) |说明|
| ---- | ---- | ---|-|
|id|String| ||
|date|String|||
|content|String||内容|
|title|String|||




