# Menu-Only

import java.util.Scanner;


public class VendingMachine{
	String type;
	int BillContent;
	Double CoinContent;
	
	int[] Sodaslot=new int[8];
	int[] SnackSlot= new int[40];
	
	public void refill() {
	    int sodaSlotCapacity=30;
		int snackSlotCapacity=60;
	}
	
	
	
	public static void main (String args[]) {
		String option;

		do{
			System.out.println("*******Vending Machine Manager********");
			System.out.println("1- To Add a Machine, enter 1 and press Enter");
			System.out.println("2- To Modify a Machine, enter 2 and press Enter");
			System.out.println("3- To Delete a Machine, enter 3 and press Enter");
			System.out.println("4- To Delete a Machine, enter 4 and press Enter");
		    System.out.println("5- To Simulate purchase and refill , enter 5 and press Enter");
		    System.out.println("6- For Audit reports , enter 6 and press Enter");
		    System.out.println("7- To Exit the menu , enter 7 and press Enter");
		    Scanner scan = new Scanner(System.in);
		    option= scan.nextLine();
		
		
	}while(!option.equals("7"));
	
  }d
	
}
