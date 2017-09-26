# Groovy Fundamentals

```
# groovy shell
groovysh
Groovy Shell (2.4.12, JVM: 1.8.0_144)
Type ':help' or ':h' for help.
-------------------------------------------------------------------------------------------------------------------
groovy:000> 3+5
===> 8
groovy:000> a+5
Unknown property: a
groovy:000> println "Hello World!"
Hello World!
===> null
groovy:000> println "Hello World!" + " Groovy".toUpperCase()
Hello World! GROOVY
===> null
groovy:000>

```

## Groovy compiler

```
groovyc Sample.groovy

```

It should generate the bytecode file, `Sample.class`.

```
javap Sample.class

javap Sample.class 
Compiled from "Sample.groovy"
public class Sample extends groovy.lang.Script {
  public static transient boolean __$stMC;
  public Sample();
  public Sample(groovy.lang.Binding);
  public static void main(java.lang.String...);
  public java.lang.Object run();
  protected groovy.lang.MetaClass $getStaticMetaClass();
}

```

Disassembles the java bytecodes.

```
groovy Sample.groovy
```

It will compile and run the groovy script.

