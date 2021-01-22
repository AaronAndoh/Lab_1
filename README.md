# Lab_1
/**
 * 
 */

/**
 * @author Aaron Kwame Andoh
 *
 */
import java.util.InputMismatchException;
import java.util.Calendar;
import java.util.Scanner;
public class Lab_1 {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		Calendar Start = Calendar.getInstance(); 
		long StartTime = Start.getTimeInMillis(); //Getting the start time in millimeters
		System.out.println("Start Time:"+StartTime);
		
		String s,reverse= "";
		Scanner stringEntered = new Scanner(System.in); // Scanner to allow input from user
		
		
	
		try {
			System.out.println("Enter the String to be reversed");
			String str = stringEntered.nextLine();
			//Reversing the string
			int length=str.length(); //setting the lenght to the input given
			for(int i=length-1;i>=0;i--)
			  reverse=reverse+str.charAt(i);
			System.out.println("Reversed string: "+reverse);
			
			
			Calendar End = Calendar.getInstance(); 
			long EndTime = Start.getTimeInMillis();//Getting the End time in millimeters
			System.out.println("End Time:"+EndTime);
			System.out.println("Execution Time ------>" + (EndTime - StartTime));
			
		} catch(InputMismatchException e) {
			System.out.println("Invalid input.");
			
		}
			
		
	}

}
