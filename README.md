#include <stdio.h>

void main(){

    int customersid, unitconsumed;
    
    float charge, surcharge=0, chargeamt, totalamt;
    
    printf("Input Customers ID :"); 
    
    scanf("%d",&customersid);
    
    printf("Input the unit consumed by the customer :");
    
    scanf("%d",&unitconsumed);
    
if (unitconsumed <199 )

	  charge = 1.50;
	  
	  
else	if (unitconsumed>=250 && unitconsumed<400)
		charge = 1.60;
		
else if (unitconsumed>=450 && unitconsumed<600)

	  charge = 1.85;
	  
else 
    charge = 2.0;
    
  
    chargeamt = unitconsumed*charge;
    
if (totalamt<400)

   surcharge = chargeamt*10/100.0;
   
   totalamt = chargeamt+surcharge;
   
if (totalamt  < 100)

	totalamt =100;
   
   printf("\n[Electricity Bill]\n");
   
   printf("Customer ID#                        :%d\n",customersid);
   
   printf("Unit Consumed                       :%d\n",unitconsumed);
   
   printf("Unit Charges @P%5.2f  per unit      :P%8.2f\n",charge,chargeamt);
   
   printf("Surchage Amount                     :P%8.2f\n",surcharge);
   
   printf("Total Customer Bill                 :P%8.2f\n",totalamt);

    return 0;
}
    
