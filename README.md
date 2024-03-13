# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio
## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by:Bala Sathiesh CS 
Registeration Number :212222040022
*/
```
```
mainactivity.java
package com.example.bala;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart()
    {

        super.onRestart();
        Toast toast =Toast.makeText(getApplicationContext(),"onReStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart()
    {

        super.onStart();
        Toast toast =Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume()
    {

        super.onResume();
        Toast toast =Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause()
    {

        super.onPause();
        Toast toast =Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop()
    {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy()
    {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }

}
```
```
androidmanifest.xml
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
        android:theme="@style/Theme.Bala"
        tools:targetApi="31">
        <activity
            android:name=".MainActivity"
            android:exported="true">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## OUTPUT
![ONDestroy](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/d316d0e5-48c3-4bbe-855e-98a1cbe1cf4e)
![OnResume](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/2aabe914-5223-4ff9-8023-b1da0845b287)
![OnRestart](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/ba3432f9-264b-4d09-a16a-949ad5c78e99)
![OnPause](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/9b19740c-4d93-45d8-b257-39615f2b2fe5)
![OnStart](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/cb1cb137-ca3d-4a15-a6cd-df3f5fa76b2a)
![OnCreate](https://github.com/BalaSathiesh/lifecyclemethods/assets/128462891/94fa91fe-98c7-4588-869b-fe981a96b2d7)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
