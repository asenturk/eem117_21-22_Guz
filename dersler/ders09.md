```C
#include <stdio.h>

int main() {
	
	int x=0;
	
	while(x<15){
		printf("%d ",x);
		x += 4;
	}

return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int x=0;
	
	while( ++x < 5 ){
		printf("%d ",x);
		
	}

return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	printf("%d ", 1>0);
    printf("%d ", 0>0);

return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int x=5;
	
	while( x-- ){
		printf("%d ",x);
		
	}

return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int x=-5;
	
	while( x++ ){
		printf("%d ",x);
		
	}

return 0;
}
```



```C
#include <stdio.h>
#include <math.h>

int main() {
	
	int taban,us;
	printf("taban ve ussu giriniz: ");
	scanf("	%d%d",&taban, &us);
	
	printf("%d^%d=%.1f\n",taban,us,pow(taban,us));
	
	printf("%d^%d",taban,us);
	while(us>1){
		taban = taban * taban;
		us--;
	}
	printf("=%d",taban);	
	
	return 0;
}
```

```C
#include <stdio.h>
#include <math.h>

int main() {
	
	int taban,us,sonuc=1;
	printf("taban ve ussu giriniz: ");
	scanf("	%d%d",&taban, &us);
	
	printf("%d^%d=%.1f\n",taban,us,pow(taban,us));
	
	printf("%d^%d",taban,us);
	while(us-->0)
		sonuc = sonuc * taban;	

	printf("=%d",sonuc);	
	
	return 0;
}
```

```C
#include <stdio.h>
#include <math.h>

int main() {
	
	int taban,us,sonuc=1;
	printf("taban ve ussu giriniz: ");
	scanf("	%d%d",&taban, &us);
	
	printf("%d^%d=%.1f\n",taban,us,pow(taban,us));
	
	printf("%d^%d",taban,us);
	while(us--)
		sonuc = sonuc * taban;
		
	printf("=%d",sonuc);	
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int i,j;
	for(i=0;i<10;i++)
	for(j=0;j<10;j++){
		printf("%d ",j);
		break;
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,j;
	for(i=0;i<5;i++)
		for(j=0;j<5;j++){
			printf("%d ",j);	
		}
	
	return 0;
}
```


```C
#include <stdio.h>

int main() {
	
	int i,j;
	for(i=0;i<5;i++){
	for(j=0;j<5;j++)
		printf("%d ",j);	
	printf("\n");
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,j;
	for(i=0;i<5;i++){
	for(j=0;j<5;j++)
		printf("%d ",i);	
	printf("\n");
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,j;
	for(i=0;i<5;i++){
		for(j=0;j<5;j++){
			printf("%d ",j);
			if (i==j)
				break;
		}		
	printf("\n");
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,n=20;
	for(i=0;i<n;i++){
		if(i%5==0)
			continue;
		printf("%d ",i);
	
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,n=20;
	for(i=0;i<n;i++){
		if(i%5!=0)
			printf("%d ",i);
	
	}
	
	return 0;
}
```

```C
#include <stdio.h>

int main() {
printf("*\n**\n***\n****")	;
return 0;
}
```

```C
#include <stdio.h>

int main() {
	
	int i,j,n=6;
	
	for(i=0;i<n;i++){
	for(j=0;j<n;j++)
		if(j<=i)
			printf("*");
	printf("\n");
	}

	return 0;
}
```

```C
#include <stdio.h>


```C
#include <stdio.h>

int main() {
	
	int i,j,n=15;
	
	for(i=0;i<n;i++){
	for(j=0;j<n;j++)
		if(j<=i)
			printf("*");
		else
			break;	
    printf("\n");
	}

	return 0;
}
```
