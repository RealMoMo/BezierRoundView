# BezierRoundView

----
# Gif

 ![image](https://github.com/RealMoMo/BezierRoundView/blob/master/gif/show.gif)
 
----

#### Version
---
 - v1.0.2  ： 增加自定义属性点与点的距离。
 - v1.0.3  ： 解决颜色叠加问题。


<br/>

### xml布局代码
```
    <android.support.v4.view.ViewPager
        android:id="@+id/viewPager"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
     />

    <com.realmo.BezierRoundView
        android:id="@+id/bezRound"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
     />
```
<br/>

### Activity里面集成代码
```
ViewPager viewPager = (BezierViewPager) findViewById(R.id.viewPager);
viewPager.setAdapter(adapter);

BezierRoundView bezRound = (BezierRoundView) findViewById(R.id.bezRound);
bezRound.attach2ViewPage(viewPager);
```
<br/>
<br/>

### 方法及属性介绍

 - BezierRoundView

name               | format      |中文解释
----               |------       |----
color_select       | color    	 |当前选中圆球颜色
color_touch        | color   	 |触摸反馈颜色
color_not_select   | color	  	 |没有选中圆球的颜色
time_animator      | integer 	 |动画时间
round_count        | integer  	 |圆的数量，即Adapter.getCount
radius             | dimension	 |贝塞尔圆球半径，圆框半径为(radius-2)
distance		   | dimension	 |圆心与圆心的距离，默认是均分viewWidth/(count+1)
attach2ViewPage    |BezierViewPager|绑定指定的ViewPager(处理滑动时触摸事件)<br/>并自动设置round_count


---


###  Thanks
	Everyone who has contributed code and reported issues and pull requests!


## License

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	   http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.