 C- programming Assignments 
   
1 wap to determine the input number is divisible by 5 or not 
#include<stdio.h>
#include<conio.h>
int main(){
 int num;
 printf("Enter any number = ");
 scanf("%d",&num);
 if (num%5==0)
 {
    printf("It is  divisible by 5");
 }
 else
 {  
    printf("It cannot divisible by 5");
}
 
return 0;
}

2 To check the input number is odd or even

#include<stdio.h>
#include<conio.h>
int main()
{
 int num;
 printf("Enter any number= ");
 scanf("%d",&num);
 if (num%2==0)
 {
   printf("Enter number  is Even");
 }
 else
 {
   printf("Enter number is Odd");
 }
 
   return 0;
}
3  To find the greatest number amoung two number

#include<stdio.h>
#include<conio.h>
int main(){
 int a,b;
 printf("Enter any number a = ");
 scanf("%d",&a);
 printf("Enter another number b= ");
 scanf("%d",&b);
 if (a>b)
 {
  printf("Entered number a i.e %d is greatest",a);
 }
 else{
  printf("Entered number b i.e %d is greatest",b);
 }
  return 0;
}

4 finding the greatest number amoung given three number using if conditional statement

#include<stdio.h>
#include<conio.h>
int main()
{ int a,b,c;
printf("Enter any three number a,b and c= ");
scanf("%d%d%d",&a,&b,&c);
if (a>b)
{    
    if (a>c)
{
    printf("a is the greatest number");
}
 }
if (b>a)
{
    if (b>c)
    {
        printf("b is the greatest number amoung three");
    }
}
else
    {
        printf("c is the greatest number ");
    }

   return 0;
}

5 To check whether the input year is leap or not

#include<stdio.h>
int main(){
 int year;
 printf("Enter any year= ");
 scanf(" %d",&year);
 if ((year%4==0 && year%100!=0) || year%400==0)
 {
  printf("The enter year %d is Leap year",year);
 }
 else{
  printf("Enter year %d is not Leap year",year);
 }
 return 0;
}

6 to determine the enter character is Uppercase,Lowercase , digit or a special one.

#include<stdio.h>
#include<conio.h>
int main()
{
  char character;
 printf("Enter any character= ");
 scanf("%c",&character);
 if (character>='A' && character<='Z')
 {
  printf("Enter character is Uppercase Alphabate");
 }
  else if (  character>= 'a' && character <= 'z' ) 
 {
 printf("Enter character is Lowercase alphabet");
 }
 else if (character>= '0' && character<='9')
 {
  printf("Enter character is   numberic ");
 }
 else
 {
  printf("Enter character is special ");
 }
  return 0;
}

7  to enter the side of triangle to find whether the triangle is valid or not 
#include<stdio.h>
#include<conio.h>
int main()
{ int a,b,c;
printf("Enter side of triangle a and b = ");
scanf("%d%d",&a,&b);
printf("Enter the largest side= ");
scanf("%d",&c);
if (a+b>c)
{
  printf("The triangle is valid");
}
else
{
  printf("sorry this is not a triangle");
}
  return 0; 
 }

8  to find the percentage got by student with grade  if he score more than 40 or passed in all subject

#include<stdio.h>
#include<conio.h>
int main()
{
float first,second,third,fourth,fifth,total,percentage;
printf("Enter mark obtained by a student in first,second,third,fourth and fifth subject= ");
scanf("%f%f%f%f%f",&first,&second,&third,&fourth,&fifth);
total=first+second+third+fourth+fifth;
percentage=(total/(5*100))*100;
printf("Total mark he/she obtained is= %.2f\n",total);
printf("He/she get about = %.2f %%\n", percentage);
if (first>=40 && second>=40 && third>=40 && fourth>=40 && fifth>=40)
{
 printf(" Result= Congratulations! Passed\n");
}
else
{
 printf(" Result= Sorry failed\n");
 return ;
}
if (percentage>=80)
{
  printf("Distinction");
}
else if (percentage>=70 && percentage<80)
{
  printf("First Division");
}
else if ( percentage>=60 && percentage<70)
{
  printf("Second Division");
}
else if (percentage>=50 && percentage<60)
{
 printf("Third Division");
}
else if ( percentage>=40 && percentage< 50)
{
  printf("Pass Division");
}
else
{
  printf("Fail");
}
return 0;
} 

9 Finding the day name with input number

#include<stdio.h>
#include<conio.h>
int main(){
  int num;
  printf("enter any number= ");
  scanf("%d",&num);
  using if statement
  if (num==1)
  {
    printf("Sunday");
  }
  if (num==2)
  {
    printf("Monday");
  }
  if (num==3)
  {
    printf("Tuesday");
  }
  if (num==4)
  {
    printf("Wednesday");
  }
  if (num==5)
  {
    printf("Thursday");
  }
  if (num==6)
  {
    printf("Friday");
  }
  if (num==7)
  {
    printf("Saturday");
  }
  if (num>7)
  {
  printf("Invalid day number");
  }
  return 0;
}
  using if----else statement
  if (num==1)
  {
    printf("Sunday");
  }
  else if (num==2)
  {
    printf("Monday");
  }
  else if (num==3)
  {
    printf("Tuesdy");
  }
  else if (num==4)
  {
    printf("Wednesday");
  }
  else if (num==5)
  {
    printf("Thursday");
  }
  else if (num==6)
  {
    printf("Friday");
  }
  else if (num==7) 
  { 
    printf("Saturday");
  }
   else
   {
    printf("Invalid day number");
   }

   Using switch statements
switch (num)
{
case 1:
printf("Sunday");
break;
case 2:
printf("Monday");
break;
case 3:
printf("Tuesday");
break;
case 4:
printf("wednesday");
break;
case 5:
printf("Thursday");
break;
case 6:
printf("Friday");
break;
case 7:
printf("Saturday");
break;
default:
printf("Invalid day number");
break;
}
return 0; 
}

10 teenager as well as middle age

#include<stdio.h>
#include<conio.h>
int main(){
  int age;
  printf("Enter age of the person= ");
  scanf("%d",&age);
  if (age>0 && age<16)
  {
    printf("He is teenager");
  }
  else if (age>16)
  {
    printf("He is not teenager");
  }
  else
  {
    printf("He is teenager as well as middle age of teenager");

  }
  return 0;
}

11 to find the area ,rectangle , triangle

#include<stdio.h>
#include<conio.h>
#define pi 3.1415
int main()
{ 
  int n;
   
printf("Enter 1 for rectangle 2 for circle and 3 for area of triangle : ");
scanf(" %d",&n);
switch (n)
{
case 1: 
   { int l,b,area;
  printf("Enter length of rectangle= ");
  scanf("%d",&l);
  printf("Enter breadth of rectangle= ");
  scanf("%d",&b);
  area=l*b;
  printf("Area of rectangle =%d sq meter",area); }

  break;
  case 2:
  { int r,area_circle;
  printf("Enter radious of circle= ");
  scanf("%d",&r);
  area_circle= pi*r*r;
  printf("Enter area of circle: %d sq meter",area_circle);
  }
  break;
  case 3:
  { 
    int base,height,area_triangle;
  printf("Enter base of triangle= ");
  scanf("%d",&base);
  printf("Enter height of triangle= ");
  scanf("%d",&height);
  area_triangle=(base*height)/2;
  printf("Area of triangle=%d sq meter",area_triangle);
break;
 }
 default: printf("Invalid Number");
 break;
}
return 0;
}

12  to find the given number is palidrome or not

#include<stdio.h>
#include<conio.h>
int main(){
 int n,num,reverse=0;
 printf("Enter any number to check whether the numbr is Palindrome or not= ");
 scanf("%d",&n);
 num=n;
 while (n!=0)
 {
reverse=(reverse*10)+(n%10);
n /=10;
 }
 if (reverse==num)
 {
  printf("The input number  is palindrome");
 }
 else
 {
  printf("Enter number is not palindome");
 }
  return 0;
}

13 to check whether the input any alphabet is vowel or not

#include<stdio.h>
#include<conio.h>
int main(){
char letter;
printf("Enter any letter= ");
scanf("%c",&letter);
if (letter=='a' || letter=='e' || letter=='i' || letter=='o' || letter=='u')
{
  printf("Input letter or character is vowel");
}
else if (letter=='A' || letter=='E' || letter=='I' || letter=='O' || letter=='U')
{
printf("Input letter or character is vowel");
}
else if (letter>='0' && letter<='9')
{
 printf("Invlid letter");
}
else
{
  printf("Enter character or letter is consonant");
}
return 0;
}

14 to selecting drivers based on provided datas

#include<stdio.h>
#include<conio.h>
int main()
{ int age;
 char gender,maritalstatus;
 printf("Enter age of a person = ");
 scanf(" %d",&age);
 printf("Enter gender of person(M/F)= ");
 scanf(" %c",&gender);
 printf("Enter marital status of person(M/U)= ");
 scanf(" %c",&maritalstatus);
 if ( (age>30) &&(  gender=='M' || gender=='m' ) && ( maritalstatus=='U' || maritalstatus=='u'))
 {
  printf("you are insured  in our company driving job");
 }
 
 else if (age>25 && gender=='F' || gender=='f' && maritalstatus=='U' || maritalstatus=='u')
{
printf("You are insured for company  driving job ");
}
else if (maritalstatus=='M' || maritalstatus=='m')
 {
 printf("You are insured for our company driving job");
 }
else
{
  printf("Sorry not insured");
}
  return 0;
}

15 to find the absolute value of the given number 
#include<stdio.h>
#include<conio.h>
int main()
{ int number;
printf("Enter any number= ");
scanf(" %d",&number);
if (number<0)
{
  number=-number;
  printf("The absolute value of the entered number is: %d",number);
}
else
{
  printf("The absolute value of number is:%d",number);
}

  return 0;
}
 16 to use switch case and printf the output as given
#include<stdio.h>
#include<conio.h>
int main()
{ char character;
printf("Enter any character= ");
scanf("%c",&character);
switch (character)
{
case'a':
case 'A':printf("appleAPPLE");
  break;
  case'b':
  case'B':printf("ballBALL");
  break;
  case'c':
  case'C':printf("catCAT");
  break;
  default:printf("helloHELLO");
  break;
}
  return 0;
}
// this is the c-programming 


WAP to print hello world 
#include<stdio.h>
#include<conio.h>
int main()
{
printf("Hello World");
    return 0;
}
2 WAP To find the addition of two number 
 #include<stdio.h>
#include<conio.h>
int main()
{ int a=3;
 int b=2;
 int sum;
 sum=a+b;
printf("sum of a and b is =%d",sum);
    return 0;
}
 3 WAP to inatilize int , float and char 
#include<stdio.h>
#include<conio.h>
int main()
{ int a=4;
 float b=5;
 char x='A';
 printf("The value of int is=%d\n",a);
printf("The value of float is=%f\n",b);
printf("The value of char is=%c\n",x);
    return 0;
}
 to find are and the pereimeter using length and the breadth of the rectangle 
 #include<stdio.h>
#include<conio.h>
int main()
{ 
    int l,b,area,perimeter;
printf("Enter length of rectangle=");
scanf("%d",&l);
printf("Enter breadth of rectangle=");
scanf("%d",&b);
area=l*b;
perimeter=2*(l+b);
printf("The area of rectangle is=%d\n",area);
printf("The perimeter of reactangle is=%d\n",perimeter);
return 0;
}
 5 wap to to convert centigrate teimp to faranhit 
#include<stdio.h>
#include<conio.h>
int main(){
 float temp,result;
 printf("Enter temperature in centigrate= ");
 scanf("%f",&temp);
 result= (temp*9/5)+32;
 printf("Temperature in fahrenheit is=%f",result);
 return 0;
}
 to calculate area adn the circumference of circle 
 #include<stdio.h>
#include<conio.h>
int main(){
 int r;
 float area;
 float circumference;
 printf("Enter radious of circle= ");
 scanf("%d",&r);
 area=3.1415*r*r;
  circumference=2*3.1415*r;
 printf("area of circle is =%f\n",area);
 printf("circumference of circle is =%f\n",circumference);
 return 0;
} 
#include<stdio.h>
#include<conio.h>
int main(){
 int p,t,r,SI;
 printf("Enter priciple,time in year,rate= ");
 scanf("%d%d%d",&p,&t,&r);
 SI=(p*t*r)/100;
 printf("Simple Intrest is =%d",SI);
 return 0;
}
to find sum and the average of three number 
#include<stdio.h>
#include<conio.h>
int main(){
 int a,b,c,sum;
 float average;
 printf("Enter three number a,b,c= ");
 scanf("%d%d%d",&a,&b,&c);
 sum=a+b+c;
 average=(a+b+c)/3;
 printf("Sum of three numbear is =%d\n",sum);
 printf("average of three numbear is =%f\n",average);
 return 0;
}
to find the square of any number
#include<stdio.h>
#include<conio.h>
int main(){
 int a,square;
 printf("Enter any number = ");
 scanf("%d",&a);
 square=a*a;
 printf("sqaure of number is =%d\n",square);
 return 0;
}
// to find the cube of any number
#include<stdio.h>
#include<conio.h>
int main(){
 int num,cube;
 printf("Enter any num = ");
 scanf("%d",&num);
 cube=num*num*num;
 printf("cube of number  is =%d\n",cube);
 return 0;
}
to find percentage 11
 #include<stdio.h>
#include<conio.h>
 int main(){
 int math,physics,english,nepali,computer,Total;
 float percentge;
 printf("enter mark  student in math= ");
 scanf("%d",&math );
 printf("mark  in physics= ");
 scanf("%d",&physics);
 printf(" mark  in english= ");
 scanf("%d",&english);
 printf(" mark  in nepali= ");
 scanf("%d",&nepali);
 printf(" mark  in computer= ");
 scanf("%d",&computer);
 Total=(math+physics+english+nepali+computer);
 percentge = (float)Total / (5 * 100) * 100;
 printf("total mark got by student is=%d\n",Total);
 printf("total percent got by a student is=% .2f",percentge);
  return 0;
} 

12 wap to pre process directives 
#include<stdio.h>
#define PI 3.1415
int main(){
    int r;
    float area,circumference;
    printf("input radious of circle= ");
    scanf("%d",&r);
    area= PI*r*r;
    circumference=2*PI*r;
    printf("the area of circle is=%f\n",area);
    printf("circumference of circle is=%f\n",circumference);
    return 0;
}
    returthis is another way 
#include<stdio.h>
 main()
{
	float circumference;
	float rad
	printf("Enter the radius of the Circle:\t");
	scanf("%f", &radi
 	circumference = 2 * PI * radius;

 	printf("circumference is= %f",circumference);
 }
 to find square root of the number using library function
 #include<math.h>
 #include<stdio.h>
 int main(){ 
  int a,squareroot;
  printf("Enter any number= ");
  scanf("%d",&a);
  squareroot=sqrt(a);
  printf("The square root of the number is=%d",squareroot);
     return 0;
 }
 absolute value of 14
 #include<stdio.h>
 #include<stdlib.h>
 int main(){ 
  int a,value;
  printf("Enter any number= ");
  scanf("%d",&a);
  value= abs(a);
  printf("The absolute value of the  number is=%d",value);
     return 0;
 }
15 cube root using library function
 #include<math.h>
 #include<stdio.h>
 int main(){ 
  int a,cuberoot;
  printf("Enter any number= ");
  scanf("%d",&a);
  cuberoot=cbrt(a);
  printf("The square root of the number is=%d",cuberoot);
     return 0;
 }
                      //cube surface area 
 #include <stdio.h>
 #include<conio.h>
 int main() {
     float side, surfaceArea;
     printf("Enter the side length of the cube: ");
     scanf("%f", &side);
     surfaceArea = 6 * side * side;
     printf("The surface area of the cube with side %.2f is: %.2f\n", side, surfaceArea);
     return 0;
 }
  input any two number and interchange content
 
 #include<stdio.h>
 #include<conio.h>
 int main(){
 int a,b,c;
 printf("Enter number a= ");
 scanf("%d",&a);
 printf("Enter number b= ");
 scanf("%d",&b);
 c=a;
 a=b;
 b=c;
 printf("The value of a is= %d\n ",a);
 printf("The valur of b is= %d\n",b);
 return 0;
 }
//  to print the volume of sphere 4/3 pie r^3
 #include<stdio.h>
 #include<conio.h>
 #define pi 3.1415
 int main(){
 int radious;
 float volume;
 printf("Enter the radious of the sphere= ");
 scanf("%d",&radious);
 volume=((4*pi)*radious*radious*radious)/3;
 printf("The volume of the sphere of  is=%f",volume);
     return 0;
 }
19 wap to add, sub , multidy and div of two input number 
 #include<stdio.h>
 #include<conio.h>
 int main(){
  int a,b,sum,sub,multi;
  float div;
  printf("Enter value of number a and b= ");
  scanf("%d%d",&a,&b);
  sum=a+b;
  sub=a-b;
  div=a/b;
  multi=a*b;
  printf("Addition of two number is=%d\n",sum);
  printf("Subtraction of two number is=%d\n",sub);
  printf(" Multiplication  of two number is=%d\n",multi);
  printf("Division of two number is=%.2f\n",div);
     return 0;
 }

  20 to input thre digit number and also find the sum of the digits

 #include <stdio.h>
 int main() {
     int number, digit1, digit2, digit3, sum;
     printf("Enter a three-digit number: ");
     scanf("%d", &number);
     digit1 = number / 100;      // Extract hundreds place digit ths is important formulas
     digit2 = (number / 10) % 10; // Extract tens place digit
     digit3 = number % 10;       // Extract ones place digit
     sum = digit1 + digit2 + digit3;
     // Display the result
     printf("Individual digits: %d, %d, %d\n", digit1, digit2, digit3);
     printf("Sum of individual digits: %d\n", sum);
     return 0;
 }
//  21 this is  first  and last digit sum of idividuals 
 #include <stdio.h>
 int main() {
     int number, digit1, digit2, digit3, sum;
     printf("Enter a three-digit number: ");
     scanf("%d", &number);
     digit1 = number / 100;     // hundreds place digit ths is important formulas
      digit3 = number%10;                           // don't need 2nd number     digit3 = number % 10;       // Extract ones place digit
     sum = digit1 + digit3;    // Display the result     printf("Individual digits: %d, %d\n", digit1, digit3);
     printf("Sum of individual digits: %d\n", sum );
         return 0;
      }
      
     // same trick is applied to digits questions

//22 right one reverst the input number
 #include<stdio.h>
 int main(){
     int number,digit1,digit2,digit3;
     printf("Input ant three-digit number= ");
     scanf("%d",&number);
     digit1=number%10;
     digit2=(number/10)%10;
     digit3=number/100;
     printf("The input number is= %d\n",number);
     printf("Before reverse number is =%d%d%d\n",digit3,digit2,digit1);
     printf("After reverse number is =%d%d%d\n",digit1,digit2,digit3);
 return 0;
 }



 
  enter number and find the sum of the 4 digits
 
 #include <stdio.h> 
 int main() {
     int number, digit1, digit2, digit3,digit4, sum;
     printf("Enter a four-digit number: ");
     scanf("%d", &number);
     digit1 = number / 1000;       // thousands place digit ths is important formulas
     digit2 = (number / 100) % 10; //hundreds place digit
     digit3 = (number / 10)%10;    // tens place digit  
     digit4 = number %10;      // ones place digit
     sum = digit1 + digit2 + digit3+digit4;   
     printf("Individual digits: %d, %d, %d,%d\n", digit1, digit2, digit3,digit4);
     printf("Sum of individual digits: %d\n", sum);   
       return 0;
 }

 // Questions number 24 digits sum of first , third and last
 
 #include <stdio.h>
 int main() {
     int number, digit1, digit2, digit3,digit4, sum;
     printf("Enter a three-digit number: ");
     scanf("%d", &number);
     digit1 = number / 1000;     // Extract thousands place digit ths is important formulas
     digit2 =(number/100)%10;              //            replace 2nd number 
     digit3 = (number / 10)%10;    //Extract tens place digit  
     digit4 = number %10;     // Extract ones place digit
     sum = digit1 +  digit3+digit4;
     //Display the result
     printf("Individual digits of digit1,digit3 and digit4: %d, %d,%d\n", digit1,digit3,digit4);
     printf("Sum of individual digits: %d\n", sum);
     return 0;
 }
// 25 number to display the following
 #include<stdio.h>
 int main()
 {
     printf("\n");
 printf("***************\n");
 printf("\n");
 printf("Name: Ram\n");
 printf("\n");
 printf("Age: 34\n");
 printf("\n");
 printf("Gender: Male \t  \t Address:Kathmandu\n");
 printf("\n");
 printf("***************");
    return 0;
 }
   //Number 26
 #include<stdio.h>
 int main()
 {
     float basicSalary,dearnessallowances,housing,grosssalay;
     printf("Enter the basic salary of Rajesh= ");
     scanf("%f",&basicSalary);
     dearnessallowances = 0.4*basicSalary;
     housing = 0.2*basicSalary;
     grosssalay = basicSalary + dearnessallowances + housing;
     printf("The basic salary is= %.3f\n",basicSalary);
     printf("The dearness allowance amount is =%.2f\n",dearnessallowances);
     printf("The housing allowances is =%.2f\n",housing);
     printf("The total gross salary is =%.2f\n",grosssalay);
     return 0;
 }
 Gets and Puts 
 #include<stdio.h>
int main()
{
 char ch;
 printf("Enter any character= ");
 scanf("%c",&ch);
printf(" value of enter character %c is  %d", ch,ch);
    return 0;
}



to input single value and print single value 
#include<stdio.h>
int main()
{ 
  char ch;
printf("Enter any character= ");
ch=getchar();
putchar(ch);
    return 0;
}

single character input and output  using gets and puts
#include<stdio.h>
int main()
{ char ch[6];
printf("Enter any  string = ");
gets(ch);
printf("The string you enter is:");
puts(ch);
    return 0;
}

// conversation specifications in c 
#include<stdio.h>
int main()
{ 
int a=260, b, x=65,z, intsum;
float c=3.1415, intval1=98.54, intval2=45.34;
char ch='A';
b=(int)c;
ch=(int)c;
a=(float)ch;
z=(char)x;
printf("b become using explicit conversion is=%d\n ",b);
printf("ch become using explicit conversion is=%c\n ",ch);
printf("a value become using explict conversion is=%d\n",a);
printf("z value become using explict conversion is=%c\n",z);
intsum=intval1+intval2;
printf("this is the example of implicit conversion=%d", intsum);
    return 0;
}
#include<stdio.h>
int main()
{
 char ch;
 printf("Enter any character= ");
 scanf("%c",&ch);
printf("ASCII value of enter character %c is  %d", ch,ch);
    return 0;
}


// to find the natural number between 100 - 200 with some contitons
#include<stdio.h>
int main()
{ 
    int i=101, n=200,b,count,sum=0;
 for(i=101; i<200; i++)
 {   b=i/7;
    if (i%7==0 && i/7!=0)
    { 
      printf("%d\n ",i);  
    sum+=i;
    n/=10;
    count++;
}
}  
   printf("Total number divisible by 7 between 100 -200 are=%d\n",count);
   printf("sum of all divisible numbers are =%d\n",sum);
    return 0;
}

 // list og all types of asignment 
 // this is another c program project
1 to print number less than 100 using for loop , do while and while loop 
#include<stdio.h>
int main()
{
 int i=1,n=100;
 for(i=1; i<=100; i++)
 {
    printf("%d ", i);
 }
//using do while
 while (i<=n)
 {
    printf("%d ", i);
    i++;
 }
 return 0;
}

do
{
 printf("%d ",i);
 i++;
} 
while (i<=n);
return 0;
}

2. to find the even numbers from 1 to n
#include<stdio.h>
int main()
{ 
   int n,i=2;
printf("Enter the number to find up to even= ");
scanf("%d",&n);
for ( i = 2; i < n; i+=2)
{
  printf("%d ",i);
}
do while
do
{ 
  printf("%d ",i);
  i+=2;
while (i<n)
}
while
while (i<n)
{
   printf("%d ",i);
   i+=2;
}
   return 0;
}

3 to display odd number from 1 to n
#include<stdio.h>
int main()
{ 
   int n,i=1;
printf("Enter the number to find up to even= ");
scanf("%d",&n);
for ( i = 1; i < n; i+=2)
{
  printf("%d ",i);
}
do while
do
{ 
  printf("%d ",i);
  i+=2;
}
while (i<n)
while using 
while (i<n)
{
   printf("%d ",i);
   i+=2;
}
   return 0;
}

4. to display first 10 odd numbers 
#include<stdio.h>
int main()
{ int i=1;
for ( i = 1; i <=10; i++)
{
   printf("%d ",2*i-1);
}
do{
   printf("%d ",2*i-1);
   i++;
}
while(i<=10);
while(i<=10)
{ 
   printf("%d ",2*i-1);
   i++;
}
return 0;
}

5. to find sum of first n natural numbers 
#include<stdio.h>
int main()
{ int i=1,n,sum=0;
printf("Enter number= ");
scanf("%d",&n);
for ( i = 1; i <=n; i++)
{
printf("%d ",i);
sum+=i;
}
while 
while (i<=n)
{
printf("%d ",i);
sum+=i;
i++;
}
printf("\nThe sum is= %d",sum);
do while loop 
do
{
printf("%d ",i);
sum+=i;
i++;
}
while (i<=n);
printf("\nThe sum is= %d",sum);
return 0;
}

6. to find the sum of the even number from 1 to n 
#include<stdio.h>
int main()
{ int i=2,n,sum=0;
printf("Enter any number= ");
scanf("%d",&n);
for ( i = 2; i <=n; i+=2)
{
   printf("%d ",i);
   sum+=i;
}
printf("\nThe sum of the even numbers is = %d", sum);
   return 0;
}

7. Sum of odd numbers from 1 to n 
#include<stdio.h>
int main()
{ int i=1,n,sum=0;
printf("Enter any number= ");
scanf("%d",&n);
for ( i = 1; i <=n; i+=2)
{
   printf("%d ",i);
   sum+=i;
}
printf("\nThe sum of the odd numbers is = %d", sum);
   return 0;
}

8. to find the factorial of any input number 
#include<stdio.h>
int main()
{ int n,factorial=1;
printf("Enter any number= ");
scanf("%d",&n);
for (int i = 1; i <=n; i++)
{
   factorial*=i;
}
printf("Factorial of number %d is = %d",n,factorial);
   return 0;
}

9. To print the multiplication table
#include<stdio.h>
int main(){
   int i=1,num;
   printf("Enter the number= ");
   scanf("%d",&num);
   for ( i = 1; i <=10; i++)
   {
     printf(" %d X %d = %d\n", num,i,num*i);
   }
   return 0;
}

10. wap to display the fabonaci sequence
#include<stdio.h>
int main()
{ int i,j,a=0,b=1,c,n=10;
for ( i = 1; i <=10; i++)
{
    printf("%d, ",a);
    c=a+b;
    a=b;
    b=c;
}
    return 0;
}

11. enter three digit number and find their sum
#include<stdio.h>
int main()
{ int num,rem, sum=0;
printf("Enter any number= ");
scanf("%d",&num);
printf("Digits are");
while(num>0)
{
   rem=num%10;
   sum+=rem;
   num/=10;
}
printf("Sum of digits are= %d",sum);
   return 0;
}

12. to enter three digits number and reverse it 
#include<stdio.h>
int main(){
 int num,rem,rev=0;
 printf("Enter any number= ");
 scanf("%d",&num);
 while (num>0)
 {
   rem=num%10;
   rev=rev*10+rem;
   num=num/10;
 }
 printf("The reverse of the number is= %d", rev);
   return 0;
}

13 to find the number is palindrome or not 
#include<stdio.h>
int main()
{
 int num,rem,rev=0 ,a;
 printf("Enter any number= ");
 scanf("%d",&num);
  a=num;
 while (num!=0)
 {
   rem=num%10;
   rev=rev*10+rem;
   num=num/10;
  } 
 if (rev==a)
 {
 printf("The number is palindrome ");
 }
 else{
   printf("The number is not Palindrome");
 }
   return 0;
}

14. To find the prime factor of any number 
#include<stdio.h>
int main()
{ int n,prime;
printf("Enter any number to find its prime factor= ");
scanf("%d",&n);
for( int i=2;i<=n;i++)
{
    if(n%i==0)
    { 
        prime=1;
        for (int j = 2; j<=i/2; j++)
        {
          if(i%j==0)
          {
            prime=0;
            break;
          }
        
        }
        if(prime==1)
        {
            printf("%d,",i);
        }
    }
}
    return 0;
}

15. to find the prime or not  of any number
#include<stdio.h>
int main()
{ int n, a=2,prime=0;
printf("Enter any number= ");
scanf("%d",&n);
while (a<n)
{
if (n%a==0)
{
  prime++;
}
a++;
}
if(prime==0)
{
  printf("Enter number is prime number");
}
else{
  printf("Enter number  is not Prime number");
}
  return 0;
}

16. to find the sum of the up to input number square 
#include<stdio.h>
int main(){
 int num,sum=0,b=0;
 printf("Enter any number= ");
 scanf("%d",&num);
while (num!=0)
{
 b=num*num;
 sum+=b;
 num--;
} 
printf("The sum of the squares are = %d",sum);
  return 0;
}

17. 
 this is break 
 #include<stdio.h>
 int main()
 { int i,n=10;
 for(i=1;i<=10;i++)
 {
    printf("%d ",i);
    if (i==4)
    {
       break;
    }  
 }
   return 0;
 }

this is continue looping 
#include<stdio.h> 
int main()
{ 
    int j,n=6;
for(j=1;j<=6;j++)
{

 if (j==3)
 {
    continue;
 }
 printf("%d ",j);
} 
  return 0;
}

this is goto looping in c 
#include<stdio.h>
#include<stdlib.h>
int main()
{ 
    int n1,n2;
    printf("enter one number= ");
    scanf("%d",&n1);
    printf("enter another  number= ");
    scanf("%d",&n2);
if(n1>n2)
    goto great;
else
    goto small;
great:
printf("%d is greatest number",n1);
exit(0);
small:
printf("%d is greatest",n2);
return 0;
}

18 . to print sequences 
#include<stdio.h>
int main(){
int i,j;
for(i=1;i<=5;i++)
{
    for ( j =1; j<=i; j++)
    {
       printf("%d ",j);
    }
    printf("\n");
}
    return 0;
}

19 wap in c to display the following in c
#include<stdio.h>
int main()
{ int i,j;
for ( i = 1; i <=5; i++)
{
    for(j=1;j<=i; j++)
    {
        printf("1 ");
    }
    printf("\n");
}
    return 0;
}

20.  to print the following series using 
#include<stdio.h>
int main()
{ int i,j;
for ( i = 1; i <=5; i++)
{
    for ( j = 1; j<=i; j++)
    {
        printf("%d ",i);         
    }
    printf("\n");
}
    return 0;
}
// strings
/* 
 Q.n 1  To find the length of the string 
#include<stdio.h>
#include<string.h>
int main()
{ char myName[20];
int len;
printf("Enter your name: ");
gets(myName);
len=strlen(myName);
printf("Length of a String is %d",len);
return 0;
}

Q.N 2 to copy one string to another string 
#include<stdio.h>
#include<string.h>
int main()
{ char hisName[20],heSay[20];
printf("Enter his name: ");
gets(hisName);
strcpy(heSay,hisName);
printf("Copied string from hisName is : %s",heSay);
 return 0;
}

Q.N 3 to concate two string
#include<stdio.h>
#include<string.h>
int main()
{ char firstName[20],lastName[20],fullName[20];
printf("Enter your first name: ");
gets(firstName);
printf("Enter your last name : ");
gets(lastName);
strcpy(fullName,strcat(firstName, lastName));
printf("His full name is : %s",fullName);
    return 0;
}

Q.n 4 To compare two strings
#include<stdio.h>
#include<string.h>
int main()
{ char string1[13],string2[23];
int result;
printf("Enter First String: ");
gets(string1);
printf("Enter second String: ");
gets(string2);
result=strcmp(string1,string2);     //if str1==str2 then 0 output
printf("The result is :%d",result);  // if str1 >str2 then 1
    return 0;                                            // if str1<str2 then -1
}

Q.N 5 to convert uppercase to lowercase
#include<stdio.h>
#include<string.h>
int main()
{ char lowerCase[15];
printf("Enter any string in Lowercase:");
gets(lowerCase);
printf("The uppercase of %s is: ",lowerCase);
puts(strupr(lowerCase));
  return 0;
}

Q.N 6 to convert uppercase to lowercase
#include<stdio.h>
#include<string.h>
int main()
{ char upperCase[20];
printf("Enter string in Uppercase: ");
gets(upperCase);
printf("The lowercase of %s is : ",upperCase);
puts(strlwr(upperCase));
  return 0;
}

Q.n to find the total numer of the alphabets , digits and the special in entered string
#include<stdio.h>
#include<string.h>
int main()
{ char anyString[30];
int alpha=0,digit=0,special=0;
printf("Enter any string: ");
gets(anyString);
for(int i=0;i<strlen(anyString);i++)
{
    if((anyString[i]>='a' && anyString[i]<='z') || (anyString[i]>='A' && anyString[i]<='Z'))
    {
        alpha++;
    }
    else if(anyString[i] >='0' && anyString[i] <= '9')
    {
        digit++;
    }
    else
    {
        special++;
    }
} 
printf("Total alphabets are :%d\n",alpha);
printf("Total digits  are :%d\n",digit);
printf("Total special characters are :%d\n",special);
    return 0;
}

Q.N to to count total number of vowel and consonatn using functions 
#include<stdio.h>
#include<string.h>
int main() 
{ char string1[20];
int vowel=0,consonant=0;
printf("Enter any string: ");
gets(string1);
strlwr(string1);
for(int i=0;i<strlen(string1);i++)
{
    if((string1[i]=='a')|| (string1[i]=='e') || (string1[i]=='i') || (string1[i]=='o') || (string1[i]=='u'))
    {
        vowel++;
    }
    else
    {
        consonant++;
    }
}
printf("Total vowel in %s is: %d\n",string1,vowel);
printf("Total consonant in %s is: %d",string1,consonant);
    return 0;
}


Q.N 9 is reamaning to do 
#include<stdio.h>
#include<string.h>
int main()
{ char name[30]; 
int word;
printf("Enter your name: ");
gets(name);
for(int i=0;i<strlen(name);i++)
{
    if((name[i]!=' ') || (name[i]!=' \0' ))
    {
        word++;
    } 
    else
    {
break;
    }
}
printf("Total numbers in word are: %d",word);

    return 0;
}

Q.N  10 to reverse a string
#include<stdio.h>
#include<string.h>
int main()
{ char name[30],rev[30];
printf("Enter your name: ");
gets(name);
strcpy(rev,strrev(name));
printf("Reverse is : ");
puts(rev);
    return 0;
    }

Q.N 11. this is the program to find the string is palindrome  or not 
#include<stdio.h>
#include<string.h>
int main()
{ 
 char enterstring[20],copies[20];
printf("Enter any string: ");
gets(enterstring);
strcpy(copies,enterstring);
if(strcmp(enterstring,strrev(copies))==0)
{
    printf("Enter string is palindrome");
}
else{
    printf("Enter string is not palindrome");
}
return 0;
} 

Q.N 12  to count totl number of the characters in entered  
#include<stdio.h>
#include<string.h>
int main()
{ char anyString[30];
int alpha=0,digit=0,special=0,total=0;
printf("Enter any string: ");
gets(anyString);
for(int i=0;i<strlen(anyString);i++)
{
    if((anyString[i]>='a' && anyString[i]<='z') || (anyString[i]>='A' && anyString[i]<='Z'))
    {
        alpha++;
    }
    else if(anyString[i] >='0' && anyString[i] <= '9')
    {
        digit++;
    }
    else
    {
        special++;
    }
} 
printf("Total alphabets are :%d\n",alpha);
printf("Total digits  are :%d\n",digit);
printf("Total special characters are :%d\n",special);
total+=alpha+digit+special;
printf("Total character in the string are:  %d",total);
    return 0;
}  

13 wap to sort the Entered name in ascending order

#include<stdio.h>
#include<string.h>
int main()
{ 
    int n,i,j;
    printf("Enter number of empolyee: ");
    scanf("%d",&n);
    char name[20][20],temp[30];
    for(i=0; i<n; i++)
    {
        gets(name[i]);
    }
    for ( i = 0; i < n; i++)
    {
        for( j = i+1; j < n; j++)
        {
                if(strcmp(name[i],name[j])>0)
                {
                    strcpy(temp,name[j]);
                    strcpy(name[j],name[i]);
                    strcpy(name[i],temp);
                }
        }  
    }
    printf("printing the names in ascendng order are : \n");
    for(i=0; i<n; i++)
    {
        puts(name[i]);
    }
    return 0;
}  */

// functions

//lab sheet 08 
/*
Q.N 1 finding the sum of the two entered numbers 
#include<stdio.h>
int sum(int , int);
int main()
{ int a,b;
printf("Enter the value of a and b: ");
scanf("%d%d",&a,&b);
int z=sum(a,b);
printf("The sum of the numbers is %d",z);
    return 0;
}
int sum(int x,int y)
{ int s;
s=x+y;
return s;
}
Q.n 2 finding the area and the perimeter of the rectangle
#include<stdio.h>
int area(){
    int l,b;
printf("Enter the length and breadth: ");
scanf("%d%d",&l,&b);
return l*b;
}
int perimeter()
{
    int l,b;
    printf("Enter the length and the breadth: ");
    scanf("%d%d",&l,&b);
    return 2*(l+b);
}
int main()
{
printf("The area of the rectangle is %d \n",area());
    printf("The perimeter of the rectangle is %d\n",perimeter());
return 0;
}

Q.N. 3 simple intrest 
#include<stdio.h>
float simpleIntrest(int, int, float );
int main()
{ int p,t;
float  r;
printf("Enter p t and rate: ");
scanf("%d%d%f",&p,&t,&r);
simpleIntrest(p,t,r);
return 0;
}
float simpleIntrest(int x, int y , float z)
{
float c;
   c=(x*y*z)/100;
    printf("The simple intrest is :  %.2f",c);
}

Q.N 4 to find the enter number is odd or the even
#include<stdio.h>
void number(int);
int main()
{ int n;
printf("Enter the numbe to find it is odd or even: ");
scanf("%d",&n);
number(n);
return 0;
}
void number(int x)
{
    if(x%2==0)
    {
        printf("Enter number is Even");
    }
    else
    {
        printf("Enter number is Odd");
    }
}

Q.N 5 to find whether the input number is prime or not 
#include<stdio.h>
void numCheck(int);
int main()
{
int a;
printf("Enter any number to check it is prime or not: ");
scanf("%d",&a);
numCheck(a);
return 0;
}
void numCheck(int x)
{


}

Q.N 6 to find the sum of n natural number
#include<stdio.h>
int sum(int);
int main(){
    int n;
    printf("Enter any number to find till its sum: ");
    scanf("%d",&n);
    sum(n);
}
int sum(int x)
{ int sum=0;
    for(int i=1; i<=x;i++)
    {
        sum+=i;
    }
    printf("The sum of %d natural number is : %d ",x,sum);
}

Q.N . 7 to find the total number of alphates digit and special
#include<stdio.h>
#include<string.h>
int findingDifferent(char anyString[20]);
int main()
{ 
    char anyString[30];
printf("Enter any string: ");
gets(anyString);
 findingDifferent(anyString);
 return 0;
}
int findingDifferent(char name[30])
{ int alpha=0,digit=0,special=0;
    for(int i=0;i<strlen(name);i++)
{
    if((name[i]>='a' && name[i]<='z') || (name[i]>='A' && name[i]<='Z'))
    {
        alpha++;
    }
    else if(name[i] >='0' && name[i] <= '9')
    {
        digit++;
    }
    else
    {
        special++;
    }
} 
printf("Total alphabets are :%d\n",alpha);
printf("Total digits  are :%d\n",digit);
printf("Total special characters are :%d\n",special);
}

Q.N 8 to check whether the enter string is palindrome or not using functions
#include<stdio.h>
#include<string.h>
char palindrome(char string[]);
int main()
{ char string[20];
printf("Enter any string: ");
gets(string);
palindrome(string);
return 0;
}
char palindrome(char name[]){
    char copied[20];
    strcpy(copied,name);
    if(strcmp(name, strrev(copied))==0)
    {
        printf("Enter string is palindrome");
    }
    else
    {
        printf("Enter string is not Palindrome");
    }
}

Q.N 9. Factorial of any input number using function in c programming  
#include<stdio.h>
int factorial(int);
int main()
{
     int n,result;
printf("Enter the num : ");
scanf("%d",&n);
//result=factorial(n);
printf("The factorial of the enter number is %d! is  : %d ",n,factorial(n));
    return 0;
}
int factorial(int x)
{ 
    int fact=1;
 for( int i=1;i<=x;i++)
 {
    fact=fact*i;
 }
   return fact;
} 

Q.n 10 to find the prime numbers form 1 to 100 using function
#include<stdio.h>
int prime(int n)
{ int a=3

}
int main(){






    return 0;
}
 */ 

// factorial using recursion 

/* #include<stdio.h>
int factorial(int);
int main()
{ 
    int n,result;
printf("Enter any number: ");
scanf("%d",&n);
result=factorial(n);
printf("The factorial of enter number %d is %d",n,result);
    return 0;
}
int factorial(int x)
{ 
    int factorial_of_number;
int i=1;
    if(x==0 ||  x==1)
{
    return 1;
}
else
factorial_of_number=x*factorial(x-i);
return factorial_of_number;
} */ 
