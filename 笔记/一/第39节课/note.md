# 求最大公约数——__gcd(m,n)
~~~c++
#include<bits/stdc++.h>
using namespace std;
int m,n;
int main(){
    cin >> m >> n;
    cout << __gcd(m,n);


    return 0;
}
~~~
## 注个释
a,bの最小公倍数 = a,bの乘积 ÷ a,bの最大公约数