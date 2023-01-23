### Write a C program to chea=ck the collinearity of three points if the co-ordinates are input through the keyboard 
#### Note :

```c
#include<stdio.h>
main(){
	float x1,x2,x3,y1,y2,y3;
	float s1,s2;
	printf("Please enter the coordinates of 1st point in 2D catesian system: ");
	scanf("%f %f",&x1,&y1);
	printf("2nd point : ");
	scanf("%f %f",&x2,&y2);
	printf("3rd point: ");
	scanf("%f %f",&x3,&y3);
	s1 = (y2 - y1)/(x2 - x1);
	s2 = (y3 - y2)/(x3 - x2);
	if(s1 == s2){
		printf("The three points lie on a same line .They are collinear");
	}
	else {
		printf("The three points do not lie on the same line .They are not collinear");
	}
}
```
