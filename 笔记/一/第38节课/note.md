# 栈の循环入栈&循环出栈
~~~c++
#include<bits/stdc++.h>
using namespace std;
stack<int>   st;
int main(){
    // 循环入栈
    for(int i=1;i<=3;i++){
        st.push(i);
    }
    // 循环出栈
    while(!st.empty()){
        cout << st.top << endl;
        st.pop();
    }

    return 0;
}