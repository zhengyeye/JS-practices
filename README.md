# JS-practices
### Day1.创建对象的四种方式：
原型关系图
![原型关系图](https://github.com/zhengyeye/JS-practices/blob/master/%E5%AF%B9%E8%B1%A1.png)

解释：创建Person构造函数后，其默认拥有prototype属性，指向的是Person的原型；
而Person的原型默认拥有constructor属性，该属性指向Person的构造函数
Person原型中的其他属性，比如name，age，是在Person原型属性之上添加的其他属性
person4、person5实列的prototype属性指的是同一个Person.prototype的指针
