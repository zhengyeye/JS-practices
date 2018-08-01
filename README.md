# JS-practices
### Day1.创建对象的四种方式：
原型关系图
![原型关系图](https://github.com/zhengyeye/JS-practices/blob/master/images/%E5%AF%B9%E8%B1%A1.png)

解释：创建Person构造函数后，其默认拥有prototype属性，指向的是Person的原型；
而Person的原型默认拥有constructor属性，该属性指向Person的构造函数
Person原型中的其他属性，比如name，age，是在Person原型属性之上添加的其他属性
person4、person5实列的prototype属性指的是同一个Person.prototype的指针
***
### Day4.构造函数、实例对象、原型对象
**原型链**是指实例对象和原型对象之间的关系，通过__proto__来联系
实例对象的原型__proto__指向的是该对象所在的构造函数的原型对象
构造函数的原型对象（prototype）指向如果改变了，实例对象的原型（__proto__）指向也会发生改变
原型的作用：实现数据共享、继承，目的都是为了节省内存空间
如果属性和方法都需要共享，那么就把属性和方法添加到原型中去

实例对象中有__proto__原型
构造函数中有prototype原型
prototype是对象
所以，prototype这个对象中也有__proto__，
实例对象中的__proto__指向的是构造函数的prototype
因此，prototype这个对象中的__proto__指向的应该是某个构造函数的原型prototype

只要是对象，里面就有下划线原型，即__proto__；
只有有下划线原型，它就指向某个构造函数的prototype
任何构造函数的prototype中都有__proto__属性
***
### Day13.原型实现继承
原型实现继承关系图
![原型实现继承](https://github.com/zhengyeye/JS-practices/blob/master/images/13%E5%8E%9F%E5%9E%8B%E5%AE%9E%E7%8E%B0%E7%BB%A7%E6%89%BF.png)
这张图被自己画的比较凌乱，后续再整理一下。
***
### Day16.拷贝继承
拷贝继承关系图
![拷贝继承](https://github.com/zhengyeye/JS-practices/blob/master/images/16%E6%8B%B7%E8%B4%9D%E7%BB%A7%E6%89%BF.png)
***
### Day17.逆推继承看原型
逆推继承看原型关系图
![逆推继承看原型](https://github.com/zhengyeye/JS-practices/blob/master/images/17%E9%80%86%E6%8E%A8%E7%BB%A7%E6%89%BF%E7%9C%8B%E5%8E%9F%E5%9E%8B.png)
