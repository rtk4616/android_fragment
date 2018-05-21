# /home/bootcode/bin/md/android_fragment

<!-- slide -->

# * [介紹 | W3School 菜鸟笔记 Android 基础入门教程](https://wizardforcel.gitbooks.io/w3school-android/content/)
<!-- slide -->

# * [ListView中Spinner的使用 - CSDN博客](https://blog.csdn.net/yangzl2008/article/details/7785401)
<!-- slide -->

# * [在Listview里面加入Spinner - CSDN博客](https://blog.csdn.net/z449077880/article/details/46430281)
<!-- slide -->

# * [在Listview里面加入Spinner - CSDN博客](https://blog.csdn.net/z449077880/article/details/46430281)



<!-- slide -->

# * [listView当中有嵌套了有onClickListener的控件时ListView自身的onItemClick无响应的解决方案 - CSDN博客](https://blog.csdn.net/yangzl2008/article/details/7761999)


<!-- slide -->

# * [ListView里面嵌套spinner和editext - CSDN博客](https://blog.csdn.net/qq_31552755/article/details/51801163)

<!-- slide -->

# * [ExpandableListAdapter Tutorial With Example In Android Studio](http://abhiandroid.com/ui/expandablelistadapter-example-android.html)

<!-- slide -->

# * [【Android學習】列表（ListView、RecyclerView)和adapter - 代碼家](http://www.dayexie.com/detail1772938.html)

<!-- slide -->

# * [Android Listview with spinner and radio button - Stack Overflow](https://stackoverflow.com/questions/32417388/android-listview-with-spinner-and-radio-button)


* [Android高手进阶教程(十五)---Android中万能的BaseAdapter(Spinner,ListView,GridView)的使用！ - 爱专集](http://www.aizhuanji.com/a/Xw7GkqZw.html)

* [Android高手进阶教程(十五)---Android中万能的BaseAdapter(Spinner,ListView,GridView)的使用！ - 爱专集](http://www.aizhuanji.com/a/Xw7GkqZw.html)

* [android listview 中button 冲突问题，不同情况不同解决方案 - 爱专集](http://www.aizhuanji.com/a/0VaKaRbx.html)

* [Android自定义适配器---实现简单文件管理器_Android自定义适配器 - 触屏版 - 阿里云](https://m.aliyun.com/jiaocheng/55239.html)

* [Android 初级躲不开的那些坑 - Android - 掘金](https://juejin.im/entry/596c16236fb9a06bbe7de339)

* [Android 精通自定义视图(2) - 简书](https://www.jianshu.com/p/092e126b623f)

* [Android UI ListView講解 - 代碼家](https://www.dayexie.com/detail649569.html)

* [Android初级躲不开的那些坑 | OCNYang](http://ocnyang.com/2016/08/31/AndroidGu/)



android:focusable=false
android:descendantFocussability=blocksDescendants
这是因为spinner把item容器的焦点抢走了，你要给最外层layout添加一个属性：

1
android:descendantFocusability="afterDescendants"
意思是让子视图获得焦点，然后才是layout自己

* [Android基础09-ListView - 简书](https://www.jianshu.com/p/c79741798fba)

* [Android基础入门教程——2.4.4 ListView的焦点问题 - 作业部落 Cmd Markdown
  编辑阅读器](https://www.zybuluo.com/coder-pig/note/178235)


* [ListVIew点击事件失效及descendantFocusability属性使用 - technical -
  ITeye博客](http://technicalsearch.iteye.com/blog/2033755)

* [ListView中Spinner的使用 -
  CSDN博客](https://blog.csdn.net/yangzl2008/article/details/7785401)

* [ good ][all android ] [健行科技Android手機程式設計人才培訓班 -
  實作範例二：要多背單字](http://www.aaronlife.com/v1/teaching/uch_android_2015-01-23_07.html)

* [ good ] [JackChan1999/Spinner:
  自定义组合控件之下拉选择框](https://github.com/JackChan1999/Spinner)

* [ListView
  小结](https://javaclee.com/android/2015/12/15/android-listview-summary.html)

* [layout調整間距 -
  程式天地](https://sites.google.com/site/chengshitiande/layout-diao-zheng-jian-ju)

* [客製 Spinner item layout (simple_spinner_dropdown_item) -
  程式天地](https://sites.google.com/site/chengshitiande/ke-zhi-spinner-item-layout)


* [Android中Spinner下拉列表（使用ArrayAdapter和自定义Adapter实现） -
  CSDN博客](https://blog.csdn.net/developer_jiangqq/article/details/7285623)

* [  ] [在安卓中，如何从所有其他 Spinners
  中删除所选项目_listview_帮酷编程问答](http://hant.ask.helplib.com/android/post_2003360)
android:layout_marginLeft="10dp"


*[gitbook] [TextView | Android
Traveling](https://chris930921.gitbooks.io/android-traveling-gitbook/xml/textview.html)

* [ good ][小鰻的Android學習筆記:
  ListView裡的OnItemClickListener失去作用(失效)](http://lp43.blogspot.tw/2012/09/listviewonitemclicklistener.html)

如上面紅色標註，
Android有提供一個快捷方式讓Layout裡的子元件全部失焦，
就是使用
android:descendantFocusability="blocksDescendants"。

註︰
1.當我在使用這個屬性時，
仍然無法讓OnItemClickListener發揮作用，
後來才發現我的TextView裡原本有設定一個屬性android:inputType="textMultiLine"
外國網友討論說這是一個Android的BUG，
此屬性一旦宣告，
又會讓上面紅色的宣告失去效果。
我把inputType="textMultiLine"拿掉，
整個問題才被解決。
2.最好用RelativeLayout的方式，使用僅一層Layout的架構客製這個list_item，
不僅在滑動有效率，也不會有這篇產生的問題。

￼
Ruei-Cheng Kao <rtk4616@gmail.com>
5月18日 (2 天前)￼
￼￼
寄給 Ruei-Cheng、 C6802￼
*[good] [ description ] [视图焦点问题 · wswenyue/note
Wiki](https://github.com/wswenyue/note/wiki/%E8%A7%86%E5%9B%BE%E7%84%A6%E7%82%B9%E9%97%AE%E9%A2%98)

* [spec] [ description] [ViewGroup  |  Android
  Developers](https://developer.android.com/reference/android/view/ViewGroup)

* [good] [ description] [Working with Input Views ·
  codepath/android_guides
Wiki](https://github.com/codepath/android_guides/wiki/Working-with-Input-Views)

* [titanium_mobile/TiListView.java at master ·
  appcelerator/titanium_mobile](https://github.com/appcelerator/titanium_mobile/blob/master/android/modules/ui/src/java/ti/modules/titanium/ui/widget/listview/TiListView.java)

* [good] [example] [Listview的OnItemClick无反应 -
  CSDN博客](https://blog.csdn.net/lihenair/article/details/49616627)

**spinner adapterview android:descendantFocusability requestFocus
beforeDescendants**

* [ASudoKube/LeaderboardActivity.java at master ·
  feiteira/ASudoKube](https://github.com/feiteira/ASudoKube/blob/master/ASudoKube/src/com/kapouta/asudokube/activities/LeaderboardActivity.java)

* [view] [attribute] [setter] [anvil/DSL.md at master ·
  zserge/anvil](https://github.com/zserge/anvil/blob/master/DSL.md)

*[good] [setContentView] [Android學習筆記---深入理解View#01 -
IT閱讀](http://www.itread01.com/articles/1476680421.html)

*[good] [setContentView] [View绘制详解(二)，从setContentView谈起 -
江南一点雨 - 博客园](http://www.cnblogs.com/lenve/p/5989997.html)

*[good] [picture]
[Android应用setContentView与LayoutInflater加载解析机制源码分析 -
CSDN博客](https://blog.csdn.net/yanbober/article/details/45970721)

*[good] [picture] [Android Activity 、 Window 、 View之间的关系 -
CSDN博客](https://blog.csdn.net/u011733020/article/details/49465707)

*[good] [picture]  [Android中View的相关知识（4） -
CSDN博客](https://blog.csdn.net/yyh448522331/article/details/72829511)

*[have to study ] [evnet] [view] [activity] [Android
Touch事件分发机制详解之由点击引发的战争 -
CSDN博客](https://blog.csdn.net/jiecsdn/article/details/70240882)

** requestFocus和clearFocus直接对View清除或转移焦点 **  * [Android
View焦点总结 – Android开发中文站](http://www.androidchina.net/6059.html)

** [good] [archetecture] *
[基于Android6.0的Activity加载View源码分析_Android_第七城市](http://www.th7.cn/Program/Android/201704/1155016.shtml)


** [good][picture] * [Android view绘制流程 -
CSDN博客](https://blog.csdn.net/coderinchina/article/details/78450495)


* [ScrollView源码分析 - 简书](https://www.jianshu.com/p/c3ed4253f87e)



* [good] [example] [luoyong/TvdVideo - Yeker Git
  Service](http://git.yekertech.com/luoyong/TvdVideo/src/master/src/com/softwinner/TvdVideo/MediaController.java)
￼


Ruei-Cheng Kao <rtk4616@gmail.com> 於 2018年5月18日 上午9:22 寫道：
android:focusable=false
android:descendantFocussability=blocksDescendants
这是因为spinner把item容器的焦点抢走了，你要给最外层layout添加一个属性：

1
android:descendantFocusability="afterDescendants"
意思是让子视图获得焦点，然后才是layout自己

* [Android基础09-ListView - 简书](https://www.jianshu.com/p/c79741798fba)

* [Android基础入门教程——2.4.4 ListView的焦点问题 - 作业部落 Cmd Markdown
  编辑阅读器](https://www.zybuluo.com/coder-pig/note/178235)


* [ListVIew点击事件失效及descendantFocusability属性使用 - technical -
  ITeye博客](http://technicalsearch.iteye.com/blog/2033755)

* [ListView中Spinner的使用 -
  CSDN博客](https://blog.csdn.net/yangzl2008/article/details/7785401)

* [ good ][all android ] [健行科技Android手機程式設計人才培訓班 -
  實作範例二：要多背單字](http://www.aaronlife.com/v1/teaching/uch_android_2015-01-23_07.html)

* [ good ] [JackChan1999/Spinner:
  自定义组合控件之下拉选择框](https://github.com/JackChan1999/Spinner)

* [ListView
  小结](https://javaclee.com/android/2015/12/15/android-listview-summary.html)

* [layout調整間距 -
  程式天地](https://sites.google.com/site/chengshitiande/layout-diao-zheng-jian-ju)

* [客製 Spinner item layout (simple_spinner_dropdown_item) -
  程式天地](https://sites.google.com/site/chengshitiande/ke-zhi-spinner-item-layout)


* [Android中Spinner下拉列表（使用ArrayAdapter和自定义Adapter实现） -
  CSDN博客](https://blog.csdn.net/developer_jiangqq/article/details/7285623)

* [  ] [在安卓中，如何从所有其他 Spinners
  中删除所选项目_listview_帮酷编程问答](http://hant.ask.helplib.com/android/post_2003360)
android:layout_marginLeft="10dp"


*[gitbook] [TextView | Android
Traveling](https://chris930921.gitbooks.io/android-traveling-gitbook/xml/textview.html)

* [ good ][小鰻的Android學習筆記:
  ListView裡的OnItemClickListener失去作用(失效)](http://lp43.blogspot.tw/2012/09/listviewonitemclicklistener.html)

如上面紅色標註，
Android有提供一個快捷方式讓Layout裡的子元件全部失焦，
就是使用
android:descendantFocusability="blocksDescendants"。

註︰
1.當我在使用這個屬性時，
仍然無法讓OnItemClickListener發揮作用，
後來才發現我的TextView裡原本有設定一個屬性android:inputType="textMultiLine"
外國網友討論說這是一個Android的BUG，
此屬性一旦宣告，
又會讓上面紅色的宣告失去效果。
我把inputType="textMultiLine"拿掉，
整個問題才被解決。
2.最好用RelativeLayout的方式，使用僅一層Layout的架構客製這個list_item，
不僅在滑動有效率，也不會有這篇產生的問題。


<!-- slide -->

# * [Android Development](http://tjach.pl/tresc/uploads/2014/11/sm_wyk14.pdf)
