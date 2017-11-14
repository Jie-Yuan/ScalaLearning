<h1 align = "center">:rocket: 面向对象 :facepunch:</h1>

---

## this: __init__

```scala
class ThisExample{  
    var id:Int = 0  
    var name: String = ""  
    def this(id:Int, name:String){  
        this()  
        this.id = id  
        this.name = name  
    }  
    def show(){  
        println(id+" "+name)  
    }  
}  

object Demo{  
    def main(args:Array[String]){  
        var t = new ThisExample(1010,"Maxsu")  
        t.show()  
    }  
}
```

```scala
class ThisExample(id:Int, name: String){  
    def show(){  
        println(id+" "+name)  
    }  
}  
```
