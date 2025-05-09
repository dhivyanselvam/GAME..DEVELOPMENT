# EX 7 : THREE DIMENSIONAL TRANSFORMATIONS

## AIM :
 
 To implement the various transformations on three dimensional odjects using a c coding.

## EQUIPMENT REQUIRED:

●	Hardware: Personal Computer (PC)

●	Software: C Compiler

## ALGORITHM :


   Step 1 : Start.

   Step 2 : Draw an image with default parameters.

   Step 3 : Get the choice from user.

   Step 4 : Get the parameters for transformation.

   Step 5 : Perform the transformation.

   Step 6 : Display the output.

   Step 7 : Stop.

## Program :
```
#include<stdio.h> 
#include<conio.h> 
#include<graphics.h> 
#include<math.h> 
int maxx,maxy,midx,midy; 
void axis() 
{ 
getch(); 
cleardevice(); 
line(midx,0,midx,maxy); 
line(0,midy,maxx,midy); 
} 
void main() 
{ 
int gd,gm,x,y,z,o,x1,x2,y1,y2; 
detectgraph(&gd,&gm); 
initgraph(&gd,&gm," "); 
setfillstyle(0,getmaxcolor()); 
maxx=getmaxx(); 
maxy=getmaxy(); 
midx=maxx/2; 
midy=maxy/2; 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Translation Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("after translation"); 
bar3d(midx+(x+50),midy-(y+100),midx+x+60,midy-(y+90),5,1); 
axis(); 
bar3d(midx+50,midy+100,midx+60,midy-90,5,1); 
printf("Enter Scaling Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("After Scaling"); 
bar3d(midx+(x*50),midy-(y*100),midx+(x*60),midy-(y*90),5*z,1); 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Rotating Angle"); 
scanf("%d",&o); 
x1=50*cos(o*3.14/180)-100*sin(o*3.14/180); 
y1=50*cos(o*3.14/180)+100*sin(o*3.14/180); 
x2=60*sin(o*3.14/180)-90*cos(o*3.14/180); 
y2=60*sin(o*3.14/180)+90*cos(o*3.14/180); 
axis(); 
printf("After Rotation about Z Axis"); 
bar3d(midx+x1,midy-y1,midx+x2,midy-y2,5,1); 
axis(); 
printf("After Rotation about X Axis"); 
bar3d(midx+50,midy-x1,midx+60,midy-x2,5,1); 
axis(); 
printf("After Rotation about Y Axis"); 
bar3d(midx+x1,midy-100,midx+x2,midy-90,5,1); 
getch(); 
closegraph(); 
}
```
Program to implement the various transformations on three dimensional odjects using a c coding.
DEVELOPED BY: AHAMADH SULAIMAN M
REGISTER NUMBER: 212224230009
## Output :
![Screenshot 2025-05-09 103808](https://github.com/user-attachments/assets/dad1baf7-85f6-4e54-b769-a44677db6ec1)
![Screenshot 2025-05-09 103823](https://github.com/user-attachments/assets/d0a86bee-647f-4df5-a3a5-f966e4107b56)
![Screenshot 2025-05-09 103848](https://github.com/user-attachments/assets/a705e28a-b9ec-4585-9d15-ebb47d39adc0)
![Screenshot 2025-05-09 104346](https://github.com/user-attachments/assets/722897b2-3737-4b52-b74a-c4c1e27fe3fa)
![Screenshot 2025-05-09 104403](https://github.com/user-attachments/assets/820a2f60-0fa1-4cfe-99c4-85a0cba6a4a5)
![Screenshot 2025-05-09 104416](https://github.com/user-attachments/assets/0d73a384-6aca-4625-91d8-7b062014b0c9)
![Screenshot 2025-05-09 104431](https://github.com/user-attachments/assets/7feebe42-0acc-46cd-9cc0-2c5367791ae2)
![Screenshot 2025-05-09 104440](https://github.com/user-attachments/assets/5e4eccd1-a3e3-4f3f-98e5-43e6ac817962)
![Screenshot 2025-05-09 104449](https://github.com/user-attachments/assets/e858bebb-cbac-4e02-a6b7-852edce0738c)

## Result :
Thus, the C program for performing three-dimensional transformations — including translation, scaling, and rotation about the X, Y, and Z axes — was successfully implemented and the output was verified through graphical representation.
