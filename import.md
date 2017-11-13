```scala
object F{
  def add(a: Int, b: Int): Int ={
    return a + b
  }
}

object G{
  def main(args: Array[String]): Unit = {
    println(F.add(1, 20))
  }
}

object G{
  def main(args: Array[String]): Unit = {
    println(p())
  }
  def p(): Int = {
    F.add(1, 200)
  }
}
```
