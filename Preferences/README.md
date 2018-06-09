
  
![效果图1](https://github.com/llfjfz/AndroidTutorials/blob/master/PreferencesTutorial/screenshots/1.png)

ListPreference  

![ListPreference](https://github.com/llfjfz/AndroidTutorials/blob/master/PreferencesTutorial/screenshots/2.png)

onCreate中代码：

    FragmentManager mFragmentManager = getFragmentManager();
    FragmentTransaction mFragmentTransaction = mFragmentManager.beginTransaction();
    PrefsFragment mPrefsFragment = new PrefsFragment();
    mFragmentTransaction.replace(android.R.id.content, mPrefsFragment);
    mFragmentTransaction.commit();



Preference文件
    
    <CheckBoxPreference
    android:key="child_checkbox_preference"
    android:dependency="parent_checkbox_preference"
    android:layout="?android:attr/preferenceLayoutChild"
    android:title="@string/title_child_preference"
    android:summary="@string/summary_child_preference" />
