# 字符串和字符串函数

不要使用指针来改变一个已经用字面值初始化的字符串。如果有两个字符串字面值相同，则它在内存中的位置可能相同，用指针改变一个可能导致改变另一个。字符串属于静态储存类。

| 字符串函数 | 用法 |
| --- | --- |
| gets(char *) | 读取字符串直到遇到换行符，丢弃换行符，添加空字符 |
| fgets(char *, int n, stdin) | 读取字符串直到遇到换行符或读取完 **(n-1)** 个字符，n指定 **数组最大可容纳的字符数（包括空字符在内）**而不是最大可读取的字符数，保留换行符，添加空字符 |
| puts(char *) | 输出字符串，添加换行符 |
| fputs(char *, stdout) | 输出字符串，不添加换行符 |
| `<string.h>` | --- |
| strlen(char *) | 字符串长度 |
| strcat(char *, const char *) | 将第二个字符串链接到第一个字符串后面，返回值是第一个字符串 |
| strncat(char *, const char *, int) | 连接字符串，指定最大可添加的字符数（注意为空字符保留位置） |
| strcmp(char *, char *) | 按机器编码顺序比较字符串 |
| strncmp(char *, char *, int) | 限制搜索的范围 |
| strcpy(char *, char *) | 将第二个字符串复制到第一个字符串的位置，返回值是第一个字符串 |
| strncpy(char *, char *, int) | 指定最大可复制的字符数（注意为空字符保留位置），最终结果“充盈”n个字符 |
| --- | --- |
| sprintf(char *, 其余参数与printf相同) | 格式化字符串并输出到指定位置 |
| --- | --- |
| strchr(char * s, int c) | 返回指向在s中存放字符c的第一个位置的指针，未找到则返回空指针 |
| strpbrk(char *, char *) | 返回指向在第一个字符串中存放第二个字符串任意一个字符的位置的指针，未找到则返回空指针 |
| strrchr(char *, int c) | 返回指向字符最后一次出现在字符串中的位置的指针 |
| strstr(char *, char *) | 返回第一个字符串中第一次出现第二个字符串的位置 |
| `<stdlib.h>` | --- |
| atoi(char *)| Alphanumeric to integer，将字符串转换为整数并返回 |
| atol, atof等 | 返回long、float类型 |
| strtol, strtoul, strtod | 可以报告第一个不是数字的字符的位置 |
| ftoa, itoa等 | 不是标准函数 |