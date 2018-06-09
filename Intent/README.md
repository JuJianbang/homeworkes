


![应用界面](https://github.com/llfjfz/AndroidTutorials/blob/master/IntentTutorials/screenshots/1.png)  


![选择界面](https://github.com/llfjfz/AndroidTutorials/blob/master/IntentTutorials/screenshots/2.png) 


![显示网页](https://github.com/llfjfz/AndroidTutorials/blob/master/IntentTutorials/screenshots/3.png) 


    String url = editUrl.getText().toString();
    Intent intent = new Intent();
    intent.setAction(Intent.ACTION_VIEW);
    intent.setData(Uri.parse(url));
    startActivity(intent);

 MyBrowser


    <intent-filter>
        <action android:name="android.intent.action.VIEW" />
        <category android:name="android.intent.category.DEFAULT" />
        <data android:scheme="http" />
    </intent-filter>

