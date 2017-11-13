- 同一个程序中对象间调用
```scala
package udfs

object F{
  def add(a: Int, b: Int): Int ={
    return a + b
  }
}

class FF{
  def add(a: Int, b: Int): Int ={
    return a + b
  }
}

object G{
  def main(args: Array[String]): Unit = {
    println(F.add(1, 20))
  }
}

object GG{
  def main(args: Array[String]): Unit = {
    println(p())
  }
  def p(): Int = {
    F.add(1, 200)
  }
}
```
- 调包
```scala
import udfs.F
import udfs.FF

object ll {
  def main(args: Array[String]): Unit = {
    println(F.add(1, 1))
    println(new FF().add(1, 2))
  }
}
```
