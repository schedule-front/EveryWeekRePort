# java类

```java
@Document("Award")
public class Award {
    @Id
    private String _id;
    @Field
    private String awardId;
    @Field
    private String title;
    @Field
    private String content;
    @Field
    private String url;
}
```