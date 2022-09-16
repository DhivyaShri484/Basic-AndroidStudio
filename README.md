### Program:
Developed By: Dhivya Shri
Register Number: 212221230009
### MainActivity.java:

<c>
package com.example.project;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
</c>
<java>
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
</java>
### activity_main.xml:

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>

OUTPUT: 
![image](https://user-images.githubusercontent.com/94505585/190554889-a0a5dc4c-0c31-41f6-940d-4bfd4e2fe968.png)
![image](https://user-images.githubusercontent.com/94505585/190554935-92f7d7b2-e257-4908-8c76-6b4223c06c02.png)
![image](https://user-images.githubusercontent.com/94505585/190554984-d4b632eb-199a-43b9-a060-dba32df0ecae.png)
![image](https://user-images.githubusercontent.com/94505585/190555001-79b21e4c-3da8-474a-b3e8-3a27373c91b7.png)
![image](https://user-images.githubusercontent.com/94505585/190555046-0d3848e7-e7f7-4e31-8391-ce0fc673b780.png)
![image](https://user-images.githubusercontent.com/94505585/190555061-6c0a77a3-1836-45b9-abe8-43e7319a4fd5.png)
![image](https://user-images.githubusercontent.com/94505585/190555082-49cf88a5-4486-4b13-bf74-651916aae59a.png)

### Result:</br>
Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.




