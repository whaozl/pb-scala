[![](https://jitpack.io/v/matfax/pb-scala.svg)](https://jitpack.io/#matfax/pb-scala)

# Terminal progress bar for Scala

Console progress bar for Scala Inspired from [pb](http://github.com/cheggaaa/pb).

![Screenshot](https://github.com/a8m/pb-scala/blob/master/gif/pb_rec.gif)

## Examples
1. simple example
```scala
object Main {
  def main(args: Array[String]) {
    var count = 1000
    var pb = new ProgressBar(count)
    // Default is true for all fields
    pb.showSpeed = false
    for (_ <- 1 to count) {
      pb.add(1)
      Thread.sleep(10)
    }
    println("done")
  }
}
```
