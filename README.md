# monster
int p=0;
int h=0;
int a=0;
char z='A';
int x =720;
char m='B';
int y =200;
void setup()
{
size(850,600);
smooth();
}
void draw()
{
background(222);
if (keyPressed) 
{
if (keyCode == LEFT) 
{ 
p=p-10;
} if (keyCode == RIGHT) 
{ 
p=p+10;
}
if (keyCode == DOWN) 
{
h=h+10;
}
if (keyCode == UP) 
{
h=h-10;
}
if ((key == 'a'))
{
a=a+50;
}
if ((key == 'b')) 
{
a=a-50;
}
}
fill(163+a);
beginShape();
vertex(0+p,300+h);
vertex(70+p,200+h);
vertex(600+p,200+h);
vertex(670+p,320+h);
vertex(600+p,450+h);
vertex(550+p,550+h);
vertex(500+p,450+h);
vertex(220+p,450+h);
vertex(170+p,550+h);
vertex(120+p,450+h);
vertex(50+p,400+h);
vertex(0+p,300+h);
endShape();
fill(255);
ellipse(720+p,200+h,200,200);
fill(0);
if(x!=mouseX||y!=mouseY)
{
if(x>mouseX)
x--;
if(x<mouseX)
x++;
if(y>mouseY)
y--;
if(y<mouseY)
y++;
}
ellipse(x,y,20,20);
}
