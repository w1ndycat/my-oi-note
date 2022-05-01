# 双端队列
## 声明
~~~c++
deque<int> que;
~~~
## 判断是否为空
~~~c++
que.empty();
~~~
## 求大小
~~~c++
que.size();
~~~
## （让我！）访问队首元素
~~~c++
que.front();
~~~
## （让我！）访问队尾元素
~~~c++
que.back();
~~~
## 插进队首
~~~c++
que.push_front(...);
~~~
## 插进队尾
~~~c++
que.push_back(...);
~~~
## 拔出队尾
~~~c++
que.pop_back();
~~~
## 拔出队首
~~~c++
que.pop_front();
~~~