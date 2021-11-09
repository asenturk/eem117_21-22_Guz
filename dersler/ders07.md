```C
#include <stdio.h>

int main() {
	
	char isim[50];
		
	printf("adinizi giriniz: ");
	scanf("%s", isim);

	printf("Merhaba %s\n", isim);
	
	return 0;
}
```



```C
#include <stdio.h>

int main() {

	char sube;

	printf("Sube: ");
	scanf("%c",&sube);
		
	printf("Subeniz: %c",sube);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	char sube;

	printf("Sube: ");
	//scanf("%c",&sube);
	sube = getchar();
	
	printf("Subeniz: %c",sube);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	char sube;

	printf("Sube: ");
	//scanf("%c",&sube);
	sube = getchar();
	
	printf("Subeniz: %c\n",sube);
	
	sube='c';
	
	printf("Subeniz: %c\n",sube);
	
	return 0;
}
```





```C
#include <stdio.h>

int main() {
	float a, b, sonuc;
	char islem;
	printf("islemi girin (+, -, *, /)");
	//islem =getchar();
	scanf("%c",&islem);
	
	printf("iki sayi giriniz: ");
	scanf("%f%f",&a, &b);
	
	if (islem == '+'){
		sonuc=a+b;
		printf("Islem sonucu: %.2f",sonuc);
	}else if(islem == '-'){
		sonuc=a-b;
		printf("Islem sonucu: %.2f",sonuc);
	}else if(islem == '*'){
		sonuc=a*b;
		printf("Islem sonucu: %.2f",sonuc);
	}else if(islem == '/'){
		sonuc=a/b;
		printf("Islem sonucu: %.2f",sonuc);
	}else{
		printf("Hatali secim. ");
	}
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	float a, b, sonuc;
	char islem;
	
	printf("islemi girin (+, -, *, /)");
	islem =getchar();
	//scanf("%c",&islem);
	
	printf("iki sayi giriniz: ");
	scanf("%f%f",&a, &b);
	
	switch(islem){
		case ('+'):
			sonuc=a+b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		case ('-'):
			sonuc=a-b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		case ('*'):
			sonuc=a*b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		case ('/'):
			sonuc=a/b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		default:
			printf("Hatali secim. ");
			break;
	}	
		
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	float a, b, sonuc;
	char islem;
	
	printf("islemi girin (+, -, *, /)");
	islem =getchar();
	//scanf("%c",&islem);
	
	printf("iki sayi giriniz: ");
	scanf("%f%f",&a, &b);
	
	switch(islem){
		case ('+'):
			sonuc=a+b;
			printf("Islem sonucu: %.2f",sonuc);
			
		case ('-'):
			sonuc=a-b;
			printf("Islem sonucu: %.2f",sonuc);
			
		case ('*'):
			sonuc=a*b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		case ('/'):
			sonuc=a/b;
			printf("Islem sonucu: %.2f",sonuc);
			break;
		default:
			printf("Hatali secim. ");
			break;
	}	
		
	return 0;
}
```



```C
#include <stdio.h>

int main() {
	int ekmek, pog, simit;
	float ciro, kdv, kar;
	printf("ekmek pog simit satis sayilarini giriniz: ");
	scanf("%d %d %d", &ekmek, &pog, &simit);
	
	ciro=ekmek*2.0+pog*1.75+simit*1.5;
	printf("satis sonucu ele gecen para: %.2f\n", ciro);
	
	kdv=ciro*0.18;
	kar=ciro-kdv;
	
	printf("odenecek kdv: %.2f\nelde edilen kar: %.2f",kdv, kar);
	
		
	return 0;
}
```




```C
#include <stdio.h>

int main() {
	int binis_saat, binis_dakika;
	int sure_saat, sure_dakika;
	int varis_saat, varis_dakika;
	
	printf("otobusun kalkis saatini giriniz (ss:dd): ");
	scanf("%d:%d",&binis_saat, &binis_dakika);
	
	printf("yolculuk suresini giriniz (ss:dd): ");
	scanf("%d:%d",&sure_saat,&sure_dakika);
	
	varis_dakika = (binis_dakika + sure_dakika)%60;
	
	varis_saat = (binis_saat + sure_saat + (binis_dakika + sure_dakika)/60)%24;
	
	printf("yolculugunuz %.2d:%.2d saatinde bitecek",varis_saat, varis_dakika);
		
	return 0;
}
```


```C
#include <stdio.h>
#include <math.h>

int main() {
	float a,b,c;
	float disc;
	float x1,  x2;
	printf(" ikinci dereceden denklemin katsayilarini giriniz (a,b,c): ");
	scanf("%f%f%f",&a,&b,&c);
	disc=b*b-4*a*c;
	if(disc<0)
		printf("denklemin reel kokleri yoktur");
	else{
		x1=(-b+sqrt(disc))/(2*a);
		x2=(-b-sqrt(disc))/(2*a);
		printf("%.1fx^2 + %.1fx + %.1f = 0\n",a,b,c);
		printf("denkleminin kokleri:\nx1=%.1f\nx2=%.1f",x1,x2);
		
	}
		
	return 0;
}
```


