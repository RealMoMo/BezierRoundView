# BezierRoundView

���ڱ���Ŀ��Դ���������˾��ĿҪ�󿪷��µ�Launcher����Ȼ��ֻ��һС���֣�չʾӦ���б���Ϊ���û����鵽���ý�����ʽ��������Ŀ�����������¡��ڴ˸�л[������Ŀ](https://github.com/qdxxxx/BezierViewPager)��



# Gif

���·Ÿ�ʾ��ͼ����ұ����UI������ô��

 ![image](https://github.com/RealMoMo/BezierRoundView/blob/master/gif/show.gif)


## Version

 - v1.0.2  �� �����Զ������Ե����ľ��룬��������ʾ��
 - v1.0.3  �� �����ɫ�������⡣


<br/>

## xml���ִ���
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

## Activity���漯�ɴ���
```
ViewPager viewPager = (BezierViewPager) findViewById(R.id.viewPager);
viewPager.setAdapter(adapter);

BezierRoundView bezRound = (BezierRoundView) findViewById(R.id.bezRound);
bezRound.attach2ViewPage(viewPager);
```
<br/>
<br/>

## ���������Խ���

 - BezierRoundView

name               | format      |���Ľ���
----               |------       |----
color_select       | color    	 |��ǰѡ��Բ����ɫ
color_touch        | color   	 |����������ɫ
color_not_select   | color	  	 |û��ѡ��Բ�����ɫ
time_animator      | integer 	 |����ʱ��
round_count        | integer  	 |Բ����������Adapter.getCount
radius             | dimension	 |������Բ��뾶
distance		   | dimension	 |Բ����Բ�ĵľ��룬Ĭ���Ǿ���viewWidth/(count+1)
attach2ViewPage    |BezierViewPager|��ָ����ViewPager(������ʱ�����¼�)<br/>���Զ�����round_count





## Thanks
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