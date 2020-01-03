匿名类实现接口
=============

## 知识点

* 匿名类接口实现

## 实战演习

~~~js
interface IDatabase {
    fun connect(connString: String);
    fun close();
}

fun main(args: Array<String>) {
    var MockDB = object : IDatabase {
        override fun connect(connString: String) {
            println("匿名数据库连接...");
        }

        override fun close() {
            println("匿名数据库关闭");
        }
    }

    MockDB.connect("匿名连接串");
    MockDB.close();
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
