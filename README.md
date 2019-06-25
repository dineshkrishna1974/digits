#include<stdio.h>
int main()
{
int i,digits[10]={10},reaminder;
long long int n;
scanf("%lld",&n);
while(n!=0)
{
reaminder = n % 10;
digits[reaminder]++;
n/=10;
}
for (i = 0; i<10; i++)
if ( digits[i]!=0)
printf("%d is present %d times\n",i, digits[i]);
return 0;
}
