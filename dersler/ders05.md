```C
#include <stdio.h>

int main() {
	int a,b=5,c=10.3;
	float x,y,z;
	a=b+c;
	printf("%d+%d=%d \n",b,c,a);
	
	y=10;
	z=15.7
	x=y+z;
	printf("%f + %f = %f \n",y,z,x);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	float x,y,z;
	y=10;
	z=15.7;
	
	x=y+z;
	printf("%f + %f = %f \n",y,z,x);
	x=y*z;
	printf("%f * %f = %f \n",y,z,x);
	x=y/z;
	printf("%f / %f = %f \n",y,z,x);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	float x,y,z;
	y=10.3;
	z=15.7;
	
	x=y+z;
	printf("%.2f + %.2f = %.2f \n",y,z,x);
	x=y*z;
	printf("%.3f * %.3f = %.3f \n",y,z,x);
	x=y/z;
	printf("%11.4f / %11.4f = %11.4f \n",y,z,x);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	int a,b,c;
	a=9;
	b=19;
	c=a*b;
	printf("%5.3d*%4.4d=%7.2d",a,b,c);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	int a,b,c;
	
	printf("1. sayiyi giriniz");
	scanf("%d",&a);

	printf("2. sayiyi giriniz");
	scanf("%d",&b);
	
	printf("3. sayiyi giriniz");
	scanf("%d",&c);
	
	printf("girilen 3 sayinin toplami: %d\n",a+b+c);
	printf("girilen 3 sayinin ortalamasi: %d\n",(a+b+c)/3);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	int a,b,c;
	
	printf("3 sayi giriniz: ");
	scanf("%d%d%d",&a,&b,&c);

	printf("girilen 3 sayinin toplami: %d\n",a+b+c);
	printf("girilen 3 sayinin ortalamasi: %d\n",(a+b+c)/3);

	return 0;
}
```



```C
#include <stdio.h>

int main() {

	float a,b,c;
	
	printf("3 sayi giriniz: ");
	scanf("%f %f %f",&a,&b,&c);

	printf("girilen 3 sayinin toplami: %.3f\n",a+b+c);
	printf("girilen 3 sayinin ortalamasi: %.3f\n",(a+b+c)/3);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	double a,b,c;
	
	printf("3 sayi giriniz: ");
	scanf("%lf %lf %lf",&a,&b,&c);

	printf("girilen 3 sayinin toplami: %.3lf\n",a+b+c);
	printf("girilen 3 sayinin ortalamasi: %.3lf\n",(a+b+c)/3);

	return 0;
}
```

```C
#include <stdio.h>

int main() {
	int hacim, yukseklik, genislik, derinlik;
	printf("Dikdortgenler prizmasinin yukseklik, genislik ve derinligni sira ile giriniz: ");
	scanf("%d%d%d", &yukseklik,  &genislik, &derinlik);
	hacim=genislik*derinlik*yukseklik;
	printf("Yuksekligi: %d\nDerinligi: %d\nGenisligi: %d\nolan prizmanin hacmi:\n%d",
				yukseklik, derinlik, genislik, hacim); 	
	 
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	int pay1, payda1, pay2, payda2;
	printf("a/b seklinde birinci kesiri giriniz: ");
	scanf("%d/%d", &pay1, &payda1);
	
	printf("a/b seklinde birinci kesiri giriniz: ");
	scanf("%d/%d", &pay2, &payda2);
	
	printf("%d/%d x %d/%d = %d/%d \n",pay1, payda1, pay2, payda2,
		pay1*pay2, payda1*payda2);
	
	printf("%d/%d + %d/%d = %d/%d \n",pay1, payda1, pay2, payda2,
		pay1*payda2+pay2*payda1, payda1*payda2);	 
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	float hacim, r;
	float pi=3.14;
	printf("yaricapi giriniz: ");
	scanf("%f", &r);
	
	hacim= (4.0/3)*pi*r*r*r;
	
	printf("yaricapi %f olan kurenin hacmi: %f", r, hacim);
	
	return 0;
}
```


```C
#include <stdio.h>
#define PI 3.14 

int main() {
	float hacim, r;
	// float pi=3.14;
	printf("yaricapi giriniz: ");
	scanf("%f", &r);
	
	hacim= (4.0/3)*PI*r*r*r;
	
	printf("yaricapi %f olan kurenin hacmi: %f", r, hacim);
	
	return 0;
}
```


```C
//bu program hatali neden?
#include <stdio.h>
#define PI (22/7)

int main() {
	float hacim, r;
	//float pi=3.14;
	printf("yaricapi giriniz: ");
	scanf("%f", &r);
	
	hacim= (4.0/3)*PI*r*r*r;
	
	printf("yaricapi %f olan kurenin hacmi: %f", r, hacim);
	
	return 0;
}
```


```C
#include <stdio.h>
#define PI (22.0/7)

int main() {
	float hacim, r;
	//float pi=3.14;
	printf("yaricapi giriniz: ");
	scanf("%f", &r);
	
	hacim= (4.0/3)*PI*r*r*r;
	
	printf("yaricapi %f olan kurenin hacmi: %f", r, hacim);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	printf("cift tirnak kullanmak icin: \"   \n"); 
	printf("ters slash kullanmak icin: \\   \n");
	printf("yeni satir icin: \\n \n");
	printf("tab icin: \\t \n");
	printf("1\t23\t123\n");
	printf("12\t2\t3\n");
	
	return 0;
}
```