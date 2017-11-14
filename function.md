## 形式
```scala
def functionName ([list of parameters]) : [return type] = {
   function body
   return [expr]
}
```

- 可变参数
```scala
object Demo {
   def main(args: Array[String]) {
      printStrings("Hello", "Scala", "Python");
   }

   def printStrings( args:String* ) = {
      var i : Int = 0;

      for( arg <- args ){
         println("Arg value[" + i + "] = " + arg );
         i = i + 1;
      }
   }
}
```
