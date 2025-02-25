#include<stdio.h>
#include<math.h>
int main()
{
	double a,b,c,d,e,x,w1,w2,w3,w4,w5;
	scanf("%lf",&x);
	a=0.015;
	b=0.021;
	c=0.0275;
	d=0.03;
	e=0.0035/4;
	w1=x+x*d*5;
	w2=x+x*b*2+(x+x*b*2)*c*3;
	w3=x+x*c*3+(x+x*c*3)*b*2;
	w4=x*pow(1+a,5);
	w5=x*pow(1+e,20);
	printf("%f ",w1);
	printf("%f ",w2);
	printf("%f ",w3);
	printf("%f ",w4);
	printf("%f",w5);
	return 0;
}
