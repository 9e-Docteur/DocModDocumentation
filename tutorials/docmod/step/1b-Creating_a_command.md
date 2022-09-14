# Creating a command

First, create a package (optional) and call it computer
Then, inside the package, create a class named "YourCommandNameCommand".

Extend the class to the **BaseCommand** Class

```java
public class MyCommandNameCommand extends BaseCommand{

}
```

You will need to create constructors and implements methods.

It should look like this:

```java
public class MyCommandNameCommand extends BaseCommand{
    public MyCommandNameCommand(String name, String usage, CommandType type){
        super(name, usage, type);
    }

    @Override
    public void performCommand(String{args}){

    }

}
```

I highly recommend remplacing **super(name, usage, type)** to :
> super("yourCommandName/Prefux", "UsageOfYourCommand", CommandType.NORMAL);

## [2 CommandType](./2-CommandType.md)