package listings;

import java.util.Scanner;

public class DivCheck {

	public static void main(String[] args) {
		
		//Variablen definieren
		int value;
		int divnr = 1;
		String output;
		int i = 1;
		
		System.out.println("Geben Sie die Zahl an, welche auf Divisoren geprüft werden soll:");
		Scanner scan = new Scanner(System.in);
		value = scan.nextInt();
		
		//Überprüft ob die aktuelle Zahl (divnr) bereits den Wert von Value hat
		while (divnr <= value){
			
			//Werte auf Intialwert zurücksetzen (nötig nach dem ersten Durchlauf)
			output = "";
			i=1;
			
			while (i<=divnr){
					
					if (divnr % i == 0){
					output += " "+i;
					}
			i++;
			}
		
		
		System.out.println("divisors of " + divnr + ":" + output);
		divnr++;
		}

	}

}
