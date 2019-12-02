## Association

### java类

```java
public class Association implements Serializable {
    @Id
    private String _id;

    @Field
    private String associationId;

    @Field
    private String name;


    @Field
    private String presidentId;

    @Field
    private Map<String,String> duitesId; // userId -> duityId

    @Field
    private Set<String> members;

    @Field
    private Set<String> announcements;

    @Field
    public Set<String> accounts;

    @Field
    private String logoUrl;

    @Field
    private Date establishedTime;

    @Field
    private Map<String,Double> stars;
}
```

### 表结构

| 名字          | java类型           | 格式(正则表达式) | 说明       |
| ------------- | ------------------ | ---------------- | ---------- |
| name          | String             |                  |            |
| duitesId      | Map<String,String> |                  |            |
| members       | List<String>       |                  | 存取成员id |
| announcements | List\<String\>     |                  |            |
|accounts||||