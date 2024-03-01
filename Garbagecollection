package week04;
import java.util.Scanner;
public class demoFinalize {
	public static void main(String[] args) {
		student1 Sanjana = new student1();
		Sanjana.display();
		System.out.println("Object reference is ... "+Sanjana);
		Sanjana.finalize();
		System.gc();
		System.out.println("Object garbage collected");

    }
}
class student1
{

	String name;
	int rno;
	float res;
	Scanner sc = new Scanner(System.in);
	student1()
	{

		System.out.println("Enter Roll Number of Student.");
		rno= Integer.parseInt(sc.next());
		System.out.println("Enter Name of Student.");
		name = sc.next();
		System.out.println("Enter result of the Student.");
		res = Float.parseFloat(sc.next());
	}
	void display()
	{

		System.out.println(rno+"\t\t"+name+"\t\t"+res);
	}
	@Override
	protected void finalize()
	{
		sc.close();
		System.out.println("Object Cleaned Up by Finalize Method.");
		
	}
}
