代码：

文件：helloworld\app\src\main\java\com\example\helloworld\MainActivity.java

速览：

```java
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainMainActivityLife","调用onCreate()");
    }
    @Override
    protected void onStart() {
        super.onStart();
        Log.i("MainMainActivityLife","调用onStart()");
    }
    @Override
    protected void onResume() {
        super.onResume();
        Log.i("MainMainActivityLife","调用onResume()");
    }
    @Override
    protected void onPause() {
        super.onPause();
        Log.i("MainMainActivityLife","调用onPause()");
    }
    @Override
    protected void onStop() {
        super.onStop();
        Log.i("MainMainActivityLife","调用onStop()");
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.i("MainMainActivityLife","调用ononDestroy()");
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Log.i("MainMainActivityLife","调用onRestart()");
    }
}
```



初始启动：

![photo1](https://github.com/407470937/Android/blob/master/photos/test01/Androidtest101.PNG)

半遮掩到后台运行：

![photo1](https://github.com/407470937/Android/blob/master/photos/test01/Androidtest102.PNG)

重回屏幕：

![photo3](<https://github.com/407470937/Android/blob/master/photos/test01/Androidtest103%20.PNG>)

退出：

![photo4](<https://github.com/407470937/Android/blob/master/photos/test01/Androidtest104.PNG>)



线性布局：

代码：helloworld\app\src\main\res\layout\layouttest.xml

![](https://github.com/407470937/Android/blob/master/photos/test02/Androidtset201.PNG)

分析：采用了水平布局嵌套4个垂直布局的方法。

思考：另外也可以采用垂直布局嵌套4个水平布局的方法。



约束布局：

代码：helloworld\app\src\main\res\layout\activity_main2.xml

![](https://github.com/407470937/Android/blob/master/photos/test02/Androidtest202.PNG)

分析：采用了拖拽+text编码辅助的方法进行了实验。

思考：拖拽已能满足需求的话是否还需要编码进行辅助。答案是肯定的，个人感觉拖拽能满足大体上的布局，但在细微之处仍然需要代码的辅助。



表格布局:

代码:helloworld\app\src\main\res\layout\layout2.xml

<![](https://github.com/407470937/Android/blob/master/photos/test02/Androidtest203.PNG)

分析：采用了表格布局，每行一个表格，每个表格内分为3部分。

思考：怎样设置表格的layout_width。

