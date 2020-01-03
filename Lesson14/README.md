with语法
========

## 知识点

* with

## 实战演习

~~~js
class Oracle {
    fun connect() {
        println("Oracle数据库连接...");
    }

    fun update() {
        println("Oracle数据库更新");
    }

    fun close() {
        println("Oracle数据库关闭");
    }
}

fun main(args: Array<String>) {
    val oracle = Oracle();
    with(oracle) {
        connect();
        update();
        close();
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
