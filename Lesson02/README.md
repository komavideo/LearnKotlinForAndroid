变量定义
=======

## 知识点

* 基本类型
* 定义方法

### 基本类型

* Byte:8位整数
* Short:16位整数
* Int:32位整数
* Long:64位整数
* Float:32位浮点数
* Double:64位浮点数
* String:字符串
* Char:字符类型
* Boolean:布尔值

## 实战演习

~~~js
fun main(args: Array<String>) {
    /**
     * 指定变量类型
     */
    //变量
    var name:String;
    name = "koma";

    println("helo ${name}.");

    //常量
    val age:Int = 10;
    //age = 20;

    println("age:${age}");

    /**
     * 推测变量类型
     */
    var title = "我的文章1";
    val point = 120;

    println("标题：${title}, 得分：${point}");
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
