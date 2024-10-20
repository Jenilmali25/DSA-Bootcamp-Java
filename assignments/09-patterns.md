Pattern Questions

Print these patterns using loops:

```text

1.  *****
    *****
    *****
    *****
    *****


2.  *
    **
    ***
    ****
    *****


3.  *****
    ****
    ***
    **
    *


4.  1
    1 2
    1 2 3
    1 2 3 4
    1 2 3 4 5


5.  *
    **
    ***
    ****
    *****
    ****
    ***
    **
    *
#include<iostream>
using namespace std;

int main(){
    cout<<"Enter n: ";
    int n;
    cin>>n;
    
    for(int i=1; i<=(2*n-1); i++){
        if(i>n){
            int k=(2*n-1)-i+1;
            for(int j=1; j<=k; j++)
                cout<<"*";
        }
        else
            for(int j=1; j<=i; j++){
                cout<<"*";
            }
    cout<<endl;
    }
    
    
    
    return 0;
}


6.       *
        **
       ***
      ****
     *****



7.   *****
      ****
       ***
        **
         *


8.      *
       ***
      *****
     *******
    *********


9.  *********
     *******
      *****
       ***
        *


10.      *
        * *
       * * *
      * * * *
     * * * * *


11.  * * * * *
      * * * *
       * * *
        * *
         *


12.  * * * * *
      * * * *
       * * *
        * *
         *
         *
        * *
       * * *
      * * * *
     * * * * *


13.      *
        * *
       *   *
      *     *
     *********


14.  *********
      *     *
       *   *
        * *
         *


15.      *
        * *
       *   *
      *     *
     *       *
      *     *
       *   *
        * *
         *


16.           1
            1   1
          1   2   1
        1   3   3   1
      1   4   6   4   1


17.      1
        212
       32123
      4321234
       32123
        212
         1
#include<iostream>
using namespace std;

int main(){
    cout<<"Enter n: ";
    int n;
    cin>>n;
    
    for(int i =1; i<=(2*n-1); i++){
        int spaces=i>n?i-n:n-i;
        
        int c=i>n?2*n-i:i;
        
        for(int s=1; s<=spaces; s++)
            cout<<"  ";
        for(int j=c; j>0; j--){
            cout<<j<<" ";
        }
        for(int j=2; j<=c; j++){
            cout<<j<<" ";
        }
        cout<<endl;
    }
    
    
    
    return 0;
}


18.   **********
      ****  ****
      ***    ***
      **      **
      *        *
      *        *
      **      **
      ***    ***
      ****  ****
      **********


19.    *        *
       **      **
       ***    ***
       ****  ****
       **********
       ****  ****
       ***    ***
       **      **
       *        *


20.    ****
       *  *
       *  *
       *  *
       ****

21.    1
       2  3
       4  5  6
       7  8  9  10
       11 12 13 14 15

22.    1
       0 1
       1 0 1
       0 1 0 1
       1 0 1 0 1

23.        *      *
         *   *  *   *
       *      *      *

24.    *        *
       **      **
       * *    * *
       *  *  *  *
       *   **   *
       *   **   *
       *  *  *  *
       * *    * *
       **      **
       *        *

25.       *****
         *   *
        *   *
       *   *
      *****

26.   1 1 1 1 1 1
      2 2 2 2 2
      3 3 3 3
      4 4 4
      5 5
      6

27.   1 2 3 4  17 18 19 20
        5 6 7  14 15 16
          8 9  12 13
            10 11

28.      *
        * *
       * * *
      * * * *
     * * * * *
      * * * *
       * * *
        * *
         *
#include<iostream>
using namespace std;

int main(){
    cout<<"Enter n: ";
    int n;
    cin>>n;
    
    for(int i=1; i<=(2*n-1); i++){
        int col=i>n?(2*n-1)-i+1:i;
        
        int spaces=i>n?i-n:n-i;
        for(int s=1; s<=spaces; s++){
            cout<<" ";
        }
        
        for(int j=1; j<=col; j++){
            cout<<"* ";
        }
        cout<<endl;
            
    }
    
    
    
    return 0;
}

29.      
       *        *
       **      **
       ***    ***
       ****  ****
       **********
       ****  ****
       ***    ***
       **      **
       *        *

30.         1
          2 1 2
        3 2 1 2 3
      4 3 2 1 2 3 4
    5 4 3 2 1 2 3 4 5


31.      4 4 4 4 4 4 4  
         4 3 3 3 3 3 4   
         4 3 2 2 2 3 4   
         4 3 2 1 2 3 4   
         4 3 2 2 2 3 4   
         4 3 3 3 3 3 4   
         4 4 4 4 4 4 4
#include<iostream>
#include<cmath>
using namespace std;

int main(){
    cout<<"Enter n: ";
    int n;
    cin>>n;
    n=2*n-1;
    for(int i=1; i<=n; i++){
        for(int j=1; j<=n; j++){
            int c=min(min(i, j), min(n-i+1, n-j+1));
            cout<<c<<" ";
        }
        cout<<endl;
    }
    
    
    
    return 0;
}

32.    E
       D E
       C D E
       B C D E
       A B C D E

33.    a
       B c
       D e F
       g H i J
       k L m N o
     
34.    E D C B A
       D C B A
       C B A
       B A
       A
       
35.    1      1
       12    21
       123  321
       12344321
```
