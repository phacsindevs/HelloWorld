# Hello World

##### 1.1 FIRST PROJECT SETUP

The first step is to create a simple Android Application using Android studio. When you click on Android studio icon, it will show screen as shown below

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld0.jpg?alt=media&token=0988e8ab-a85a-4ee9-9add-a21c64e53477)]()

You can start your application development by calling start a new android studio project. in a new installation frame should ask Application name, package information and location of the project

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld1.png?alt=media&token=a012f7e6-71d8-4458-8553-ff72ed4f9aa8)]()

After entered application name, it going to be called select the form factors your application runs on, here need to specify Minimum SDK, in our tutorial, We have declared as API15 - (IceCream Sandwich). Lower APIs will cover more devices but has limited functionality.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld2.png?alt=media&token=af63bd2d-7a11-423f-8fe4-97f7999e852d)]()

The next level of installation should contain selecting the activity to mobile, it specifies the default layout for Applications. You should choose Empty activity for this example.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld2.png?alt=media&token=af63bd2d-7a11-423f-8fe4-97f7999e852d)]()

The final step is to give the name of the Java class and the layout. For now we will be giving the default names provided.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld4.png?alt=media&token=d0eefb98-08bc-43c0-8a71-047bc05d1d92)]()

After these steps, the Android studio will look this.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld4.png?alt=media&token=d0eefb98-08bc-43c0-8a71-047bc05d1d92)]()


##### 1.2 ANDROID APP FILES

The MainActivity.java file will contain the following code

```sh
public class MainActivity extends AppCompatActivity {

      @Override 
     protected void onCreate(Bundle savedInstanceState) {
         super.onCreate(savedInstanceState);
         setContentView(R.layout.activity_main);
     }
 }


```
>Here, R.layout.activity_main refers to the activity_main.xml file located in the res/layout folder. The onCreate() method is one of many methods that are figured when an activity is loaded. The activty_main.xml inside res/layout folder should look this
```sh
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent" >

    <TextView
       android:layout_width="wrap_content"
       android:layout_height="wrap_content"
       android:layout_centerHorizontal="true"
       android:layout_centerVertical="true"
       android:padding="@dimen/padding_medium"
       android:text="@string/hello_world"
       tools:context=".MainActivity" />

  </RelativeLayout>
  ```
  ##### 1.3 RUNNING THE APP
  First go to developer options in your device and enable USB debugging. When you connect your phone to your computer it will show a pop-up as shown below.

 [![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld6.png?alt=media&token=dfcdcb30-56c6-4f0e-9485-0adb6e7a0cfd)]()

>By accepting this, you will be able to run your app on your device and debug your app in case something goes wrong. Now finally to run the app, press Shift + F10 (For Windows/Ubuntu) or Command + R (For Mac). Now you will see a pop-up with your device listed.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld7.png?alt=media&token=f580bf44-b8fc-4d3f-8964-7175cb625f24)]()

> After choosing your device, your app should run on your device with no errors. It should look something like this.

[![N|Solid](https://firebasestorage.googleapis.com/v0/b/phacsinedu.appspot.com/o/HelloWorld8.png?alt=media&token=227b506a-46a6-4236-aeac-f121ca6f966d)]()
