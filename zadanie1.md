package labs1;
import java.util.ArrayList;
import java.util.Scanner;

public class zad123 {

	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
		System.out.println("Введите массив, включающий в себя числа от 0 до 4.");
		ArrayList<String> mas = new ArrayList<>();
		String N = in.next();
		char[] myMas = N.toCharArray();
		
		for (int i = 0; i < myMas.length; i++)
		{
			if(Character.digit(myMas[i], 10) > 4) {
				System.out.println("Ошибка! Вы ввели числа не в заданном диапазоне [0;4]");
				return;
			}
		}
		mas.add(N);
		System.out.println("Массив в 5-ной системе счисления: " + mas);
		mas.add(0,"0");
		System.out.println("Дробное чисто в 5-ной системе счисления: " + mas);
		
		// доделать перевод в 10-тичную
	}
}
