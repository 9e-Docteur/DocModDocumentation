# Creating your OS

First, create a package (optional) and call it computer
Then, inside the package, create another package (optional) and call it os, then create a class named "YourOSName".

Extend the class to the **BaseOS** Class

```java
public class MyOSName extends BaseOS {

}
```

You will need to create constructors and implements methods.

It should look like this:

```java
public class MyOSName extends BaseCommand{
    public MyOSName(String name, String arch, String shopPackageName){
        super(name, arch, shopPackageName);
    }

    @Override
    public void boot(){

    }

    @Override
    public void bootMessage(){

    }

    @Override
    public void commands(){
        
    }

}
```

I highly recommend remplacing **super(name, arch, shopPackageName)** to :
> super("yourOSName", "x64/ARM/UNIVERSAL", "yourOSNamePackageForTheShop");
