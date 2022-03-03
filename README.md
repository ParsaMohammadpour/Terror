# Terror!
## About The Project
It was one of my ***algorithm*** class assignments.
This question's topic was about ***BFS & DFS algorithms***.
In the questions there are some limits that we are going to mention.

## Question
### Main Question
نیما اخیراً مدیر فنی شرکت کدنویس گستران شرق به جز محمدرضا شده است. با توجه به این که نیما در حال حاضر فقط پول پارو می کند و بازار کار را برای سایر برنامه نویسان کساد کرده، گروهی از برنامه نویسان کلاه قرمز با هم تبانی کرده و قصد ترور نیما را دارند.

این برنامه نویس ها می دانند که نیما هم اکنون درگیر انجام یک پروژه است (نیما از هیچ فرصتی برای کسب درآمد دریغ نمی کند)؛ بنابراین، او هر روز صبح در یک جلسه در یک ساختمان شرکت می کند. این ساختمان ها از ۱ تا nn شماره گذاری شده اند. آنها همچنین می دانند که اگر نیما در روز dاُم در جلسه ی ساختمانiاُم شرکت کند، در روزd+1اُم در جلسه ی ساختمان b_i
  شرکت می کند، اما نمی دانند که در روز اول نیما در کدام یک از ساختمان ها بوده. آن ها برای ترور کردن نیما باید تعدادی ساختمان را بمب گذاری کنند و آن قدر منتظر بمانند تا نیما وارد یکی از این ساختمان ها شود. هزینه ی بمب گذاری در ساختمان iiاُم برابر با c_iاست.
کمینه ی هزینه ی بمب گذاری را پیدا کنید؛ به این صورت که تعدادی از ساختمان ها را بمب گذاری کنیم و مطمئن باشیم که نیما بالأخره در جلسه ی یکی از این ساختمان ها شرکت می کند.

### Limits
محدودیت زمان: ۱ ثانیه
محدودیت حافظه: ۲۵۶ مگابایت


### Inputs
در خط اول، عدد صحیح n وارد می شود.

1 <= n <= 10 ^ 6

در خط دوم، n عدد صحیح وارد می شود که عدد iاُم بیانگر b_i است.

1 <= b_i <= n

در خط سوم، n عدد صحیح وارد می شود که عدد iاًم بیانگر هزینه ی بمب گذاری در ساختمان iاُم (c_i) است.

1 <= c_i <= 10^9
### Outputs
کمینه ی هزینه ی بمب گذاری برای ترور کردن نیما را چاپ کنید.

### Examples
#### Input1
10
5 3 4 2 6 8 9 1 10 7
6 9 1 1 1 10 2 4 9 6

#### Output1
4

#### Input2
10
7 1 6 3 4 8 5 10 2 9
9 19 19 1 3 9 1 12 10 8

#### Output2
1

## Answer
As we said, this question is solved by ***BFS Algorithm***.
The only point is the way that we recieving inputs.Because of the time limit, we was forced to use a faster way instead of using _Scanner_ class.
The solution is to search all the graph nodes, one by one and if we have passed (for this usage we defined a passed matrix which is matrix of boolean) that special node, we don't disscuss about that node anymore and we just simply pass that node. But if we haven't passed that node we go through that node and all nodes whivh are connected to that node to find the minimum price of a node which is located in that path(with ***BFS Algorithm***). then we add that minimum to the main Sum.
At the end we print that Main sum.

## Run & Compile
for running and compiling this project you can simply make a project with the file name in _Intellij IDE_ or compile and run it in your command line.
There is nothing strange or unusual about running and compiling this project.
