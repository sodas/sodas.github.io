---
layout: post
category : Android
tagline: 
tags : 
---
{% include JB/setup %}

###fragment
一个fragment是一个activity的一部分，它有：
	-自己的生命周期
	-接受自己的输入事件
	-当activity在运行的时候可以被添加或者删除

**一个fragment必须总嵌入在一个activity中**

fragments 在 HoneyComb(3.0)之前不是API的一部分，在HoneyComb之前想使用fragments就需要**添加SupportPackage**到你的project里并且使用**FragmentActivity**来hold你的fragments。而在3.0之后则可以直接使用Activity来holdFragments。

###一些细节：

**3.0以后：**

use android.app.Fragment with Activity

调用getFragmentManager() 来得到 android.app.FragmentManager

调用getLoaderManager() 来得到 android.app.LoaderManager

**3.0以前：**

Use android.support.v4.app.Fragment withFragmentActivity

调用getSupportFragmentManager()来得到android.support.v4.app.FragmentManager

调用getSupportLoaderManager()来得到android.support.v4.app.LoaderManager


