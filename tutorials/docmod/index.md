1. Create a folder called "Lib"
2. Place DocMod inside the folder.
3. Go to your build.gradle
4. Put in dependencies and inside type : 
> runtimeOnly fileTree(include: ['*.jar'], dir: 'libs')
4. Press the reload gradle button.
5. Now you are ready 😎

## [Next Step](./../docmod/index.md)