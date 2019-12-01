## Activity

### java类

```java
@Document(collection="Activtity")
public class Activity {
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

    @Field
    private Integer numPeople;
    
    @Field
    private String location;
}
```