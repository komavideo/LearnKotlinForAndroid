Null空安全
=========

## 知识点

* null
* null允许符号:?
* 跳过编译时null检测:!!

## 实战演习

~~~js
fun main(args: Array<String>) {

    // 编译报错(null安全特性)
    var name: String;
    //name = null;

    // null值允许
    var title: String?;
    title = "我的文章1";
    if (title != null)
        println("${title}");

    var length = title.length;
    println("length is ${length}");

    // null设定
    title = null;
    // (编译时错误)
    //length = title.length;

    // !!跳过编译null检测(运行时错误)
    length = title!!.length;
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
