
# Ex.No:4 Design an android application Send SMS using Intent.


## AIM:

To create and design an android application Send SMS using Intent using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as “ex.no.4″ and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Send SMS and Display details give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to create and design an android application Send SMS using Intent.
Developed by: Dhivya Shri
Registeration Number : 212221230009
*/
```

### MainActivity.java
```
package com.sanath.smscontentprovider;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Button mbutton=(Button) findViewById(R.id.smsButton);
        mbutton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Intent intent =new Intent(Intent.ACTION_VIEW, Uri.fromParts("sms","9360247533",null));
                intent.putExtra("sms_body","SMS using Intent");
                startActivity(intent);
            }
        });
    }
}
```

### Activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/smsButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:backgroundTint="@color/design_default_color_secondary"
        android:text="send sms"
        android:layout_centerHorizontal="true"
        android:layout_centerVertical="true"/>

</RelativeLayout>
```

### AndroidManifest.xml
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools">

    <application
        android:allowBackup="true"
        android:dataExtractionRules="@xml/data_extraction_rules"
        android:fullBackupContent="@xml/backup_rules"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/Theme.SmscontentProvider"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>

            <meta-data
                android:name="android.app.lib_name"
                android:value="" />
        </activity>
    </application>

</manifest>
```

## OUTPUT

<img width="1440" alt="1" src="https://user-images.githubusercontent.com/94505585/199951553-343fa110-2708-4bc6-bed5-f83f8f94383b.png">

<img width="1440" alt="2" src="https://user-images.githubusercontent.com/94505585/199951595-d1645cb9-2dea-4c8d-9ebb-3404c12a9c44.png">

<img width="1440" alt="3" src="https://user-images.githubusercontent.com/94505585/199951652-ec22444e-bd5d-43a4-b796-fd0f23b4f97c.png">

<img width="331" alt="4" src="https://user-images.githubusercontent.com/94505585/199951700-dc0ee946-8f11-4fb4-ac3a-0142d3d32961.png">

<img width="331" alt="5" src="https://user-images.githubusercontent.com/94505585/199951726-b1125c9e-9496-4040-a9c6-5b4c44ba802e.png">

<img width="331" alt="6" src="https://user-images.githubusercontent.com/94505585/199951735-4a05f452-e50e-4eb8-846b-382125c6841c.png">



## RESULT
Thus a Simple Android Application create and design an android application Send SMS using Intent using Android Studio is developed and executed successfully.
