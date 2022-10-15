# 高精度加法（不考虑负数）
~~~c++
#include<bits/stdc++.h>
using namespace std;
string s1,s2;
int a[10086],b[10086],c[10086]; // a,b——加数    c——和
int main(){
	cin >> s1 >> s2;
	// 倒序
	int L1 = s1.size();
	int L2 = s2.size();
	for(int i=0;i<L1;i++){
		a[i] = s1[L1-1-i]-'0';
	}
	for(int i=0;i<L2;i++){
		b[i] = s2[L2-1-i]-'0'; 
	}
	// 相加
	int L = max(L1,L2);
	int x=0;// 进位
	for(int i=0;i<L;i++){
		c[i] = a[i] + b[i] + x;
		x = c[i]/10;
		c[i] = c[i]%10;
	}
	
	// 特殊处理——x
	if(x==1){
		c[L]= 1;
		L++;
		
	}
	// 输出
	for(int i=L-1;i>=0;i--){
		cout << c[i];
	}
	
	return 0;
}
~~~