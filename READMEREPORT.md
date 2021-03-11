# lab.02
report

art 1
1) $ cd ${GITHUB_USERNAME}/workspace/projects; mkdir lab.02; cd lab.02
$ git init; git remote add origin https://github.com/${GITHUB_USERNAME}/lab.02.git
2)$ touch README.md; git add README.md; git commit -m"added readme" -a ; git push origin master
3)$ touch hello_world.cpp; edit hello_world.cpp

#include <iostream>
using namespace std;
int main() {
cout << "**HELLO WORLD**" << endl;
return 1;
}
 
4)$ git add hello_world.cpp
5)$ git commit -m"added helloworld" -a; git push origin master
6)$ edit hello_world.cpp

#include <iostream>
#include <string>
using namespace std;
int main(){
string a; cin»a;
cout << endl << "HELLO WORLD FROM " << a << endl;
return 1;}

7)$ git commit -m" clean hellow" -a; 
8)$ git push origin master
9)$ git status; git log;


part 2
1)$ git checkout -b patch1
2)$ edit hello_world.cpp

#include <iostream>
#include <string>
int main(){
string a; std::cin»a;
std::cout << endl << "HELLO WORLD FROM " << a << endl;
return 1;}

3)$ git commit -m" clean hellow" -a; git push origin patch1

4)ручками на сайте
5)$ git pull-request patch1->master
6)$ edit hello_world.cpp

#include <iostream>
#include <string>
int main(){
string a; std::cin >> a;//deleted"using namespace std"
std::cout << endl << "HELLO WORLD FROM " << a << endl;
return 1;}

7)$ git commit -m"added comments" -a ; git push origin patch1
8)ручками на сайте
9)$ git checkout master
$ git merge patch1
$ git push origin master
$ git push origin :patch1
$ git checkout master 

10)$ git pull origin master
11)$ git log
12)$ git branch -D patch1
