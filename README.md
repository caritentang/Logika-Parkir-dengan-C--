Logika-Parkir-dengan-C--
========================

Program Parkir dengan C++

#include<conio.h>              
#include<stdio.h>

void main ()
{
        float a,b,c,d;

        printf(" ----BIAYA PARKIR---- \n\n");
        printf("JAM MASUK \t= ");scanf("%f",&a);

	if (a<=24)
 	{
        printf("\nJAM KELUAR \t= ");scanf("%f",&b);

        if (b<=24)
        {
        		if (b>a)
        		{
                c=b-a;
                printf(" \nLAMA PARKIR = %.2f",c);
            }
            else if (b<a)
            {
                c=(24-a)+b;
                printf(" \nLAMA PARKIR = %.2f", c);
            }
        		if (c<=1)
          	{
            	d=5000;
            	printf(" \nBIAYA PARKIR = %.2f", d);
          	}
        		else if (c>1)
          	{
            	d=5000+(1000*(c-2));
            	printf(" \nBIAYA PARKIR = %.2f", d);
          	}
        		else
          	{
            	printf("\nMAAF ANDA SALAH");
          	}
        }
   }
   else                     
   {
        printf("\n\n\nMAAF ANDA SALAH MEMASUKAN JAM\n");
        printf("BATASAN WAKTU SAMPAI 24.00\n");
        printf("TERIMA KASIH");
    }
	getch();
}
