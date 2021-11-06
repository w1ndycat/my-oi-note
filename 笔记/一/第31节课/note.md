# printf&scanf的用法
贼难用（小声逼逼）
## printf
~~~c++
double a;
cin >> a;
printf("%.3lf",a)
~~~
相当于
~~~c++
cout << fixed << setprecision(3) << a;
~~~
**懂?**