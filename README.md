# Program-6D
C module 6
EX NO-6)D)Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary
DATE:20/10/25
NAME:JADE ADRINA J
REF NO:25017000
AIM: TO Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary
ALGORITHM:
1)define a structure .2)call the sturucture and take inputs from the user.3) print the data .4) calulate the gross salary(da =10% and HRA=30% from BP) .5) print the output using printf() function.
PROGRAM:
```
#include<stdio.h>
struct employee{int empno;char dept[50];float basic,gross,da,hra;};
int main(){
struct employee emp[3];int i;
for(i=0;i<3;i++){
scanf("%d",&emp[i].empno);
scanf("%s",emp[i].dept);
scanf("%f",&emp[i].basic);
emp[i].da=0.10*emp[i].basic;
emp[i].hra=0.30*emp[i].basic;
emp[i].gross=emp[i].basic+emp[i].da+emp[i].hra;
}
printf("Details of the Employee:\n");
for(i=0;i<3;i++){
printf("%d %s %.f %.f %.f %.2f\n",emp[i].empno,emp[i].dept,emp[i].basic,emp[i].basic/10,(emp[i].basic/10)*3,emp[i].gross);
}
```
OUTPUT:
<img width="1002" height="886" alt="Screenshot 2025-10-20 092641" src="https://github.com/user-attachments/assets/8121e1f4-f116-4dca-bc6a-311078a79362" />
RESULT:
thus,a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary has been executed successfully.

return 0;
}
