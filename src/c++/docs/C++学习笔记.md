# 基础知识

bool	存储值 true 或 false。
char	通常是一个八位字节（一个字节）。这是一个字符串类型。
int	对机器而言，整数的最自然的大小。
float	单精度浮点值。
double	双精度浮点值。
void	表示类型的缺失。
wchar_t	宽字符类型。

#define 和 const 命名常量 （unix环境高级编程）

#define 主要用来定义宏，用来做展开

# 和 ## 预处理运算符在 C++ 和 ANSI/ISO C 中都是可用的。# 运算符会把 replacement-text 令牌转换为用引号引起来的字符串。

## 运算符用于连接两个

signed
unsigned
long
short


const	const 类型的对象在程序执行期间不能被修改改变。
volatile	修饰符 volatile 告诉编译器，变量的值可能以程序未明确指定的方式被改变。
restrict	由 restrict 修饰的指针是唯一一种访问它所指向的对象的方式。只有 C99 增加了新的类型限定符 restrict。

存储类
auto
在C++11 中， auto 关键字不再是C++存储类说明符。从C++11开始，auto 关键字声明一个变量，该变量的类型是从其声明中的初始化表达式推导出来的。
auto 只能用在函数内，即 auto 只能修饰局部变量。

register
register 存储类用于定义存储在寄存器中而不是 RAM 中的局部变量。这意味着变量的最大尺寸等于寄存器的大小（通常是一个词），且不能对它应用一元的 '&' 运算符（因为它没有内存位置）。

static（堆栈为止）
static 存储类指示编译器在程序的生命周期内保持局部变量的存在，而不需要在每次它进入和离开作用域时进行创建和销毁。因此，使用 static 修饰局部变量可以在函数调用之间保持局部变量的值。

static 修饰符也可以应用于全局变量。当 static 修饰全局变量时，会使变量的作用域限制在声明它的文件内。

在 C++ 中，当 static 用在类数据成员上时，会导致仅有一个该成员的副本被类的所有对象共享。

extern
extern 修饰符通常用于当有两个或多个文件共享相同的全局变量或函数的时候，如下所示


mutable
mutable 说明符仅适用于类的对象，这将在本教程的最后进行讲解。它允许对象的成员替代常量。也就是说，mutable 成员可以通过 const 成员函数修改。


__LINE__	这会在程序编译时包含当前行号。
__FILE__	这会在程序编译时包含当前文件名。
__DATE__	这会包含一个形式为 month/day/year 的字符串，它表示把源文件转换为目标代码的日期。
__TIME__	这会包含一个形式为 hour:minute:second 的字符串，它表示程序被编译的时间。


pthread.h

https://www.w3cschool.cn/cpp/cpp-az4l3kdi.html

https://en.cppreference.com/w/