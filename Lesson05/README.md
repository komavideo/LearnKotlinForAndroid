循环逻辑
=======

## 知识点

* while
* do-while
* for

## 实战演习

~~~js
fun main(args: Array<String>) {

    // while
    var count = 5;
    while (count > 0) {
        println("1:${count}");
        count--;
    }

    // do-while
    count = 5;
    do {
        println("2:${count}");
        count--;
    } while (count > 0);

    // for-1
    var names = arrayOf("库里", "哈登", "阿詹");
    for (name in names)
        println("3:${name}");
    for (i in names.indices)
        println("4:${i}.${names[i]}");
    for ((index, name) in names.withIndex())
        println("5:${index}.${name}");

    // for-2
    for (i in 1..5) {
        println("X:${i}");
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
