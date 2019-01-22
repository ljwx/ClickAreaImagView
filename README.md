# ClickAreaImagView

针对一张图,指定点击区域才能响应
我们app很多地方点击都是没有效果的,所以有时候就是一张大图,ios好像有点击区域,他们总是说让切一张大图就好了,安卓就只能分开切
这个控件也是希望做到他们一眼的效果
##### 支持预览区域,可控制是否显示
![avatar](https://github.com/ljwx/Image/blob/master/ClickAreaImageView.png)
```xml
<com.ljwx.view.ClickAreaImageView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:src="@mipmap/game_stone2"
        app:tag1_bottom="80dp"
        app:tag1_left="20dp"
        app:tag1_right="80dp"
        app:tag1_top="20dp"
        app:drawArea="true"/>
```
##### 设置点击
```java
ClickAreaImageView view = findViewById(R.id.img);
        view.setOnClickListenerTag1(new ClickAreaImageView.TouchAreaListener() {
            @Override
            public void call() {
                Toast.makeText(MainActivity.this, "tag1", Toast.LENGTH_SHORT).show();
            }
        });
 ```
