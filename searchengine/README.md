# Ex.No:6 Build a program to create a first display screen of any search engine using Auto Complete Text View.

## AIM:

To develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as searchengine and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout using AutoComplete TextView in activity_main.xml.

Step 6: Display screen of search engine in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “display screen of any search engine”.
Developed by:
Registeration Number :
*/
```
### MainActivity.java

```
package com.example.exp6;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;

public class MainActivity extends AppCompatActivity {
    AutoCompleteTextView autocomplete;

    String[] arr = { "Bing","youtube","Google","Yandex","Yahoo","DuckDuckGo","Swisscows","StartPage","Gibiru"};

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        autocomplete = (AutoCompleteTextView)
                findViewById(R.id.autoCompleteTextView1);

        ArrayAdapter<String> adapter = new ArrayAdapter<String>
                (this,android.R.layout.select_dialog_item, arr);

        autocomplete.setThreshold(2);
        autocomplete.setAdapter(adapter);
    }
}
```
### activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/blue"
    android:padding="5dp"
    tools:context=".MainActivity">


    <AutoCompleteTextView
        android:id="@+id/autoCompleteTextView1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/textView2"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="30dp"
        android:layout_marginTop="30dp"
        android:layout_marginEnd="30dp"
        android:layout_marginBottom="30dp"
        android:ems="10"
        android:hint="Search Engine"
        android:textAlignment="center"
        tools:ignore="UnknownId" />

</RelativeLayout>
```
## OUTPUT

<img width="219" alt="red colour" src="https://user-images.githubusercontent.com/94505585/200015899-c1e3ae3c-d7af-41c8-8918-cd9ee45fec9e.png">

<img width="221" alt="duckduck" src="https://user-images.githubusercontent.com/94505585/200015928-16c002af-c09d-43e7-9d27-2e2d6965af19.png">

![Screenshot (20)](https://user-images.githubusercontent.com/94505585/200016025-baffe8c8-9989-4e64-bbc1-b8182837ddce.png)

![Screenshot (21)](https://user-images.githubusercontent.com/94505585/200016056-d551f339-f6d9-4fe1-b20e-a10c22ce3e21.png)


![Screenshot (22)](https://user-images.githubusercontent.com/94505585/200016133-b2574b9d-5fe3-40e1-8677-7a7d2f21fe65.png)


## RESULT
Thus a Simple Android Application develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio is developed and executed successfully.
