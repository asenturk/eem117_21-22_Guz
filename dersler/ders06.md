```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b)
		printf("%birinci sayi buyuktur: %d",a);
	
	if(b>a)
		printf("ikinci sayi buyuktur: %d",b);
	
	if(a==b)
		printf("iki sayi birbirine esit: %d, %d",a,b);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b)
		printf("birinci sayi buyuktur: %d",a);
	else
		printf("ikinci sayi buyuktur: %d veya sayilar esit",b);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b)
		printf("birinci sayi buyuktur: %d",a);
	else if(a==b)
		printf("sayilar esit");
	else
		printf("ikinci sayi buyuktur: %d",b);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b)
		printf("birinci sayi buyuktur: %d",a);
	else if(a<b)
		printf("birinci sayi kucuktur: %d",a);

	return 0;
}
```

Yapmış olduğumuz hizalamalar kodu daha rahat anlamak için yoksa aşağıdaki gibi bir kod da çalışır.
```C
#include <stdio.h>
int main() {int a,b;printf("iki sayi giriniz"); scanf("%d%d",&a,&b); if(a>b)printf("birinci sayi buyuktur: %d",a); else if(a<b) printf("birinci sayi kucuktur: %d",a); return 0;}
```


```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b)
	
	printf("birinci sayi buyuktur: %d",a);
	printf("bu ifade her halukarda calisir.");
		
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int a,b;
	printf("iki sayi giriniz");
	scanf("%d%d",&a,&b);
	
	if(a>b){
		printf("birinci sayi buyuktur: %d\n",a);
		printf("bu ifin icindeki 2. ifade");
	}
	
	return 0;
}
```


```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10)
	if(a<20)
	printf("girilen sayi 10 ile 20 arasindadir");
	else
	printf("1: girilen sayi 10 ile 20 arasinda degil");
	else
	printf("2: girilen sayi 10 ile 20 arasinda degil");
	
	return 0; 
}  
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10)
		if(a<20)
			printf("girilen sayi 10 ile 20 arasindadir");
 		
	return 0;
} 
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10)
				
		if(a<20)
			printf("girilen sayi 10 ile 20 arasindadir");	 
		else
			printf("1: girilen sayi 10 ile 20 arasinda degil");
			
	return 0;
} 
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10)
	if(a<20)
			printf("girilen sayi 10 ile 20 arasindadir");	 
		else
			printf("1: girilen sayi 10 ile 20 arasinda degil");
	else
		printf("2: girilen sayi 10 ile 20 arasinda degil");
	
	return 0;
} 
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10)
	if(a<20)
	printf("girilen sayi 10 ile 20 arasindadir");	 
	else
	printf("1: girilen sayi 10 ile 20 arasinda degil");
	else
	printf("2: girilen sayi 10 ile 20 arasinda degil");
	
	return 0; 
}  
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a>10 && a<20)
		printf("girilen sayi 10 ile 20 arasindadir");	 	
	else
		printf("girilen sayi 10 ile 20 arasinda degil");	
	
	return 0; 
}  
 ``` 



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("bir sayi giriniz");
	scanf("%d",&a);
	
	//girilen sayi 10 ile 20 arasında mi?
	if(a<10 || a>20)
		printf("girilen sayi 10dan kucuk 20den buyuktur.");	 	
	else
		printf("girilen sayi 10 ile 20 arasinda (sayilar dahil)");
	
	return 0; 
}  
 ``` 

```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=0;i<10;i++)
		printf("%d ",i);
		
	return 0; 
} 

```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=0;i<100;i++)
		printf("%d ",i);
	
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=10;i<100;i=i+3)
		printf("%d ",i);
		
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=97;i<100;i=i+3)
		printf("%d ",i);
	
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=100;i>0;i--)
		printf("%d ",i);
		
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=100;i>0;i=i-5)
		printf("%d ",i);
		
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=100;i>0;){
		if(i>50)
			i=i-3;
		else
			i=i-2;
		printf("%d ",i);
	}
		
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	
	for(i=100;i>0;){
		printf("%d ",i);
		if(i>50)
			i=i-3;
		else
			i=i-2;	
	}

	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	int carpim=1;
	
	for(i=40;i<50;i++){
		carpim = carpim * i;	
	}
	printf("%d",carpim);
		
	return 0; 
} 
```


```C
#include <stdio.h>

int main() {
	
	int i;
	int toplam=0;
	
	for(i=10;i<20;i++){
		toplam = toplam + i;	
	}
	printf("%d",toplam);
	
	return 0; 
} 
```