```C 
#include <stdio.h>

int main() {
	
	return 0;
}
 ``` 

```C 
#include <stdio.h>

int main() {
	
	/* bu program ilk c programim */
	
	/*
	bu cok satirli yorum
	ikinci satir
	*/
	
	//tek satır yorum için // kullanılabilir.
	
    return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	//ilk program
	printf("Merhaba dunya!\n");

	return 0;
}
```

```C 
#include <stdio.h>

int main() {
	
	printf("Merhaba dunya!\n");
	printf("\nMerhaba dunya!");
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	printf("****\n");
	printf("*  *\n");
	printf("*  *\n");
	printf("*  *\n");
	printf("****\n\n");
	
	printf("****\n*  *\n*  *\n*  *\n****\n");

	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	printf("\\\\\\\\");

	return 0;
}
```


```C 
#include <stdio.h>

int main() {
	
	char a;
	a = 97;
	printf("a: %d \n", a);
	printf("a: %c \n", a);
	
	a=100;
	printf("a: %d \n", a);
	printf("a: %c \n", a);
	
	a=70;
	printf("a: %d \n", a);
	printf("a: %c \n", a);
	
	a=66;
	printf("a: %d \n", a);
	printf("a: %c \n", a);
	
	printf("%d:%c \n",105,105);	
	
	printf("%d:%c \n",a+9,a+9);
	
	printf("a degiskeninin bellekte kapladigi alan: %d bytetir\n",sizeof(a));
	printf("char turunun bellekte kapladigi alan: %d bytetir\n",sizeof(char));
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a=1000;	
	printf("a degiskeninin bellekte kapladigi alan: %d bytetir\n",sizeof(a));
	printf("int turunun bellekte kapladigi alan: %d bytetir\n",sizeof(int));
	printf("short turunun bellekte kapladigi alan: %d bytetir\n",sizeof(short));
	printf("long turunun bellekte kapladigi alan: %d bytetir\n",sizeof(long));
	printf("float turunun bellekte kapladigi alan: %d bytetir\n",sizeof(float));
	printf("double turunun bellekte kapladigi alan: %d bytetir\n",sizeof(double));
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b, c;
	a=1000;
	b=2000;
	c=a-b;
	printf("%d - %d = %d",a,b,c);	
	
	return 0;
}
```

```C 
#include <stdio.h>

int main() {
	
	int a, b, c;
	a=1000;
	b=2000;
	c=a/b;
	printf("%d / %d = %d",a,b,c);	
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b, c;
	a=25;
	b=10;
	c=a/b;
	printf("%d / %d = %d",a,b,c);	

	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b, c;
	a=25;
	b=10;
	c=a%b;
	printf("%d %% %d = %d",a,b,c);	
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b, c, d;
	a=25;
	b=10;
	c=a/b;
	d=a%b;
	printf("%d = %d x %d + %d ",a,b,c);	

	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a=2521654, b=14210;

	printf("%d = %d x %d + %d ",a,b,a/b,a%b);	
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b;
	printf("birinci sayiyi giriniz: ");
	scanf("%d", &a);
	printf("ikinci sayiyi giriniz: ");
	scanf("%d", &b);

	printf("%d = %d x %d + %d ",a,b,a/b,a%b);	
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b;
	printf("birinci sayiyi giriniz: ");
	scanf("%d", &a);
	printf("ikinci sayiyi giriniz: ");
	scanf("%d", &b);

	printf("%d = %d x %d + %d ",a,b,a/b,a%b);	
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("sayi giriniz: ");
	scanf("%d", &a);
	//a=a+100;
	a += 100;
	printf("%d\n",a);
	
	//a=a+1;
	a += 1;
	printf("%d\n",a);
	
	//a=a*10;
	a *= 10;
	printf("%d\n",a);
	
	//a=a/10;
	a/=10;
	printf("%d\n",a);
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a;
	printf("sayi giriniz: ");
	scanf("%d", &a);
	
	a++;
	printf("%d\n",a);
	
	a--;
	printf("%d\n",a);
	
	++a;
	printf("%d\n",a);
	
	--a;
	printf("%d\n",a);
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a, b;
	printf("sayi giriniz: ");
	scanf("%d", &a);
	
	a++;
	printf("%d\n",a++);
	
	a--;
	printf("%d\n",a--);
	
	
	++a;
	printf("%d\n",++a);
	
	--a;
	printf("%d\n",--a);
	
	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	int a=10, b=20, c=30, d;
	
	d= ++a + ++b + c++;
	printf("%d %d %d %d",a,b,c,d);

	return 0;
}
```



```C 
#include <stdio.h>

int main() {
	
	printf("%d \n",10>20); //0
	printf("%d \n",10>10); //0
	printf("%d \n",10>=10); //1
	printf("%d \n",10>5); //1
	
	printf("%d \n",10<20); //1
	printf("%d \n",20<20); //0
	printf("%d \n",20<=20); //1
	printf("%d \n",30<=20); //0
	
	printf("%d \n",20==10); //0
	printf("%d \n",20==20); //1
	printf("%d \n",20!=10); //1
	printf("%d \n",10!=10); //0
	
	printf("%d \n",!(10<20)); //0
	printf("%d \n",!(30<20)); //1

	return 0;
}
```

