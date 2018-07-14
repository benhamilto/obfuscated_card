Just a dumb program that prints a basic business card to the console.

Code is purposefully obfuscated and shortened to fit on the rear side of a business card.


Sample output (may not be up to date):
```
 ------------------------------------------------------------ 
|                                                            |
|                                                            |
|    Ben Hamilton                                            |
|                                                            |
|                                                            |
|                                                            |
|                                                            |
|    P: ***-***-****                                         |
|    E: benhamilton10@gmail.com                              |
|                                                            |
|                                                            |
|                                                            |
 ------------------------------------------------------------ 
|#include <iostream> //g++ -o prog prog.cpp && ./prog        |
|#include <fstream>                                          |
|#define c(x) std::cout<<x;                                  |
|std::string l,m="",a[6]={" --------------------------------"|
|"---------------------------- \n","|                       "|
|"                                     |\n","Ben Hamilton",  |
|"P: ***-***-****","E: benhamilton10@gmail.com"};int main(){c|
|(a[0]);std::ifstream f; f.open("prog.cpp");for(int i = 0;i< |
|12 ;i++){m = a[1];c((i==2?m.replace(5,12,a[2]):i==7?        |
|m.replace(5,15,a[3]):i==8?m.replace(5,26,a[4]):m));}c(a[0]);|
|if( f.is_open()){while(getline(f,l)){m=a[1];c(m.replace(1,  |
|l.length(),l));}f.close();c(a[0]);}}                        |
 ------------------------------------------------------------ 
```
