Local global ve static değişkenler:
```C
#include <stdio.h>
void f1(int i){
    i++;
    printf("f1 fonk icindeki i: %d\n",i);
}
int main() {
    int i=10;
    f1(5);
    printf("main fonk icindeki i: %d",i);
   return 0;
}
```

    f1 fonk icindeki i: 6
    main fonk icindeki i: 10


```C
#include <stdio.h>
int i=10;
void f1(){
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    printf("1-main fonk gorulen i: %d\n",i);
    f1();
    printf("2-main fonk gorulen i: %d\n",i);
   return 0;
}
```

    1-main fonk gorulen i: 10
    f1 fonk gorulen i: 11
    2-main fonk gorulen i: 11



```C
#include <stdio.h>
int i=10;
void f1(){
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    int i=20;
    printf("1-main fonk gorulen i: %d\n",i);
    f1();
    printf("2-main fonk gorulen i: %d\n",i);
   return 0;
}
```

    1-main fonk gorulen i: 20
    f1 fonk gorulen i: 11
    2-main fonk gorulen i: 20



```C
#include <stdio.h>
int i=10;
void f1(){
    int i=5;
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    int i=20;
    printf("1-main fonk gorulen i: %d\n",i);
    f1();
    printf("2-main fonk gorulen i: %d\n",i);
   return 0;
}
```

    1-main fonk gorulen i: 20
    f1 fonk gorulen i: 6
    2-main fonk gorulen i: 20



```C
#include <stdio.h>
int i=10;
void f1(){
    int i=5;
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    int i=20;
    printf("1-main fonk gorulen i: %d\n",i);
    for(int i=0;i<15;i++)
        printf("%d ",i);
    printf("\n");
    f1();
    printf("2-main fonk gorulen i: %d\n",i);
   return 0;
}
```

    1-main fonk gorulen i: 20
    0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 
    f1 fonk gorulen i: 6
    2-main fonk gorulen i: 20



```C
#include <stdio.h>
int i=10;
void f1(){
    int i=5;
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    int i=20;
    printf("1-main fonk gorulen i: %d\n",i);
    for(i=0;i<15;i++)
        printf("%d ",i);
    printf("\n");
    f1();
    printf("2-main fonk gorulen i: %d\n",i);
   return 0;
}
```

    1-main fonk gorulen i: 20
    0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 
    f1 fonk gorulen i: 6
    2-main fonk gorulen i: 15



```C
#include <stdio.h>

void f1(){
    int i=5;
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    f1();
    f1();
    f1();
   return 0;
}
```

    f1 fonk gorulen i: 6
    f1 fonk gorulen i: 6
    f1 fonk gorulen i: 6



```C
#include <stdio.h>

void f1(){
    static int i=5;
    i++;
    printf("f1 fonk gorulen i: %d\n",i);
}
int main() {
    f1();
    f1();
    f1();
   return 0;
}
```

    f1 fonk gorulen i: 6
    f1 fonk gorulen i: 7
    f1 fonk gorulen i: 8



Stringler (karakter dizisi)

```C
#include <stdio.h>

int main() {
    char a[100];
    printf("bir metin giriniz: ");
    scanf("%s",a);
    printf("girilen metin: %s\n",a);
    printf("a'nin degeri: %u\n",a);
    printf("a[0]'in degeri: %d\n",a[0]);
    printf("a[0]'in degeri: %c\n",a[0]);
    printf("a[0]'in adresi: %u\n",&a[0]);
    printf("a[3]'unn adresi: %u\n",&a[3]);
   return 0;
}
```

    bir metin giriniz: 

     bu_bir_metindir


    girilen metin: bu_bir_metindir
    a'nin degeri: 4015026592
    a[0]'in degeri: 98
    a[0]'in degeri: b
    a[0]'in adresi: 4015026592
    a[3]'unn adresi: 4015026595



```C
#include <stdio.h>

int main() {
    char a[100]={'a',101, 105,'A','\0','x','y','z'};
    int i;
    for(i=0;i<8;i++)
        printf("%c ",a[i]);
    printf("\n");
    printf("%s",a);
   return 0;
}
```

    a e i A x y z 
    aeiA


```C
#include <stdio.h>

int main() {
    char a[100];
    int i;
    printf("bir metin giriniz: ");
    scanf("%s",a);
    printf("%s\n",a);
    for(i=0;i<100;i++)
        printf("%d ",a[i]); 
   return 0;
}
```

    bir metin giriniz: 

     bu_bir_metindir.


    bu_bir_metindir.
    98 117 95 98 105 114 95 109 101 116 105 110 100 105 114 46 0 0 0 0 0 0 0 0 58 21 76 29 28 127 0 0 16 -29 80 29 28 127 0 0 84 -16 80 29 28 127 0 0 -64 18 -94 -44 -1 127 0 0 84 -16 80 29 28 127 0 0 -82 -30 80 29 28 127 0 0 70 27 42 29 28 127 0 0 0 0 0 0 0 0 0 0 0 88 94 -122 89 121 30 -95 -112 -55 105 -37 

```C
#include <stdio.h>

int main() {
    char a[100]="abc.def,g hij-klmno";
    int i;
    for(i=0;i<19;i++)
        printf("%c:%d ",a[i],a[i]);
    printf("\n");
    printf("%s",a);
   return 0;
}
```

    a:97 b:98 c:99 .:46 d:100 e:101 f:102 ,:44 g:103  :32 h:104 i:105 j:106 -:45 k:107 l:108 m:109 n:110 o:111 
    abc.def,g hij-klmno


```C
#include <stdio.h>
#include <string.h>
int main() {
    char a[100]="abc.def,g hija-klmnaoAaHKaH";
    int i, sayac=0;
    //stringin uzunlugu:
    for(i=0;a[i]!='\0';i++)
        if(a[i]=='a')
            sayac++;
    printf("stringdeki a karakterinin sayisi: %d\n", sayac);
    printf("stringin uzunlugu: %d\n",strlen(a));
    printf("stringin uzunlugu: %d",i);
   return 0;
}
```

    stringdeki a karakterinin sayisi: 5
    stringin uzunlugu: 27
    stringin uzunlugu: 27


```C
#include <stdio.h>
#include <string.h>
int main() {
    char a[100]="abc.def,234234g hijadfgsd-klmnaoA456  aHKaH";
    int i=0;
    while(a[i]!='\0')
        i++;

    printf("stringin uzunlugu: %d\n",strlen(a));
    printf("stringin uzunlugu: %d",i); 
   return 0;
}
```

    stringin uzunlugu: 43
    stringin uzunlugu: 43


```C
#include <stdio.h>
#include <string.h>
int main() {
    char a[100]="abc.def,234234g hijadfgsd-klmnaoA456  aHKaH";
    int i=0;
    while(a[++i]!='\0');

    printf("stringin uzunlugu: %d\n",strlen(a));
    printf("stringin uzunlugu: %d",i); 
   return 0;
}
```

    stringin uzunlugu: 43
    stringin uzunlugu: 43


```C
#include <stdio.h>
#include <string.h>
int main() {
    char a[100]="abc.def,234234g hijadfgsd-klmnaoA456  aHKaH";
    int i=0;
    while(a[++i]);
    
    printf("stringin uzunlugu: %d\n",strlen(a));
    printf("stringin uzunlugu: %d",i);
   return 0;
}
```

    stringin uzunlugu: 43
    stringin uzunlugu: 43


```C
#include <stdio.h>
int main() {
    char a[100]="bu bir ifadedir.";
    int i=14;
    while(i >= 0){
        printf("%c",a[i]);
        i--;
    }
   return 0;
}
```

    ridedafi rib ub


```C
#include <stdio.h>
int main() {
    char a[100]="bu bir ifadedir.sdfsdfsdfsd";
    int i=0;
    while(a[i]!='\0'){i++;}
    while(i >= 0){
        printf("%c",a[i]);
        i--;
    }
   return 0;
}
```

    dsfdsfdsfds.ridedafi rib ub


```C
#include <stdio.h>
int main() {
    char a[100]="bu bir ifadedir.sdfsdfsdfsd";
    char b[100];
    int i;
    for(i=0;a[i]!='\0';i++)
        b[i]=a[i];
    b[i]='\0';
    printf("%s",b); 
   return 0;
}
```

    bu bir ifadedir.sdfsdfsdfsd







