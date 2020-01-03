范围的使用
========

## 知识点

* ranges(for, if)

## 实战演习

~~~js
fun main(args: Array<String>) {
    // from i=1 to i<=5
    for (i in 1..5) {
        print("${i},");
    }  // 结果：1,2,3,4,5,
    println();

    // from i=1 to i<5
    for (i in 1 until 5) {
        print("${i},");
    } // 结果：1,2,3,4,
    println();

    for (i in 2..10 step 2) {
        print("${i},");
    } // 结果：2,4,6,8,10,
    println();

    for (i in 10 downTo 1) {
        print("${i},");
    } // 结果：10,9,8,7,6,5,4,3,2,1,
    println();

    var num = 5;
    //  num >=1 and num <= 10
    if (num in 1..10) {
        println("${num}在1到10之间");
    } // 结果：5在1到10之间
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
