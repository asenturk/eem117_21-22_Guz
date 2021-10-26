## düzenlenecek!

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
	int a,b=5,c=10.3;
	float x,y,z;
	a=b+c;
	printf("%d+%d=%d \n",b,c,a);
	
	y=10;
	z=15.7;
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
	printf("%.10f + %.10f = %.10f \n",y,z,x);
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
	printf("%7.4f / %7.4f = %7.4f \n",y,z,x);

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
	
	printf("1. sayiyi giriniz: ");
	scanf("%d",&a);

	printf("2. sayiyi giriniz: ");
	scanf("%d",&b);
	
	printf("3. sayiyi giriniz: ");
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

	int a,b,c;
	
	printf("3 sayi giriniz: ");
	scanf("%d %d %d",&a,&b,&c);

	printf("girilen 3 sayinin toplami: %d\n",a+b+c);
	printf("girilen 3 sayinin ortalamasi: %d\n",(a+b+c)/3);

	return 0;
}
```


```C
#include <stdio.h>

int main() {

	double a,b,c;
	
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



