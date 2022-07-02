using System;
					
public class BMI 
{
	public static void Main()
	{	//Variables to be declaired
		int weight;
		int height;
		int bmi;
		
		
		Console.WriteLine("Please Enter your height in inches: "); //Asks user for their height in inches
		height = Convert.ToInt32(Console.ReadLine());
		
		Console.WriteLine("Enter your weight in pounds: "); //Asks user for their weight in pounds
		weight = Convert.ToInt32(Console.ReadLine());

		
		bmi = (weight * 703)/(height * height); //Actual BMI calculation
		
	    if (bmi >= 18 && bmi <= 30 ) //Tests the users input, tells the user what their BMI is 
		{
			
		Console.WriteLine("Your BMI is {0}. Please follow the chart below to see if you are underweight, normal, overweight or obese.",bmi);	//Tells user BMI score and provides the chart to display the information
		
		Console.WriteLine("\nUnderweight: less than 18.5\nNormal: between 18.5 and 24.9\nOverweight: between 25 and 29.9\nObese: 30 or greater.");
		}	
		
		
		}
			
	}
