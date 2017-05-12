---
layout: post
title: "Making button for Android App"
modified:
categories: blog
excerpt:
tags: []
image:
  feature:
date: 2017-05-12T11:13:51Z
---

Want to design custom buttons for you android App?

After adding your button to the layout, add the background variable too```android:background="@drawable/clickbuttonshape"```
It should look some what like below

```xml
       <Button
            android:id="@+id/button"
            android:layout_width="80dp"
            android:layout_height="80dp"
            android:layout_gravity="center"
            android:background="@drawable/clickbuttonshapemenu"
            android:layout_alignParentBottom="true"
            android:layout_centerHorizontal="true"
            android:layout_marginBottom="11dp" />
```

Create a file in drawable named ```clickbuttonshapemenu```


```xml
<?xml version="1.0" encoding="utf-8"?>
<selector xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:state_pressed="true"
        android:drawable="@drawable/clickbuttonshapeoff"></item>

<item android:drawable="@drawable/clickbuttonshapeon">
    </item>

</selector>
```
This is where we can create different buttons for normal and pressed state, the code above is self explanatory. Create two files in drawables 
```clickbuttonshapeoff``` . 

```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle" >
    <corners
        android:radius="100dp"
        />
    <solid
        android:color="#881152d2"
        />
    <padding
        android:left="0dp"
        android:top="0dp"
        android:right="0dp"
        android:bottom="0dp"
        />
    <size
        android:width="70dp"
        android:height="70dp"
        />
    <stroke
        android:width="6dp"
        android:color="#55383333"
        />


</shape>

```

```clickbuttonshapeon``` .

```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle" >
    <corners
        android:radius="70dp"
        />
    <solid
        android:color="#774c6399"
        />
    <padding
        android:left="0dp"
        android:top="0dp"
        android:right="0dp"
        android:bottom="0dp"
        />
    <size
        android:width="70dp"
        android:height="70dp"
        />
    <stroke
        android:width="10dp"
        android:color="#55383333"
        />


</shape>

```
By changing the parameters like the radius, color, size and the stroke width, various designs can be made. The current  one makes a circular button.