# Experiment 15

**Aim:** <br>
To study and implement Recursion. <br>
<br>
**Theory:** <br>
In C++, recursion is executed through when a function calls itself. The concept itself is essentially the same as in other programming languages; the function ultimately calls itself with changed arguments consistently until a base case is reached at which point it will stop calling itself and begin returning results along the route of recursive calls.  <br>
<br>
Properties of Recursion: <br>
&#8594; _Base Case:_ Recursion stops when there is a condition. <br>
&#8594; _Recursive Case_: It is a solution to sub problems through recursive call. <br>
&#8594; _Call Stack:_ The modules that contain each separate function in memory. <br>
&#8594; _Overhead:_ Non-direct calculations that bite into the call and storage space. <br>
&#8594; _Memory Consumption:_ Excessive levels of recursion may lead to rampant overflow of state. <br>
&#8594; Tail Recursion: This is a type of recursion where the last action is that of invoking another instance of the same function, and thus optimizations can be made. <br>
&#8594; Direct/Indirect Recursion: This is an instance of recursion in which the function invokes itself directly or indirectly. <br>
&#8594; Multiple Recursive Calls: Functions can perform more than one recursive call. <br>
&#8594; Backtracking: This method is used in algorithms that use multiple paths to find solutions. <br>
<br>

**Code:** <br>
<br>
a.<br>

```
#include <iostream>
using namespace std;
int fact(int n)
{
    if (n<=1)
    {
        return 1;
    }
    else
    {
        return (n*fact(n-1));
    }
}
int main()
{
    int x,n;
    cout<<"Enter a number: ";
    cin>>n;
    x= fact(n);
    cout<<n<<"!: "<<x;
}


```
<br>
b.<br>

```
#include <iostream>
using namespace std;
int add(int n)
{
    if (n<=1)
    {
        return 1;
    }
    else
    {
        return (n+add(n-1));
    }
}
int main()
{
    int x,n;
    cout<<"Enter a number: ";
    cin>>n;
    x= add(n);
    cout<<x;
}

```
<br>
c.<br>

```
#include <iostream>
#include <string>
using namespace std;
void rev(char *str)
{
    if (*str)
    {
        rev(str+1);
        cout<<("%c",*str);

    }

}
int main()
{
    char s[50];
    cout<<"Enter a string: ";
    cin>>s;
    rev(s);
}

```
<br>
d.<br>

```
#include <iostream>
#include <string>
using namespace std;
void revn(int i)
{
    if (i>0)
    {
        cout<<i%10;
        revn(i/10);
        

    }

}
int main()
{
    int i;
    cout<<"Enter a number: ";
    cin>>i;
    revn(i);
}

```
<br>

**Outputs:**  <br>
<br>
a.<br>
![exp15a](https://github.com/user-attachments/assets/a22000b8-467d-431d-bc1e-faed72aad425)
 <br>
b.<br>
![exp15b](https://github.com/user-attachments/assets/153b99b9-7b87-4045-8ecc-a7f4169f6687)
 <br>
c.<br>
![exp15c](https://github.com/user-attachments/assets/c5125880-cabb-4ff0-aff9-595798c31fac)
 <br>
d.<br>
![exp15d](https://github.com/user-attachments/assets/584c068b-a1a6-4273-a915-b14244676772)
 <br>



<br>

**Conclusion:** <br>
&#8594; We learnt about recursion in C++. <br>
&#8594; We learnt the use case of recursion in C++. <br>
*******
<br>
