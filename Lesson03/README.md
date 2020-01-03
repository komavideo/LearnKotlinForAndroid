条件分支
=======

## 知识点

* if/else
* if/else赋值
* is

## 实战演习

~~~js
fun main(args: Array<String>) {
    // if/else
    var APILevel = 26;
    if (APILevel >= 16){
        println("Android 4.1以上，是我支持的版本。");
    }else{
        println("我们已经不支持该版本的Andoid系统。");
    }

    // if/else赋值
    // (condition) ? value1 : value2
    var isSupport = if (APILevel >= 16) true else false;
    println("isSupport:${isSupport}");

    // is判断类型
    if (APILevel is Int){
        println("APILevel是整形");
    }else{
        println(APILevel.javaClass.toString());
    }

    var content = "超级马里奥";
    if (content is String)
        println("content是字符串类型");
    if (isSupport is Boolean)
        println("isSupport是布尔类型");
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
