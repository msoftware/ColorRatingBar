# ColorRatingBar

## Introduction
Change Star Color of Rating Bar(min SDK: 14)


#### * An example project / library of ColorRatingBar

![](assets/ColorRatingBar.gif)

## Usages

Add your buildscript
#### • maven
```xml
<dependency>
  <groupId>hyogeun.github.com.colorratingbar</groupId>
  <artifactId>ColorRatingBar</artifactId>
  <version>1.0.0</version>
  <type>pom</type>
</dependency>
```
#### • gradle
```groovy
compile 'hyogeun.github.com.colorratingbar:ColorRatingBar:1.0.0'
```


### Example
#### 1. xml
```xml
<hyogeun.github.com.colorratingbarlib.ColorRatingBar
        android:id="@+id/rating_1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:rating="3"
        app:empty_color="#f0f000"
        app:progress_color="#00f0f0" />
```

#### 2. Code
  ##### 1) Activity
  ```java
  ColorRatingBar colorRatingBar = new ColorRatingBar(this);
  colorRatingBar.setRatingProgressColor(R.color.colorPrimary);
  colorRatingBar.setRatingEmptyColor(R.color.colorAccent);
  colorRatingBar.setRating(3.0f);
  ```
  ##### 2) Fragment
  ```java
  ColorRatingBar colorRatingBar = new ColorRatingBar(getContext());
  colorRatingBar.setRatingProgressColor(R.color.colorPrimary);
  colorRatingBar.setRatingEmptyColor(R.color.colorAccent);
  colorRatingBar.setRating(3.0f);
  ```

## LICENSE
```
Copyright (c) 2017 hyogeun.park

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
