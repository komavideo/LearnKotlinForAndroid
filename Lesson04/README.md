多重分支
=======

## 知识点

* when
* is

## 实战演习

~~~js
fun main(args: Array<String>) {

    // Android API Level
    var APILevel = 26;

    // when
    when (APILevel) {
        26, 27 -> {
            println("Android Oreo");
        }
        24, 25 -> println("Android Nougat");
        23 -> {
            println("Android Marshmallow");
        }
        else -> {
            println("Android 5以下");
        }
    }

    // when赋值
    var content = when (APILevel) {
        26, 27 -> "Android Oreo"
        24, 25 -> "Android Nougat"
        23 -> "Android Marshmallow"
        else -> "Android 5以下"
    }
    println("content is ${content}");

    // when is判断
    var obj = null;
    when (obj) {
        is Int -> println("obj是整数类型");
        is String -> println("obj是字符串类型");
        is Boolean -> println("obj是布尔类型");
        else -> println("未知类型");
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
