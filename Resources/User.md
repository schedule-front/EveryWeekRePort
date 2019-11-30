## User/Admin

### java类

```java
@Document(collection="User")
public class User implements Serializable {
    final public static String collectionName = "User";
    @Id
    String _id;

    @Field
    private String userId;

    @Field
    private String password;

    @Field(value = "class")
    private String clasS;
    @Field
    private String major;
    @Field
    private String name;

    @Field
    private String eMail;

    @Field
    private String phone;

    @Field
    private String role;

    @Field
    public List<String> announcements;

    @Field
    public List<String> associations;
}

```

### 表结构

表名: User


| 名字     | java类型 | 格式(正则表达式)                                                                         | 说明                                      |
| -------- | -------- | ---------------------------------------------------------------------------------------- |-------------------------------------------------------------------------- |
|_id|||||
| userId      | String   | 317\d{5}                                                                                 |                                                                            |
| password | String   | ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,10}$                                                  | 强密码(必须包含大小写字母和数字的组合，可以使用特殊字符，长度在8-10之间)： |
| name     | String   |                                                                                          |                                                                            |
| eMail    | string   | ^\w+([-+.]\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$                                            | 考虑通过邮件通知                                                           |
| phone    | string   | ^(13[0-9]\|14[5\|7]\|15[0\|1\|2\|3\|5\|6\|7\|8\|9]\|18[0\|1\|2\|3\|5\|6\|7\|8\|9])\d{8}$ | 电话号码正则表达式（支持手机号码，3-4位区号，7-8位直播号码，1－4位分机号） |
| QQ       | string   | [1-9][0-9]{4,}                                                                           | 腾讯QQ号： 腾讯QQ号从10000开始)                                            |
|userClass||||||
|major||||
|announcements||
|associations|||||

### 注册

#### 请求 

/user/register

####  JSON格式

| 名字     | 说明         |
| -------- | ------------ |
| uid      | 判断是否重复 |
| password | 加密传输     |
| name     |              |
| eMail    |              |
| phone    |              |
| QQ       |              |
| CAPTCHA  |              |

### 登陆

#### 请求 

/user/login

| 名字     | 说明         |
| -------- | ------------ |
| uid      | 判断是否存在 |
| password | 加密传输     |
| CAPTCHA  |              |

### 找回密码

| 名字  | 说明                                                   |
| ----- | ------------------------------------------------------ |
| uid   | 判断是否存在                                           |
| eMail | 提示部分,服务端校验是否一致,一致就向邮箱发送连接(待定) |

