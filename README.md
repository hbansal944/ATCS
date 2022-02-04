# ATCS
package com.atcs.main.assessment;
import java.util.Random;

public class assessment {
	public static void main(String[] args) {
		char[] chararray = Array();
	    System.out.println("alphabets");
	     displayArray(chararray);

	    int[] counts = countLetters(chararray);
	  
	    System.out.println();
	    System.out.println("No. of time each alphabet are in array");
	     displayCounts(counts);
	  }
	

	  public static char[] Array() {
		  
	    char[] chararray1 = new char[26];
	    Random generator = new Random();
	    String S ="abcdefghijklmnopqrstuvwxyz";
	    for (int i = 0; i < chararray1.length; i++) 
	      chararray1[i] = (char) S.charAt(generator.nextInt(26));
	   return chararray1;
	  } 

	  
	public static void displayArray(char[] chars) {
	   
	    for (int i = 0; i < chars.length; i++) {
	    	System.out.println(chars[i] + " ");
	  
	           }
	         }
	       
	         public static int[] countLetters(char[] chars) {
	    
	           int[] count = new int[26];
	      
	           for (int i = 0; i < chars.length; i++) 
	             count[chars[i] - 'a']++;
	      
	           return count;
	         }
	      
	        public static void displayCounts(int[] counts) {
	           for (int i = 0; i < counts.length; i++) {
	        	   System.out.println(counts[i] + "- " + (char)(i + 'a'));
	           }
	         }
}
	
	    
	         
