# Sample command

Here i'm gonna to create a command who'll answer "hello world!" when the command is executed.

So for now, our command class look like this:


```java
public class MyCommandNameCommand extends BaseCommand{
    public MyCommandNameCommand(String name, String usage, CommandType type){
        super("yourCommandName", "yourCommandUsage", CommandType.NORMAL);
    }

    @Override
    public void performCommand(String{args}){

    }

}
```

I have created a function who allow you to answer very easily.

> answer(component, AnswerType.NORMAL);

----
## Answer Type

Answer type describe if your command is:
> NORMAL: The answer will be send in white.
> FAILED: The answer will be send in red.
> INFO: The answer will be send in yellow.
> SUCCESS: The answer will be send in green.
---

So, in performCommand type:
answer(Component.literral("Hello world!"), AnswerType.SUCCESS);

so your class should look like this:

```java
public class MyCommandNameCommand extends BaseCommand{
    public MyCommandNameCommand(String name, String usage, CommandType type){
        super("yourCommandName", "yourCommandUsage", CommandType.NORMAL);
    }

    @Override
    public void performCommand(String{args}){
        answer(Component.literral("Hello world!"), AnswerType.SUCCESS);
    }

}
```