/*CIS 144. 
Vending Machine
Jorge Bravo - jlbravo93@hotmail.com 
Seema Khan - khanseema2000@gmail.com
Hoda Masteri - hodamasteri@gmail.com
Rudy Cordero - rcordero17@student.ccc.edu
*/
import java.util.Scanner;
public class MainTask{
	public static void main (String args[]) 
	{
		String option, opType;
		int n=0; 
		VendingMachine methosVM=new VendingMachine();
		sodaMachine sMachine=new sodaMachine();
		snackMachine snMachine=new snackMachine();
		comboMachine cMachine=new comboMachine();
		VendingMachine[] machineArray=new VendingMachine[40];
		do
		{
			System.out.println("\n\n\n\n*******Vending Machine Manager********");
			System.out.println("1- To Add a Machine, enter 1 and press Enter");
			System.out.println("2- To Delete a Machine, enter 2 and press Enter");
			System.out.println("3- To Refill a Machine, enter 3 and press Enter");
		    System.out.println("4- To Simulate purchase, enter 4 and press Enter");
		    System.out.println("5- For Audit reports , enter 5 and press Enter");
		    System.out.println("6- To Exit the menu , enter 6 and press Enter");
		    System.out.println("\n Please insert an intiger:");
		    Scanner scan = new Scanner(System.in);
		    option= scan.nextLine();
		    switch(option)
		    {
		    	case "1":
		    	{
		    		if(n==40)
		    		{	System.out.println("The float of Machines is full. No more Machine can be add.");
		    			break;}
		    		System.out.println("Please select wath type of Machine you want to add");
		    		System.out.println("1- Soda Machine");
					System.out.println("2- Snack Machine");
					System.out.println("3- Combo Machine");
				    System.out.println("\n Please insert an intiger and press Enter:");
				    opType= scan.nextLine();
				    switch(opType)
				    {
				    	case "1":
				    	{
				    		 machineArray[n]=new VendingMachine(n,"Soda",sMachine.soslots(),0,30);
				    		 //methosVM.addMachine("Soda");
				    		 n++;
				    		break;
				    	}
				    	case "2":
				    	{
				    		machineArray[n]=new VendingMachine(n,"Snack",snMachine.snslots(),0,30);
				    		//methosVM.addMachine("Snack");
				    		n++;
				    		break;
				    	}
				    	case "3":
				    	{
				    		machineArray[n]=new VendingMachine(n,"Combo",cMachine.cslots(),0,30);
				    		//methosVM.addMachine("Combo");
				    		n++;
				    		break;
				    	}
				    	default:
				    		System.out.println("Invalid entry! Please enter an intiger between 1 to 3");
				    }
		    		//addMachine=new
		    		break;
		    	}
		    	case "2":
		    	{
		    		//deleteMAchine=new
		    		if(n>0)
			        {
		    			System.out.print("Enter Machine ID to be deleted : ");
		    			int IDnum = scan.nextInt();
		    			if(IDnum>=0&&IDnum<=n)
		    			{	machineArray=methosVM.deleteMachine(IDnum, machineArray, n);
			        		n--;
			        		break;
		    			}else
		    			{	System.out.print("\nMachine ID not found ");
		        			break;}
			        }else
			        {	System.out.print("\nThere are no machines");
		        		break;
			        }
		    	}
		    	case "3":
		    	{
		    		//refillMachine=new
		    		break;
		    	}
		    	case "4":
		    	{
		    		//simulation=new
		    		System.out.print("Enter Machine ID to purchase from : ");
			        int IDnum = scan.nextInt();
			        boolean machineDetected=false;
			        for(int k = 0; k <n; k++)
			        {   if(machineArray[k].machineId == IDnum)
			            {	machineDetected=true;
			            	machineArray[k].simulation(k);
			            }
					}
			        if (machineDetected==false) 
			        {  	System.out.print("\nInvalid Machine ID");}
		    		break;
		    	}
		    	case "5":
		    	{
		    		methosVM.audit(machineArray,n);		    		//audit=new
		    		break;
		    	}
		    	case "6":
		    	{
		    		//addMachine=new
		    		break;
		    	}
		    	default:
		    		System.out.println("Invalid entry! Please enter an intiger between 1 to 6");
		    }
		}while(!option.equals("6"));
	}
}
