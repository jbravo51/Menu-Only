
import java.util.Scanner;
public class MainTask
{
	public static void main (String args[]) 
	{
		String option;
		//int 
		VendingMcahine[] machineArray=new VendingMachine[40];
		do
		{
			System.out.println("*******Vending Machine Manager********");
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
		    			//addMachine=new
		    			break;
		    		}
		    		case "2":
		    		{
		    			//deleteMAchine=new
		    			break;
		    		}
		    		case "3":
		    		{
		    			//refillMachine=new
		    			break;
		    		}
		    		case "4":
		    		{
		    			//simulation=new
		    			break;
		    		}
		    		case "5":
		    		{
		    			//audit=new
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
		}while(!option.equals("7"));
	}
}
public class VendingMachine()
{	//Member Variables
	String type:
	int machineID;
	int billContain;
	Dooble coinContain;
	//Constructor
	public VendingMachine()
	{
		
	}
	//Method to add a Machine
	public void addMachine()
	{	
		
		
	}
	//Method to refill a Machine
	public void refillMachine()
	{
	
	}
        //Method to remove a Machine
	public void deleteMachine()
	{
	
	}
	//Method that shows the inventory of a Machine
	public void inventory()
	{
	
	}
	//Method that simulate the use of a machine
	public void simulation()
	{
	
	}
	//Method that shows the inventory of a Machine
	public void audit()
	{
	
	}
	
}
public class sodaMachine extends VendingMachine
{	
	int[] slot=new int[8];
	dooble[] cost=new int[8];
}
public class snackMachine extends VendingMachine
{	
	int[] slot=new int[40];
	dooble[] cost=new int[8];
}
public class comboMachine extends VendingMachine
{	
	int[] SodaSlot=new int[8];
	int[] snackSlot=new int[20];
	dooble[] sodaCost=new int[8];
	dooble[] sodaCost=new int[20];
}

