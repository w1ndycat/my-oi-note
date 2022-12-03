# 广搜（BFS）格式
~~~c++
void bfs(){
    起点入队——起点是结构体对象——包含起点x,y坐标和步数step
    book[起点x坐标][起点y坐标] = 1;
    while(!que.empty()){
        for(队首各个方向){
            int newx ———— 在队首元素x基础上变化
            int newy ———— 在队首元素y基础上变化
            int newstep ———— 在队首元素step基础上+1
            if(1.不越界 2.是通路 3.没用过){
                book[newx][newy] = 1;
                创建结构体对象 ———— 包含newx,newy,newstep
                入队
                if(特判)......
            }
        }
        队首出队 que.pop()
    }
}
~~~
## 总感觉下面的代码能用到
~~~c++
while(!que.empty()){
		for(int i=0;i<4;i++){
			int newx = que.front().x + f[i][0];
			int newy = que.front().y + f[i][1];
			int newstep = que.front().step + 1;
			if(newx<1 or newx>n or newy<1 or newy>m) continue;
			if(ditu[newx][newy]==0 and book[newx][newy]==0){
				book[newx][newy]=1;
				if(newx==ex and newy==ey){
					cout << newstep;
					return 0;
				}
				a = {newx,newy,newstep};
				que.push(a);
			}
		}
		que.pop();
	}
~~~