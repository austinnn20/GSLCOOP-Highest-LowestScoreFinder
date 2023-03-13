# GSLCOOP-Highest-LowestScoreFinder
This code is for finding the biggest and the smallest from a set of integer arrays (GPA)

This is the code :

import java.util.Scanner;

public class GSLCOOP {
	 
	 static int Max(int[] num) {
	        int max = num[0];
	        for (int i = 1; i < num.length; i++) {
	            if (num[i] > max) {
	                max = num[i];
	            }
	        }
	        return max;
	    }
	 
	    static int Min(int[] num) {
	        int min = num[0];
	        for (int i = 1; i < num.length; i++) {
	            if (num[i] < min) {
	                min = num[i];
	            }
	        }
	        return min;
	    }
	 
	 public static void main(String[] args) {
	      
	        Scanner input = new Scanner(System.in);
	        System.out.print("Enter the ammount of Students	: ");
	        
	        int n = input.nextInt();
	        int[] num = new int[n];
	        System.out.print("Enter " + n + " Scores : ");
	        for (int i = 0; i < n; i++) {
	            num[i] = input.nextInt();
	        }
	        int max = Max(num);
	        int min = Min(num);
	        System.out.println("Highest Score	: " + max);
	        System.out.println("Lowest Score	: " + min);
	    }

	}
