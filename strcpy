    strcpy  字符串复制
　　原型：char* strcpy(char *dest, const char *src);
　　头文件：<string.h>
　　功能：把src地址开始的含有’\0’的字符串复制到以dest开始的地址空间
　　返回：指向dest的指针，为了实现链式表达式
　　条件：dest和src所指的地址空间不能重叠且dest有足够的空间容纳src的字符串
　　
　　实现1：典型、官方
　　char* my_strcpy(char *dest, char *src)
　　{
　　    assert(dest != NULL && src != NULL);//检查指针有效性，写代码的代码 
　　    char *address = dest;   //保存原始dest地址，以供返回用 
　　    while((*dest++ = *src++) != '\0')  //复制，包括末尾的'\0' 
　　        ;
　　    return address;
　　} 
　　实现2：GNU C中
　　char* my_strcpy_gnu(char *dest, char *src)
　　{
　　    char *address = dest;
　　    while((*dest++ = *src++))  //两层括号为了取表达式的值
　　        ;
　　    return address;
　　} 
　　eg：
　　char dest[10];
　　char *src ="hello";
　　my_strcpy_gnu(dest,src);
