
  import java.util.Scanner;
public class TotalPayable{
	public static void main(String[]args){

		//Declare variables
		String lname,fname,sname,department;
		int dcode,idnumber,nunits;
		double rpunit,mfee,regfee,ttl_pay,tfee;
		department = "Engineering";
		nunits = 24;
		regfee = 350.00;
		mfee = 1800.20;

		//create scanner obj
		Scanner in = new Scanner(System.in);


		//input screen
		System.out.printf("Last Name of Student   :");
		lname = in.nextLine();
		System.out.printf("First Name of Student  :");
		fname = in.nextLine();
		System.out.printf("Department Code        :");
		dcode = in.nextInt();
		System.out.printf("ID Number              :");
		idnumber = in.nextInt();
		System.out.printf("Rate per unit          :");
		rpunit = in.nextDouble();

		//Output Screen
		System.out.printf("\nStudent Name           :%s%s\n",lname,fname);
		System.out.printf("Department Code        :%d\n",dcode);
		System.out.printf("Department             :%s\n",department);
		System.out.printf("ID Number              :%d\n",idnumber);
		System.out.printf("Number of Units        :%d\n",nunits);
		System.out.printf("Rate per Unit          :%.2f\n",rpunit);

		//Compute sheesh
		tfee = rpunit*nunits;
		ttl_pay = tfee+regfee+mfee;


		System.out.printf("\nTotal Payable          :%.2f",ttl_pay);




	}
}
