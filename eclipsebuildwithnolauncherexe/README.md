# reproducers/tycho eclipse product build without launcher.exe
## This demonstrates how to  build an eclipse product with or without the launcher.exe created. eclipse.exe is only needed to launch the IDE

``` mvn clean install ```

# result as for now:
## The created eclipse product out of the tycho maven is in here going to be without launcher.exe by default. You first will get this exe file if you configure for example a name for it in the .product file
``` 
<launcher name="demo">..</launcher>
```

## Alternative would be to remove it via instructing tycho using p2.inf touchpoint as in this stackoverflow post
https://stackoverflow.com/questions/11829809/maven-tycho-how-to-exclude-eclipsec-exe-in-a-product-build


