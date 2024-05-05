# ADDITION-OF-TWO-NUMBERS
# AIM:
To develop a program to perform addition of two numbers using Android Studio.

# EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)
# ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as SMSIntent and click Next.

Step 3: Select the Minimum SDK below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally, click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Perform the Calculator Operation in MainActivity.java

Step 7: Save and run the application.

# Program:
```
/*
Program to create simple calculator using Android Studio.
Developed by:NITHYAA SRI S S
RegisterNumber: 212222230100
*/
```
# MainActivity.java:
```
package com.example.addition_of_two_numbers;

import androidx.appcompat.app.AppCompatActivity;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;
import android.widget.Toast;
import android.os.Bundle;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private EditText txtFirstNo;
    private EditText txtSecondNo;
    private TextView txtResult;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        txtFirstNo=(EditText) findViewById(R.id.txtFirstNo);
        txtSecondNo=(EditText) findViewById(R.id.txtSecondNo);
        txtResult=(TextView) findViewById(R.id.txtResult);
    }

    public void Calculate(View v){

        Float first= Float.parseFloat( txtFirstNo.getText().toString()) ;
        Float second= Float.parseFloat( txtSecondNo.getText().toString()) ;
        Float result=first+second;
        txtResult.setText(result.toString());

    }

}
# activity_main.xml:

```<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="50dp"
        android:textSize="20dp"
        android:text="Enter the First Number:"
        />
    <EditText
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="25dp"
        android:ems="10"
        android:id="@+id/txtFirstNo"
        />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="50dp"
        android:textSize="20dp"
        android:text="Enter the Second Number:"
        />
    <EditText
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="25dp"
        android:ems="10"
        android:id="@+id/txtSecondNo"
        />
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/btnAdd"
        android:text="Add"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="25dp"
        android:onClick="Calculate"
        />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/txtResult"
        android:layout_gravity="center_horizontal"
        android:gravity="center_horizontal"
        android:layout_marginTop="50dp"
        android:textSize="20dp"
        />
</LinearLayout>
```
# AndroidMainfest.xml
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
        android:theme="@style/Theme.ADDITIONOFTWONUMBERS"
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
# OUTPUT:
![WhatsApp Image 2024-05-05 at 15 00 41_63a32c38](https://github.com/ssnithyaasri/ADDITION-OF-TWO-NUMBERS/assets/119122478/f920ad87-363c-4f88-9f06-80592ed129e8)

# Result:
Thus a Simple Android Application to perform addition of two numbers using Android Studio was developed and executed successfully.
