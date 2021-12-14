```C
#include <stdio.h>

int main() {
	int sayilar[5];
	sayilar[0]=5;
	sayilar[1]=10;
	sayilar[2]=15;
	sayilar[3]=20;
	sayilar[4]=25;
	printf("%d \n",sayilar[4]);
	printf("%d \n",sayilar[3]);
	printf("%d \n",sayilar[2]);
	printf("%d \n",sayilar[1]);
	printf("%d \n",sayilar[0]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[5],i;
	sayilar[0]=5;
	sayilar[1]=10;
	sayilar[2]=15;
	sayilar[3]=20;
	sayilar[4]=25;
	
	for(i=0;i<5;i++)
		printf("%d \n",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[5],i;
	sayilar[0]=5;
	sayilar[1]=10;
	sayilar[2]=15;
	sayilar[3]=20;
	sayilar[4]=25;
	
	for(i=0;i<5;i++)
		printf("%d ",sayilar[i]);
	printf("\n");
	for(i=4;i>=0;i--)
		printf("%d ",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[5]={5,10,15,20,25};
	int i;

for(i=0;i<5;i++)
		printf("%d ",sayilar[i]);
	printf("\n");
	for(i=4;i>=0;i--)
		printf("%d ",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[]={5,10,15,20,25};
	int i;

	printf("sayilar dizisinin bellekteki boyutu: %d\n",sizeof(sayilar));
	printf("sayilar dizisinin boyutu: %d\n",sizeof(sayilar)/sizeof(sayilar[0]));
	
	for(i=0;i<5;i++)
		printf("%d ",sayilar[i]);
	printf("\n");
	for(i=4;i>=0;i--)
		printf("%d ",sayilar[i]);

return 0;
}
```



```C
#include <stdio.h>

int main() {
	int sayilar[]={5,10,15,20,25,30};
	int i;
	int boyut;

	printf("sayilar dizisinin bellekteki boyutu: %d\n",sizeof(sayilar));
	printf("sayilar dizisinin boyutu: %d\n",sizeof(sayilar)/sizeof(sayilar[0]));
	boyut=sizeof(sayilar)/sizeof(sayilar[0]);
	for(i=0;i<boyut;i++)
		printf("%d ",sayilar[i]);
	printf("\n");
	for(i=boyut-1;i>=0;i--)
		printf("%d ",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[]={5,10,15,20,25,30,35,40,45};
	int i;
	int boyut;

	printf("sayilar dizisinin bellekteki boyutu: %d\n",sizeof(sayilar));
	printf("sayilar dizisinin boyutu: %d\n",sizeof(sayilar)/sizeof(sayilar[0]));
	boyut=sizeof(sayilar)/sizeof(sayilar[0]);
	for(i=0;i<boyut;i++)
		printf("%d ",sayilar[i]);
	printf("\n");
	for(i=boyut-1;i>=0;i--)
		printf("%d ",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[5];
	int i;
	for(i=0;i<5;i++){
		printf("%d. sayi:",i+1);
		scanf("%d",&sayilar[i]);
	}
	printf("\nveriler alindi\n");
	for(i=0;i<5;i++)
		printf("%d ",sayilar[i]);

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int sayilar[3][4];
	
	sayilar[0][0]=2;
	sayilar[0][5]=2;

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int matris[3][4];
	printf("matrisin degerlerini giriniz:\n");
	
	printf("1. satir, 1. sutun");
	scanf("%d",&matris[0][0]);
	
	printf("1. satir, 2. sutun");
	scanf("%d",&matris[0][1]);
	
	printf("1. satir, 3. sutun");
	scanf("%d",&matris[0][2]);
	
	printf("1. satir, 4. sutun");
	scanf("%d",&matris[0][3]);

	printf("2. satir, 1. sutun");
	scanf("%d",&matris[1][0]);
	
return 0;
}
```

```C
#include <stdio.h>

int main() {
	int matris[3][4];
	int i, j;
	printf("matrisin degerlerini giriniz:\n");
	
	for(i=0;i<3;i++)
		for(j=0;j<4;j++){
			printf("%d. satir, %d. sutun",i+1,j+1);
			scanf("%d",&matris[i][j]);	
		}

	for(i=0;i<3;i++){
		for(j=0;j<4;j++)
			printf("%d ",matris[i][j]);
		printf("\n");
	}
				
return 0;
}
```

```C
#include <stdio.h>

int main() {
	int matris[3][4];
	int i, j;
	printf("matrisin degerlerini giriniz:\n");
	
	for(i=0;i<3;i++)
		for(j=0;j<4;j++){
			printf("%d. satir, %d. sutun: ",i+1,j+1);
			scanf("%d",&matris[i][j]);	
		}

	for(i=0;i<3;i++){
		for(j=0;j<4;j++)
			printf("%d ",matris[i][j]);
		printf("\n");
	}
				
return 0;
}
```

```C
#include <stdio.h>

int main() {
	int matris[3][4];
	int i, j;
	printf("matrisin degerlerini giriniz:\n");
	
	for(i=0;i<3;i++)
		for(j=0;j<4;j++){
			printf("%d. satir, %d. sutun: ",i+1,j+1);
			scanf("%d",&matris[i][j]);	
		}

	for(i=0;i<3;i++){
		for(j=0;j<4;j++)
			printf("%3d ",matris[i][j]);
		printf("\n");
	}
				
return 0;
}
```

```C
#include <stdio.h>

int main() {
	int matris[3][4];
	int i, j;
	printf("matrisin degerlerini giriniz:\n");
	
	for(i=0;i<3;i++)
		for(j=0;j<4;j++){
			matris[i][j]=i*4+j;
		}

	for(i=0;i<3;i++){
		for(j=0;j<4;j++)
			printf("%3d ",matris[i][j]);
		printf("\n");
	}
				
			

return 0;
}
```

```C

#include <stdio.h>

int main() {
	int matris[][4]={{0,1,2,3},
					  {4,5,6,7},
					  {8,9,0,1}};
	int i, j;
	
	for(i=0;i<3;i++){
		for(j=0;j<4;j++)
			printf("%3d ",matris[i][j]);
		printf("\n");
	}			
			

return 0;
}
```

```C
#include <stdio.h>

int main() {
	int x[50];
	int i;
	int toplam=0;
	for(i=0;i<50;i++)
		scanf("%d",&x[i]);
	
	for(i=0;i<50;i++)
		toplam=toplam+x[i];
	
	printf("sayilarin toplami: %d",toplam);
		
return 0;
}
```

```C
#include <stdio.h>

int main() {
	int x[50];
	int i;
	int en_buyuk;
	for(i=0;i<50;i++)
		scanf("%d",&x[i]);
	
	en_buyuk=x[0];
	for(i=1;i<50;i++)
		if(x[i]>en_buyuk)
			en_buyuk=x[i];		
	
	printf("en buyuk sayi: %d",en_buyuk);
			
return 0;
}
```

```C
#include <stdio.h>
#define N 400

int main() {
	int x[N];
	int i;
	int en_buyuk;
	for(i=0;i<N;i++)
		scanf("%d",&x[i]);
	
	en_buyuk=x[0];
	for(i=1;i<N;i++)
		if(x[i]>en_buyuk)
			en_buyuk=x[i];
		
	printf("en buyuk sayi: %d",en_buyuk);
		
return 0;
}
```