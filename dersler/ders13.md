```C
#include <stdio.h>
int main() {
	char a[100];
	printf("bir metin giriniz: ");
	//scanf("%s", a); 
	gets(a);
	printf("girilen metin: %s",a);
	
	return 0;
}
```

```C
#include <stdio.h>
int palindrom(char str[]){
	int uzunluk;
	int i;
	for(i=0;str[i]!='\0';i++);
	uzunluk=i;
	for(i=0;i<uzunluk;i++)
		if(str[i]!=str[uzunluk-1-i])
			return 0;
	return 1;	
}
int main() {
	char a[100];
	char ch;
	printf("metin giriniz: "); 
	gets(a);
	if(palindrom(a))
		printf("girilen metin palindromdur: %s",a);
	else
		printf("girilen metin palindrom degildir: %s",a);
	
	return 0;
}
```


```C
#include <stdio.h>
void birlestir(char kaynak1[], char kaynak2[],  char hedef[]){
	int i,j;
	for(i=0;kaynak1[i]!='\0';i++)
		hedef[i]=kaynak1[i];	
	for(j=0;kaynak2[j]!='\0';j++)
		hedef[i+j]=kaynak2[j];
	hedef[i+j]='\0';		
}
int main() {
	char a[100], b[100], c[200];
	
	printf("iki tane metin giriniz: "); 
	gets(a);
	gets(b);
	birlestir(a,b,c);
	printf("birlestirilen metin: %s",c);
	
	return 0;
}
```


```C
#include <stdio.h>
void buyuk_harfe_cevir(char kaynak[], char hedef[]){
	int i;
	for(i=0;kaynak[i]!='\0';i++){
		if(kaynak[i]>='a' && kaynak[i]<='z')
			hedef[i]=kaynak[i]-('a'-'A');
		else
			hedef[i]=kaynak[i];
	}
	hedef[i]='\0';
}
int main() {
	char a[100], b[100];
	
	printf("metin giriniz: "); 
	gets(a);
	
	buyuk_harfe_cevir(a, b);
	printf("BUYUK HARF: %s",b);
	
	return 0;
}
```


```C
#include <stdio.h>
int main() {
	char a[5][100];
	int i;
	for(i=0;i<5;i++){
		printf("metin giriniz: "); 
		gets(a[i]);
	}
	
	printf("girilen metinler: \n");
	for(i=0;i<5;i++)
		puts(a[i]);
	
	return 0;
}
```


```C
#include <stdio.h>
int ikiliden_on_tabanina(char ikili[]){
	int uzunluk, i;
	int ikinin_usleri=1;
	int sayi_10=0;
	for(i=0;ikili[i]!='\0';i++);
	uzunluk=i;
	
	for(i= uzunluk-1;i>=0;i--){
		if(ikili[i]=='1')
			sayi_10 = sayi_10 + ikinin_usleri;
		ikinin_usleri= ikinin_usleri*2;	
	}
	return sayi_10;
}
int main() {
	char sayi_2[100];
	int sayi_10;
	printf("iki tabaninda bir sayi giriniz: ");
	scanf("%s",sayi_2);
	sayi_10=ikiliden_on_tabanina(sayi_2);
	printf("%s sayisinin 10 tabanindaki karsiligi: %d",
						sayi_2, sayi_10);
	
	return 0;
}
```