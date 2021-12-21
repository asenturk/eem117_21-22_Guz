```C
// ornek fonksiyon tanimlamalari
// fonksiyonların input ve outputlarının
// goruldugu asagidaki gosterimlere
// fonksiyon prototipi denir.
// fonksiyona girilen değerler parametre olarak
// adlandirilir.
// fonksiyonların başındaki ifade döndürülen
// değerin turudur.

int us_al(int taban, int us);

void yazdir(void);

void topla_ve_yazdir(int sayi1, int sayi2);

int klavyeden_al_yazdir(void);

int faktoriyel(int n);

```

```C
#include <stdio.h>

void yazdir(void){
	printf("############################\n");
	printf("###yapilan islemin sonucu###\n");
	printf("############################\n");
}
int main() {
	int a,b;
	printf("toplam islemi icin degerleri giriniz: ");
	scanf("%d%d",&a,&b);
	yazdir();
	printf("%d",a+b);

return 0;
}
```

```C
#include <stdio.h>

void topla_ve_yazdir(int sayi1, int sayi2){
	printf("############################\n");
	printf("###yapilan islemin sonucu###\n");
	printf("############################\n");
	printf("%d",sayi1+sayi2);	
}
int main() {
	int a,b;
	printf("toplam islemi icin degerleri giriniz: ");
	scanf("%d%d",&a,&b);
	topla_ve_yazdir(a,b);

return 0;
}
```

```C
#include <stdio.h>

float ortalama_bul(float sayi1, float sayi2, float sayi3){
	float toplam, ortalama;
	toplam=sayi1+sayi2+sayi3;
	ortalama=toplam/3.0;
	return ortalama;
}
int main() {
	float a,b,c, ort;
	printf("3 tane sayi giriniz: ");
	scanf("%f%f%f",&a,&b,&c);
	ort = ortalama_bul(a,b,c);
	printf("sayilarin ortalamasi: %.2f", ort);

return 0;
}
```

```C
#include <stdio.h>

float ortalama_bul(float sayi1, float sayi2, float sayi3){
	return (sayi1+sayi2+sayi3)/3.0;
}

int main() {
	float a,b,c;
	printf("3 tane sayi giriniz: ");
	scanf("%f%f%f",&a,&b,&c);
	printf("sayilarin ortalamasi: %.2f", ortalama_bul(a,b,c));

return 0;
}
```

```C
#include <stdio.h>

float ortalama_bul(void){	
	float a,b,c;
	printf("3 tane sayi giriniz: ");
	scanf("%f%f%f",&a,&b,&c);	
	return (a+b+c)/3.0;
}
int main() {
	
	printf("sayilarin ortalamasi: %.2f", ortalama_bul());
	
	return 0;
}
```

```C
#include <stdio.h>

float ortalama_bul(void){	
	float a,b,c;
	printf("3 tane sayi giriniz: ");
	scanf("%f%f%f",&a,&b,&c);	
	return (a+b+c)/3.0;
}
int main() {
	int i;
	for(i=0;i<3;i++){
		printf("sayilarin ortalamasi: %.2f\n\n", ortalama_bul());
	}

return 0;
}
```

```C
#include <stdio.h>

int faktoriyel(int n){
	int i, sonuc=1;
	for(i=2;i<=n;i++)
		sonuc=sonuc*i;
	return sonuc;
}
int main() {
	
	printf("%d", faktoriyel(6));

return 0;
}
```

```C
#include <stdio.h>

int faktoriyel(int n){
	int i, sonuc=1;
	for(i=2;i<=n;i++)
		sonuc=sonuc*i;
	return sonuc;
}
int main() {
	
	int sayilar[5]={2,5,4,7,8};
	int i;
	for(i=0;i<5;i++)
		printf("%d! = %d\n",sayilar[i],faktoriyel(sayilar[i]));

return 0;
}
```

```C
#include <stdio.h>

int dizi_toplam(int dizi[], int boyut){
	
	int i, toplam=0;
	for(i=0;i<boyut;i++)
		toplam =  toplam + dizi[i];
	
	return  toplam;
}
int main() {
	
	int sayilar[]={2,5,4,7,8,10,12};
	printf("sayilar dizisindeki sayilarin toplami: %d",
										dizi_toplam(sayilar, 7));

return 0;
}
```

```C
#include <stdio.h>

int dizi_toplam(int dizi[], int boyut){
	
	int i, toplam=0;
	for(i=0;i<boyut;i++)
		toplam =  toplam + dizi[i];
	
	return  toplam;
}
int main() {
	
	int sayilar[]={2,5,4,7,8,10,12,12,15,8,1};
	printf("sayilar dizisindeki sayilarin toplami: %d",
				dizi_toplam(sayilar, sizeof(sayilar)/sizeof(int)));

return 0;
}
```

```C
#include <stdio.h>

void dizileri_topla(int dizi1[], int dizi2[],  int sonuc[], int n){	
	int i;
	for(i=0;i<n;i++)
		sonuc[i]=dizi1[i]+dizi2[i];	
}
int main() {
	int i;
	int sayilar1[]={2,5,4,7,8,10,12,12,15,8,1};
	int sayilar2[]={2,5,4,7,8,10,12,12,15,8,1};
	int toplam[11];
	dizileri_topla(sayilar1, sayilar2, toplam, 11);
	
	for(i=0;i<11;i++)
		printf("%d ",toplam[i]);

	return 0;
}
```


```C
#include <stdio.h>

int dizi_enbuyuk(int dizi[], int n){
	int eb,i;
	eb=dizi[0];
	for(i=0;i<n;i++)
		if(dizi[i]>eb)
			eb=dizi[i];
	return eb;
}
int main() {
	
	int a[]={2,3,111,7,4};
	printf("dizinin en buyuk elemani: %d", dizi_enbuyuk(a,5));

	return 0;
}
```