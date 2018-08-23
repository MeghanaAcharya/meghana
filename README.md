# meghana
#include<stdio.h>

int main() {
   printf("Blood Donation Application\n");
   int i=0;
   char email[100][100],name[100][100],group[100][100],address[100][100];
   char num[100][10];
   int age[100];
   while(1)
   {
       #ask user if wants to donate blood
       printf("If you want to donate blood press Y else press N\n");
       char ch;
       scanf("%c",&ch);
       if(ch=='N')
       {
           break;
       }
       else if(ch=='Y')
       {
           printf("Enter name\n");
           scanf("%s",name[i]);
           printf("Enter emailID\n");
           scanf("%s",email[i]);
           printf("Enter address");
           scanf("%s",address[i]);
           printf("Enter age");
           scanf("%d",age[i]);
           printf("Enter blood group");
           scanf("%s",group[i]);
           printf("Enter number");
           scanf("%s",num[i]);
           i++;
           
       }
       else
       {
           printf("Enter valid Key\n");
       }
   }
    for(int k=0;k<=i;k++)
   {
       printf("%s\n",name[k]);
       printf("%s\n",email[k]);
       printf("%s\n",address[k]);
       printf("%d\n",age[k]);
       printf("%s\n",group[k]);
       printf("%s\n",num[k]);
   }
   
}
