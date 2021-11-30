```C
#include <stdio.h>

int main() {

	int i;
	for(i=0; i<10; i++)
		printf("%d ",i);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	int i;
	for(i=0; i<10; i++)
		printf("%d ",i);
	printf("\n");
	
	i=0;
	while(i<10){
		printf("%d ",i);
		i++;
	}
	printf("\n");
	
	i=1;
	do{
		printf("%d ",i);
		i++;
	}while(i<10);
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {

	int i;
	for(i=0; i<10; i++)
		printf("%d ",i);
	printf("\n");
	
	i=0;
	while(i<10){
		printf("%d ",i);
		i++;
	}
	printf("\n");
	
	i=10;
	do{
		printf("%d ",i);
		i++;
	}while(i<10)
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	int sayi, toplam=0, i;
	for(i=0;i<10;i++){
		printf("%d. sayiyi giriniz: ",i+1);
		scanf("%d",&sayi);
		toplam=toplam+sayi;
	}
	printf("sayilarin toplami: %d", toplam);
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	//girilen sayi pozitif ve 0 oldugu surece
	//sayilari toplayan
	// negatif sayi girildiginde toplam ve 
	// ortalamayi bulan program
	
	int sayi, toplam=0, i=0;
	float ortalama;
	
	printf("sayi giriniz: ");
	scanf("%d", &sayi);
	while(sayi>=0){
		toplam = toplam + sayi;
		i++;
		printf("sayi giriniz: ");
		scanf("%d", &sayi);	
	}
	
	printf("%d sayi girildi\n",i);
	printf("girilen sayilarin toplami: %d",toplam);
	
	ortalama=(toplam*1.0)/i;
	printf("girilen sayilarin ortalamasi: %.2f", ortalama);
	
	return 0;
}
```



```C
#include <stdio.h>

int main() {

	// n! bulan program
	int fakt=1, n;
	printf("n yi giriniz: ");
	scanf("%d",&n);
	while(n>1){
		fakt = fakt * n;
		n--;
	}
	printf("%d! = %d",n, fakt);
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {

	// n! bulan program
	int fakt=1, n;
	printf("n yi giriniz: ");
	scanf("%d",&n);
	printf("%d! = ",n);
	while(n>1){
		fakt = fakt * n;
		n--;
	}
	printf("%d",n, fakt);
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {

	// n! bulan program
	int fakt=1, n;
	printf("n yi giriniz: ");
	scanf("%d",&n);
	printf("%d! = ",n);
	while(n>1){
		fakt = fakt * n;
		n--;
	}
	printf("%d\n", fakt);
	printf("n yi giriniz: ");
	scanf("%d",&n);
	printf("%d! = ",n);
	for(fakt=1 ; n>1; n--){
		fakt = fakt * n;
	}
	printf("%d", fakt);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	// bir sayinin kendinden kucuk
	// en buyuk bolenini bulan program
	int sayi, ebb, i;
	printf("sayiyi giriniz: ");
	scanf("%d",&sayi);
	for(i=1;i<sayi;i++)
		if(sayi%i==0)
			ebb=i;
	printf("%d sayisinin ebb: %d", sayi, ebb);
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {

	// bir sayinin kendinden kucuk
	// en buyuk bolenini bulan program
	int sayi, ebb, i;
	printf("sayiyi giriniz: ");
	scanf("%d",&sayi);
	for(i=1;i<sayi;i++)
		if(sayi%i==0)
			ebb=i;
	printf("%d sayisinin ebb: %d\n", sayi, ebb);
	
	i=1;
	while(sayi>i){
		if(sayi%i==0)
			ebb=i;
		i++;
	}
	printf("%d sayisinin ebb: %d\n", sayi, ebb);
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {

	// ebob
	int sayi1, sayi2, ebb, i;
	printf("2 sayiyi giriniz: ");
	scanf("%d%d",&sayi1,&sayi2);
	i=1;
	while(sayi1>=i && sayi2>=i){
		if(sayi1%i==0 && sayi2%i==0)
			ebb=i;
		i++;
	}
	printf("%d ve %d sayisinin ebb: %d\n", sayi1, sayi2, ebb);
	
	return 0;
}
```



```C
#include <stdio.h>

int main() {

	int sayi, i;
	printf("sayi giriniz: ");
	scanf("%d",&sayi);
	for(i=2;i<sayi;i++)
		if(sayi%i==0){
			printf("sayi asal degildir.\n");
			break;
		}
	printf("%d sayisini %d sayisi boler",sayi,i);
	
	return 0;
}
```




```C
#include <stdio.h>

int main() {

	int sayi, i;
	printf("sayi giriniz: ");
	scanf("%d",&sayi);
	for(i=2;i<sayi;i++)
		if(sayi%i==0){
			printf("sayi asal degildir.\n");
			break;
		}
	if(sayi==i)
		printf("%d sayisi asaldir.", sayi);
	else
		printf("%d sayisini %d sayisi boler",sayi,i);
	
	return 0;
}
```




```C
#include <stdio.h>

int main() {

	// bir sayinin kendinden kucuk
	//en buyuk bolenini bulan program
	int sayi, i, j;
	printf("sayi giriniz: ");
	scanf("%d",&sayi);
	for(i=0; i<=sayi; i++){
		for(j=0; j<=sayi; j++)
			printf("%3d",i*j);
		printf("\n");
	}
	
	return 0;
}
```




```C
#include <stdio.h>

int main() {

	// carpim tablosu
	int sayi, i, j;
	printf("sayi giriniz: ");
	scanf("%d",&sayi);
	for(i=0; i<=sayi; i++){
		for(j=0; j<=sayi; j++)
			printf("%5d",i*j);
		printf("\n");
	}
	
	return 0;
}
```