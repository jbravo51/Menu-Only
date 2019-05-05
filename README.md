public class VendingMachine
{	//Member Variables
	String type;
	int machineId;
	int[] slot;
	int billContain;
	Double coinContain;
	//Constructor
	public VendingMachine()
	{

	}
	public VendingMachine(int machineId,String type,int[] slot)
	{
		this.machineId=machineId;
		this.slot=slot;
		this.type=type;
	}
	void info()
    {
        System.out.println("Machine"+machineId+" is a "+type+", and it have "+slot+"");
    }
	//Method to add a Machine
	public void addMachine(String type)
	{	
		//return VendingMachine(,String type,int[] slot)
		
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
class sodaMachine extends VendingMachine
{	
	int[] slot=new int[8];
	public int[] soslots()
	{
		for(int i=0;i<8;i++)
		slot[i]=i;
		return slot
	}
	//double[] cost=new int[8];
}
class snackMachine extends VendingMachine
{	
	int[] slot=new int[40];
	public int[] snslots()
	{
		for(int i=0;i<8;i++)
			slot[i]=i;
	}

	//double[] cost=new int[8];
}
class comboMachine extends VendingMachine
{	
	static int[] SodaSlot=new int[8];
	//int[] snackSlot=new int[20];
	public int[] cslots()
	{
	for(int i=0;i<8;i++)
	{
		SodaSlot[i]=i;
	}}
	//double[] sodaCost=new int[8];
	//double[] sodaCost=new int[20];
}

