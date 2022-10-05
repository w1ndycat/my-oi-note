# 质数
## 质数筛

**因子**个数**为2**——是质数  
**因子**个数**不为2**——不是质数
~~~c++
cin >> n;
for(int i=1;i<=n;i++){
    if(n%1==0) s++;
}
if(s==2) cout << "是质数";
else cout << "不是质数";
~~~
改良亿下
~~~c++
cin >> n;
for(int i=2;i<n;i++){
    if(n%i==0){
        cout << "不是质数";
        return 0;
    }
}
cout << "是质数";
~~~
最终（最**牛逼**）
~~~c++
#include<bits/stdc++.h>
using namespace std;
long long a,b;
bool zhishu(int n){
    if(n<2) return false;
    for(int i=2;i*i<=n;i++){
        if(n%i==0) return false;
    }
    return true;
}
int main(){
    cin >> a >> b;
    for(int i=a;i<=b;i++){
        if(zhishu(i)){
            cout << i << " ";
        }
    }

    return 0;
}
~~~
## 判断质数の方法(即朴素筛)（要背）
~~~c++
bool zhishu(int n){
    if(n<2) return false;
    for(int i=2;i*i<=n;i++){
        if(n%i==0) return false;
    }
    return true;
}
~~~