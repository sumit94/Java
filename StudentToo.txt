/**Define a Student class (roll number, name, and percentage). Define a default and parameterized
constructor. Override the toString method. Keep a count objects created. Create objects using
parameterized constructor and display the object count after each object is created. (Use static member
and method). Also display the contents of each object.*/
class StudentToo{
	int roll;
	String name;
	int percentage;
	static int a=0;

	
	public StudentToo()
	{
		this.roll= 0;
		this.name=" ";
		this.percentage=0;
		
		this.a++;
		System.out.println("No Of Object Created   "+StudentToo.a);
		
		
	}
	
	 public StudentToo(int roll,String name,int percentage)
	{
		this.roll=roll;
		this.name=name;
		this.percentage=percentage;
		
		this.a++;
		
		System.out.println("No Of Object Created   "+StudentToo.a);
		
	} 
		public String toString()
		{
			
			return "Roll-    "+roll+"     Name-"+name+"    Percentage="+percentage;
			
			
			
		}
		
		
		


public static void main(String args[])
{
	StudentToo st=new StudentToo();
	System.out.println(st);
	
	StudentToo st1=new StudentToo(21,"Sumit",85);
	System.out.println(st1);
	
	StudentToo st2=new StudentToo(01,"SAm",45);
	System.out.println(st2);
	
	
	
	

	
	
	
	
	
	
}		
	
	
	
	
}