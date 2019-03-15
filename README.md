# HelloWorld
This is a HelloWorld program...

## 实验内容：

Android实验一_Android开发基础，本代码创建了Android工程，并在工程中通过一系列的输出验证了Activity的生命周期。

## 关键代码：

通过覆写Activity生命周期中主要涉及的七种方法验证生命周期。

```
package com.example.helloworld;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainActivityLife","调用onCreate()");
    }

    @Override
    protected void onStart() {
        super.onStart();
        Log.i("MainActivityLife","调用onStart()");
    }

    @Override
    protected void onResume() {
        super.onResume();
        Log.i("MainActivityLife","调用onResume");
    }

    @Override
    protected void onPause() {
        super.onPause();
        Log.i("MainActivityLife","调用onPause");
    }

    @Override
    protected  void onStop() {
        super.onStop();
        Log.i("MainActivityLife","调用onStop");
    }

    @Override
    protected  void onDestroy() {
        super.onDestroy();
        Log.i("MainActivityLife","调用onDestroy");
    }

    @Override
    protected  void onRestart() {
        super.onRestart();
        Log.i("MainActivityLife","调用onRestart");
    }
}

```

## 实验结果：
### 1.运行HelloWorld<br>
![Image text](https://github.com/Apple-Jobs/img-folder/blob/master/HelloWorld.png)<br>
![Image text](https://github.com/Apple-Jobs/img-folder/blob/master/Activity1.png)<br>
### 2.返回桌面时的后台输出<br>
![Image text](https://github.com/Apple-Jobs/img-folder/blob/master/Activity2.png)<br>
### 3.再次返回HelloWorld<br>
![Image text](https://github.com/Apple-Jobs/img-folder/blob/master/Activity3.png)<br>
### 4.退出程序HelloWorld<br>
![Image text](https://github.com/Apple-Jobs/img-folder/blob/master/Activity4.png)<br>
