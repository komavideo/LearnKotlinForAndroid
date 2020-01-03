例外处理
=======

## 知识点

* try/catch/finally

## 实战演习

~~~js
fun main(args: Array<String>) {

    val value = "10";
    var out: Int? = null;

    // 错误处理
    try {
        out = Integer.parseInt(value);
    } catch (e: NumberFormatException) {
        println(">>>NumberFormatException<<<");
        println(e.message);
    } catch (e: Exception) {
        println("-->Exception<--");
        println(e.message);
    } finally {
        println("out is ${out}");
    }

    // 赋值处理
    var output = try {
        Integer.parseInt(value)
    } catch (e: Exception) {
        -1
    }
    println("output is ${output}");
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
