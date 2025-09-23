# const
### const含义
1.const 属于类型修饰符 用const 修饰的变量或对象的值是不可被更新的。
### const 作用
1.用于修饰，防止修改，节省空间。
### 指针与const
1.常指针 char * const a;
2.指向const 对象的指针 const char * a 等价于 char const * a
3.指向const 对象的常指针 const char * const a
注意 不能使用void *指针保存const 对象的地址，如果要使用必须使用const void *
补充：void *指针不能直接解引用，需要先进行类型转换，void *指针可以指向任何数据类型，主要用于泛型编程和内存管理函数等。
### 函数与const
1.const 修饰函数参数时 表示参数在函数内不可变，在值传递时无意义，可以用于保证指针内容不可变，以及在自定义类型中使用 const A & a 加快效率，避免了复制的时间消耗。
### 类与const
1.const对象只能使用const 成员函数，而非const 对象可以访问任意的成员函数 