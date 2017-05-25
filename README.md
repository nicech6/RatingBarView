# RatingBarView
自定义RatingBar控件
### 1) In your root build.gradle:
allprojects {

    repositories {
        jcenter()
        maven { url 'https://jitpack.io' }
    }
}
### 2) In your library/build.gradle add:
<pre><code>
compile 'com.github.icuihai:RatingBarView:1.0'
</code></pre>
### 如何使用
        app:starImageSize="20dp" 星星大校小
        app:starPadding="20dp" //星星之间的间距
        app:starEmpty="@mipmap/ic_launcher" //没有选中的星星
        app:starFill="@mipmap/ic_launcher" //选中的星星
        * ratingBarView.setOnRatingChangeListener(new RatingBarView.OnRatingChangeListener() {
            @Override
            public void onRatingChange(float v) {
                选择后监听
            }
        });
        ratingBarView.setStar(2); //设置星
        
![image](https://github.com/icuihai/RatingBarView/raw/master/img/star.png)
