## Account

### java类

``` java
@Document("Account")
public class Account {
    @Id
    private String _id;

    @Field
    private String activityId;

    @Field
    private String title;

    @Field
    private String content;

    @Field
    private Date date;

    @Field
    private String associationId;

}
```

