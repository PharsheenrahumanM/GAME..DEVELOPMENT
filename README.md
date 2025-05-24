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
~~~
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
initgraph(&gd,&gm,"c://turboc3//bgi");
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

Program to implement the various transformations on three dimensional odjects using a c coding.
DEVELOPED BY: MIDHUN S
REGISTER NUMBER: 212224230158
~~~
## Output :
![image](https://github.com/user-attachments/assets/9901cd33-355e-4c31-8b56-efede8249fc9)
![image](https://github.com/user-attachments/assets/d9eada57-4ee3-46b5-b1c3-c3b96f5c0159)
![image](https://github.com/user-attachments/assets/00b620f3-1eb6-4a84-87dc-bfd131c41733)
![image](https://github.com/user-attachments/assets/553713f1-2df7-4120-850c-e9eb055a27af)
![image](https://github.com/user-attachments/assets/b6b948be-2d2a-441e-92ef-4cc32b023b38)
![image](https://github.com/user-attachments/assets/e84620fd-5bcc-4f91-80c6-93dba17d19c6)
![image](https://github.com/user-attachments/assets/c394168b-c4be-4eec-9408-79cfe5e84220)
![image](https://github.com/user-attachments/assets/6650ad6b-11e8-474a-80ac-ecd5dff69ee7)
## Result :
Thus, the C program for performing three-dimensional transformations — including translation, scaling, and rotation about the X, Y, and Z axes — was successfully implemented and the output was verified through graphical representation.
