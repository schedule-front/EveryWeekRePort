## Announcements

### java类

```java
@Document(collection="Announcements")
public class Announcement implements Serializable {
    @Id
    private String _id;

    @Field
    private String announcementId;

    @Field
    private String date;
    

    @Field
    private String title;

```


### 表结构

| 名字    | java类型 | 格式(正则表达式) | 说明 |
| ------- | -------- | ---------------- | ---- |
| id      | String   |                  |      |
| date    | String   |                  |      |
| content | String   |                  | 内容 |
| title   | String   |                  |      |
|||||