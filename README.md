#include<stdio.h>
void
main ()
{
  int a[] = { 1, 0, 1, 0, 1, 0, 0, 1 }, i, j, temp;
  for (i = 0; i < 8; i++)
    {
      for (j = i + 1; j < 8; j++)
	{
	  if (a[i] < a[j])
	    {
	      temp = a[i];
	      a[i] = a[j];
	      a[j] = temp;
	    }
	}
    }
    for(i=0;i<8;i++)
    {
       printf ("%d\t", a[i]);
     }
}
