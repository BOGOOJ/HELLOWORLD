# HELLOWORLD
#pointer
int *p = &a;(p=&a)
p指向a的地址
*p = a  *p是一个整数的值
数组a[];a（数组名）只当作指针 ；a[0]是a[]的首地址 和 a 显示地址相同；
char *p="";    //指向一个字符串地址 只读 不能写；
a[]="";       //是一个数组字符串 可写；


指针 可以相加减 可以相互比较 但不能乘除
1、相减为地址的差除以他们类型的值 eg: int*a,*b;
                                      值为 (a-b)/4
                          
  #  *p++
  ++ 优先级 *高
  *p++ = * (p+n)    n为 数据类型的最小单位  int = 4   char = 1 
  但数组中 可以  *p = a[o] ; *p++ = a[1]
  

#malloc(size_t size)  //这个函数是申请以字节为单位的空间  返回结果为 void* 类型
 （在 #inlucde“stdlib.h”下）
 作用 eg：   int number
              int * a = （int*）malloc(number*sizeof(int));//这样就让a有number个int 的数了 
            free（a）；
// 在最后用完时要 free（a）；   将空间还回去
