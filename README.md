# jvmMaterial
java four reference: strong, soft, weak, phantom



#java Timer

<pre>
<code>
import java.util.{Timer, TimerTask}
object TimerTest {
  def main(args: Array[String]) {
    var count = 0
    val task: TimerTask = new TimerTask {
      def run {
        count = count + 1
        System.out.println("****************")
        System.out.println("Hi" + count)
      }
    }
    val timer: Timer = new Timer
    timer.schedule(task, 0, 2000)
  }

}
</code>
</pre>
