# sizeof函数——可以一个数组全赋同一个值
~~~c++
memset(数组名,要赋的值,sizeof(数组名))
~~~
# 栈の模板——用数组模拟栈
~~~c++
#include<bits/stdc++.h>
using namespace std;
int a[1001],m;
int main(){
    //用数组模拟栈
    int top=1;
    //入栈
    while(cin >> m){
        a[top++] = m;
    }
    //获取栈顶元素
    cout << a[top-1] << endl;
    //出栈
    top--;

    return 0;
}
~~~
