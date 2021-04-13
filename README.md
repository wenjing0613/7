package week6
import java.util.Scanner;
class Rectangle
{
	double width=0;
	double height=0;
	
	public static void area(double w,double h)
	{
		double area=0;
		area=w*h;
		System.out.println("面积为："+area);
	}
	public static void perimeter(double w,double h)
	{
		double perimeter=0;
		perimeter=2*(w+h);
		System.out.println("周长为："+perimeter);
	}
	public static void main(String args[])
	{
		Scanner sc=new Scanner(System.in);
		System.out.println("分别输入矩形的宽和高:");
		double width=sc.nextDouble();
		double height=sc.nextDouble();//转换
		
		System.out.println("该矩形宽："+width+",长："+height);
		area(width,height);
		perimeter(width,height);
	}
}
