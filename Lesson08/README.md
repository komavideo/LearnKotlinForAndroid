类继承
======

## 知识点

* open关键字
* 构造器的使用

## 实战演习

~~~js
open class Car(brand: String) {
    var brand: String = brand;

    fun showBrand() {
        println("brand is ${brand}");
    }
}

class Lexus : Car("Lexus") {}

class Honda : Car("Honda") {}

fun main(args: Array<String>) {
    var car = Car("Toyota");
    var lexus = Lexus();
    var honda = Honda();

    car.showBrand();
    lexus.showBrand();
    honda.showBrand();
}
~~~

## 课程文件

https://github.com/komavideo/LearnKotlinForAndroid

## 小马视频频道

http://komavideo.com
