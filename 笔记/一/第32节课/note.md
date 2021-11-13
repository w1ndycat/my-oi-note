# 循环输入の好写法
n组数据
~~~c++
int n;
~~~
每一个数据
~~~c++
int a;
~~~
循环输入
~~~c++
cin >> n;
while(n--){
    cin >> a;
}
~~~
# sortの稳定版本——stable_sort
## 主要是不容易出bug
~~~c++
stable_sort()
~~~