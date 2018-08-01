# Hierarchial_inheritance
class Father
{
 int a,b;
 void getdata(int x,int y)
{
 a=x;
 b=y;
}
}
class Son extends Father
{
 int add()
{
  return(a+b);
}
void disp()
{
 System.out.println("A:"+a);
System.out.println("B:"+b);
System.out.println("Sum:"+add());
}
}
class Daughter extends Father
{
int mul()
{
 return(a*b);
}
void disp()
{
 System.out.println("A:"+a);
System.out.println("B:"+b);
System.out.println("Mul:"+mul());
}
}
class Test19
{
public static void main(String args[])
{
 Son objs=new Son();
 Daughter objd=new Daughter();
 objs.getdata(25,35);
 objs.disp();
  objd.getdata(45,65);
 objd.disp();
}
}

