类定义
======

## 知识点

* 面向对象的编程
* 类定义class

## 实战演习

~~~js
class Player {
    var name: String = "";

    constructor(fullname: String) {
        this.name = fullname;
    }

    fun sayHelo() {
        println("helo ${name}");
    }

    fun getAge(): Int {
        return 20;
    }
}

class Match(val home: String, val away: String, val date: String) {
    fun getMatchInfo(): String {
        return "${away} vs ${home} @ ${date}"
    }
}

fun main(args: Array<String>) {

    val player = Player("koma");
    player.sayHelo();
    println("${player.name} is ${player.getAge()}");

    val match = Match("勇士", "骑士", "2018/1/1");
    println(match.getMatchInfo());
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
