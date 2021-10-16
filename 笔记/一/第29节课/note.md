# C++函数
## 主函数
~~~c++
int main(){
    return 0;
}
~~~
熟悉的配方，熟悉的味道
## 无返回值
~~~c++
void cao(){
    cout << "lbwnb!!!" << endl;
    return;
}
~~~
不过，要**调用**一下
~~~c++
cao()
~~~
输出结果
~~~markdown
lbwnb!!!
~~~
熟悉的配方，熟悉的味道
## 有返回值
~~~c++
string oac(){
    return "lbwnb!!!";
}
~~~
这里string**可以替换**为bool,int或其他数据类型，但return的数据类型也要**相同**  
返回值要用一个**变量**接收
~~~c++
string a = oac();
cout << a;
~~~
输出结果
~~~markdown
lbwnb!!!
~~~
**或者**
~~~c++
int ac(int a,int b){
    return a+b;
}
~~~
~~~c++
int ca = ac(2233,2233)
cout << ac();
~~~