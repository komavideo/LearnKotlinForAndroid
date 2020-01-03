接口定义
=======

## 知识点

* interface关键字
* 接口的实现

## 实战演习

~~~js
interface IDatabase {
    fun connect();
    fun close();
}

abstract class Database(databaseName: String) : IDatabase {
    val databaseName: String = databaseName;

    var connString: String = "";

    fun showInfo() {
        println("数据库是:${databaseName}");
    }
}

class Oracle(connString: String) : Database("Oracle") {

    init {
        super.connString = connString;
    }

    override fun connect() {
        println("${databaseName}连接...(${connString})");
    }

    override fun close() {
        println("${databaseName}关闭");
    }
}

fun main(args: Array<String>) {
    var oracle = Oracle("Oracle数据库连接串");
    oracle.showInfo();
    oracle.connect();
    oracle.close();
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
