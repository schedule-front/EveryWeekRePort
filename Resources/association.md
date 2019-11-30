## Association

### java类

```java
public class Association implements Serializable {
    private String id;
    private String associationId;
    private String name;
    private Map<String,List<String>> duitesId;
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