# Android 复习资料汇总（每周持续更新中~）
接触 Android 开发也有一段时间了，前段时间便开始想抽空整理一些知识点，通过笔记整理的方式减少自己重复学习的时间成本和提高自身的效率。

整理的知识点会有Java、Android SDK、Android 源码、其他的一些计算机基础以及常见的面试题等几个部分，往后的一个月时间里会陆续补充更新。

目录：  
## Java 知识点汇总
  * [jvm](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#jvm)
     * [jvm工作流程](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#jvm工作流程)
     * [运行时数据区（Runtime Data Area）](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#运行时数据区runtime-data-area)
     * [方法指令](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#方法指令)
     * [类加载器](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#类加载器)
  * [Object](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#object)
     * [equals 方法](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#equals-%E6%96%B9%E6%B3%95)
     * [hashCode 方法](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#hashcode-%E6%96%B9%E6%B3%95)
  * [static](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#static)
  * [final](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#final)
  * [String、StringBuffer、StringBuilder](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#stringstringbufferstringbuilder)
  * [异常处理](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#异常处理)
  * [内部类](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#内部类)
  * [多态](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#多态)
  * [抽象和接口](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#抽象和接口)
  * [集合](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#集合)
  * [反射](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#反射)
  * [单例](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#单例)
     * [饿汉式](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#饿汉式)
     * [双重检查模式](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#双重检查模式)
     * [静态内部类模式](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#静态内部类模式)
  * [线程](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#线程)
  * [valatile](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#valatile)
  * [HashMap](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#hashmap)
     * [HashMap的工作原理](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#hashmap的工作原理)
  * [synchronized](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#synchronized)
     * [根据获取的锁分类](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#根据获取的锁分类)
     * [原理](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#原理)
  * [Lock](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#lock)
     * [悲观锁、乐观锁](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#悲观锁乐观锁)
     * [自旋锁、适应性自旋锁](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#自旋锁适应性自旋锁)
     * [死锁](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#死锁)
  * [引用类型](https://github.com/JasonWu1111/Android-Review/blob/master/Java%20知识点汇总.md#引用类型)

&nbsp;
## Android 知识点汇总
   * [Dalvik 和 ART](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#dalvik-和-art)
   * [Activity](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#activity)
      * [生命周期](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#生命周期)
      * [启动模式](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#启动模式)
      * [启动过程](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#启动过程)
   * [Fragment](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#fragment)
      * [特点](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#特点)
      * [生命周期](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#生命周期-1)
      * [与Activity通信](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#与activity通信)
   * [Service](#service)
      * [生命周期：](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#生命周期-2)
      * [启用前台服务：](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#启用前台服务)
   * [BroadcastReceiver](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#broadcastreceiver)
   * [ContentProvider](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#contentprovider)
   * [数据存储](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#数据存储)
   * [View](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#view)
      * [MeasureSpec](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#measurespec)
      * [MotionEvent](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#motionevent)
      * [VelocityTracker](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#velocitytracker)
      * [GestureDetector](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#gesturedetector)
      * [Scroller](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#scroller)
      * [View的滑动](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#view的滑动)
      * [View的事件分发](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#view的事件分发)
      * [在Activity中获取某个View的宽高](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#在activity中获取某个view的宽高)
      * [Draw的基本流程](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#draw的基本流程)
      * [自定义View](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#自定义view)
   * [进程](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#进程)
      * [进程生命周期](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#进程生命周期)
      * [多进程](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#多进程)
      * [进程存活](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#进程存活)
         * [OOM_ADJ](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#oom_adj)
         * [进程被杀情况](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#进程被杀情况)
         * [进程保活方案](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#进程保活方案)
   * [IPC](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#ipc)
      * [IPC方式](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#ipc方式)
      * [AIDL](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#aidl)
      * [Messenger](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#messenger)
   * [Bitmap](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#bitmap)
      * [配置信息与压缩方式](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#配置信息与压缩方式)
      * [常用操作](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#常用操作)
         * [裁剪、缩放、旋转、移动](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#裁剪缩放旋转移动)
         * [Bitmap与Drawable转换](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#bitmap与drawable转换)
         * [保存与释放](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#保存与释放)
         * [图片压缩](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#图片压缩)
      * [BitmapFactory](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#bitmapfactory)
         * [Bitmap创建流程](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#bitmap创建流程)
         * [Option类](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#option类)
         * [基本使用](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#基本使用)
      * [内存回收](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#内存回收)
   * [Serializable/Parcelable](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#serializableparcelable)
   * [屏幕适配](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#屏幕适配)
      * [单位](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#单位)
      * [头条适配方案](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#头条适配方案)
   * [Context](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#context)
   * [SharedPreferences](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#sharedpreferences)
      * [获取方式](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#获取方式)
         * [getPreferences](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#getpreferences)
         * [getDefaultSharedPreferences](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#getdefaultsharedpreferences)
         * [getSharedPreferences](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#getsharedpreferences)
      * [架构](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#架构)
      * [apply / commit](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#apply--commit)
      * [注意](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#注意)
   * [NDK](#ndk)
      * [用途](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#用途)
   * [消息机制](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#消息机制)
      * [Handler机制](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#handler机制)
      * [工作原理](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#工作原理)
         * [ThreadLocal](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#threadlocal)
         * [MessageQueue](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#messagequeue)
         * [Looper](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#looper)
         * [Handler](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#handler)
   * [线程异步](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#线程异步)
      * [AsyncTask](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#asynctask)
         * [基本使用](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#基本使用-1)
         * [工作原理](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#工作原理-1)
      * [HandlerThread](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#handlerthread)
      * [IntentService](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#intentservice)
      * [线程池](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#线程池)
   * [Recyclerview 优化](https://github.com/JasonWu1111/Android-Review/blob/master/Android%20%E7%9F%A5%E8%AF%86%E7%82%B9%E6%B1%87%E6%80%BB.md#recyclerview-%E4%BC%98%E5%8C%96)
      
&nbsp;
## 常见面试算法题汇总
   * [排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#排序)
      * [比较排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#比较排序)
         * [冒泡排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#冒泡排序)
         * [归并排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#归并排序)
         * [快速排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#快速排序)
      * [线性排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#线性排序)
         * [计数排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#计数排序)
         * [桶排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#桶排序)
   * [二叉树](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#二叉树)
      * [顺序遍历](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#顺序遍历)
      * [层次遍历](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#层次遍历)
      * [左右翻转](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#左右翻转)
      * [最大值](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最大值)
      * [最大深度](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最大深度)
      * [最小深度](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最小深度)
      * [平衡二叉树](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#平衡二叉树)
   * [链表](#链表)
      * [删除节点](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#删除节点)
      * [翻转链表](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#翻转链表)
      * [中间元素](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#中间元素)
      * [判断是否为循环链表](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#判断是否为循环链表)
      * [合并两个已排序链表](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#合并两个已排序链表)
      * [链表排序](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#链表排序)
      * [删除倒数第N个节点](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#删除倒数第n个节点)
      * [两个链表是否相交](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#两个链表是否相交)
   * [栈 / 队列](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#栈--队列)
      * [带最小值操作的栈](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#带最小值操作的栈)
      * [有效括号](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#有效括号)
      * [用栈实现队列](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#用栈实现队列)
      * [逆波兰表达式求值](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#逆波兰表达式求值)
   * [二分](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#二分)
      * [二分搜索](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#二分搜索)
      * [X的平方根](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#x的平方根)
   * [哈希表](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#哈希表)
      * [两数之和](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#两数之和)
      * [连续数组](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#连续数组)
      * [最长无重复字符的子串](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最长无重复字符的子串)
      * [最多点在一条直线上](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最多点在一条直线上)
   * [堆 / 优先队列](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#堆--优先队列)
      * [前K大的数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#前k大的数)
      * [前K大的数II](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#前k大的数ii)
      * [第K大的数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#第k大的数)
   * [二叉搜索树](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#二叉搜索树)
      * [验证二叉搜索树](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#验证二叉搜索树)
      * [第K小的元素](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#第k小的元素)
   * [数组 / 双指针](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#数组--双指针)
      * [加一](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#加一)
      * [删除元素](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#删除元素)
      * [删除排序数组中的重复数字](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#删除排序数组中的重复数字)
      * [我的日程安排表 I](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#我的日程安排表-i)
      * [合并排序数组](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#合并排序数组)
   * [贪心](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#贪心)
      * [买卖股票的最佳时机](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#买卖股票的最佳时机)
      * [买卖股票的最佳时机 II](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#买卖股票的最佳时机-ii)
      * [最大子数组](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最大子数组)
      * [主元素](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#主元素)
   * [字符串处理](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#字符串处理)
      * [生成括号](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#生成括号)
      * [Excel表列标题](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#excel表列标题)
      * [翻转游戏](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#翻转游戏)
      * [翻转字符串中的单词](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#翻转字符串中的单词)
      * [转换字符串到整数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#转换字符串到整数)
      * [最长公共前缀](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#最长公共前缀)
      * [回文数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#回文数)
   * [动态规划](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#动态规划)
      * [单词拆分](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#单词拆分)
      * [爬楼梯](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#爬楼梯)
      * [打劫房屋](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#打劫房屋)
      * [编辑距离](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#编辑距离)
      * [乘积最大子序列](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#乘积最大子序列)
   * [矩阵](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#矩阵)
      * [螺旋矩阵](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#螺旋矩阵)
      * [判断数独是否合法](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#判断数独是否合法)
      * [旋转图像](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#旋转图像)
   * [二进制 / 位运算](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#二进制--位运算)
      * [落单的数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#落单的数)
      * [格雷编码](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#格雷编码)
   * [其他](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#其他)
      * [反转整数](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#反转整数)
      * [LRU缓存策略](https://github.com/JasonWu1111/Android-Review/blob/master/%E5%B8%B8%E8%A7%81%E9%9D%A2%E8%AF%95%E7%AE%97%E6%B3%95%E9%A2%98%E6%B1%87%E6%80%BB.md#lru缓存策略) 
