# Session3-Ex7

// ب ن ک اعداد اول بین یک میلیون تا ده میلیون را در خروجی چاپ کند

package com.personal.ex7;

public class ex7 {

	public static void main(String[] args) {
		long prime=1000000;
		
		do {
			if (PrimeFinder(prime))
			System.out.println(prime);

			prime++;
			
		}
		while(prime<10000000);
		

	}
	
	
static boolean PrimeFinder(long prime) {
		
		double root= Math.sqrt(prime);
		for (int i = 2; i <= root; i++) {
			
			if(prime %i==0) {
				return false;}
			
			}
		return true;
		
	}


}
