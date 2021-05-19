import java.util.Scanner;

class Add{
	static int arr[] = new int[100];
	static float sum=0;
	static int flag=0;
	static Scanner input = new Scanner(System.in);
	public static void avg()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		System.out.println("Enter "+ n +" elements of array");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		System.out.println("Enter Element to be found");
		int ind = input.nextInt();
		for(int i=0;i<n;i++)
		{
			if(ind==arr[i])
			{
				System.out.println("Element is present");
				flag=flag+1;
				
			}
		}
		if(flag==0)
		{
			System.out.println("Element not found");
		}
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.avg();
	}
}
