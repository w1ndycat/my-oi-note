# 0-1背包
## ~~也是P1048的题解~~
~~~c++
#include<bits/stdc++.h>
using namespace std;
int m,n;//m背包容量，n物品个数
int w[105];//物品の体积
int v[105];//物品の价值
int f[1005];//f[j]为当前容量j下的最大价值
int main(){
	cin >> m >> n;
	for(int i=1;i<=n;i++) cin >> w[i] >> v[i];
	// 0-1背包
	for(int i=1;i<=n;i++){// 遍历物品
		for(int j=m;j>=w[i];j--){// 遍历容量
			f[j] = max(f[j],f[j-w[i]]+v[i]);
		}
	}
	cout << f[m];
	
	return 0;
}
~~~