# CustomFontView
<img src="https://camo.githubusercontent.com/7a097bb07d47506d643804b222bb8ad2be336498/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4150492d392532422d6f72616e67652e7376673f7374796c653d666c6174" alt="API" data-canonical-src="https://img.shields.io/badge/API-9%2B-orange.svg?style=flat" style="max-width:100%;">

Custom font classes for TextView, EditText &amp; Buttons

![screenshot_20170816-153601](https://user-images.githubusercontent.com/22608780/29374593-9d9f71d4-82cf-11e7-915d-dcead8093d40.png)

<h2>How to integrate the library in your app?</h2>
<b>Gradle Dependecy</b></br>

```gradle
dependencies {
        compile 'com.an.customfontview:customfont:0.1.0'
}
```

<b>Maven Dependecy</b></br>
```xml
<dependency>
  <groupId>com.an.customfontview</groupId>
  <artifactId>customfont</artifactId>
  <version>0.1.0</version>
  <type>pom</type>
</dependency>
```

<h2>Add fonts</h2>

Add your custom fonts to ```assets/``` .</br>
If the assets directory does not already exist, you should create it under ```src/main/``` in your project directory.</br>
You might consider creating a ```fonts/``` subdirectory in the assets directory (as in examples).

<h2>Usage</h2>

Add the below line to the root layout of your xml file:

```xml
xmlns:app="http://schemas.android.com/apk/res-auto"
```

<h3>Custom TextView</h3>

```xml
.....
       <com.an.customfontview.CustomTextView
          android:layout_gravity="center"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          app:textFontPath="fonts/gotham_bold.otf"
          android:text="Works for any number of fonts" />
.....
``` 

<h3>Custom EditText</h3>

```xml
.....
       <com.an.customfontview.CustomEditText
          android:text="Works for edit text too!"
          android:layout_width="match_parent"
          android:layout_height="wrap_content"
          app:editFontPath="fonts/product_sans.ttf" />
.....
``` 

<h3>Custom Buttons</h3>

```xml
.....
           <com.an.customfontview.CustomButton
              android:layout_gravity="center"
              android:layout_width="wrap_content"
              android:layout_height="wrap_content"
              app:btnFontPath="fonts/gt_medium.otf"
              android:text="Works for me too!"/>
.....
``` 

That's all folks!
