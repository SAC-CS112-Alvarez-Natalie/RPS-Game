RPS-Game
========

Simple rock paper scissors game. No repeat, i'll fix that later

import java.util.Scanner;

public class rpsgame {

	public static void main(String[] args) {

		Scanner key = new Scanner(System.in);

		int opponent;
		int user = 0;
		String option = null;
		String username;
		boolean gameOn = false;

		System.out.println("Hello user. Let's play Rock, Paper, Scissors.\n");

		while (gameOn != true) {

			opponent = 1 + (int) (Math.random() * 3);

			switch (opponent) {
			case 1:
				option = "r";
				break;
			case 2:
				option = "p";
				break;
			case 3:
				option = "s";
				break;
			}

			System.out.println("On 3 pick r, p, or s! Ready?");
			System.out.println("One");
			System.out.println("Two");
			System.out.println("Three");

			username = key.next();
			System.out.println("User > " + username);
			System.out.println("Opponent > " + option);


			if (user == opponent) {
				System.out.println("Draw");
				
			} else if (user == 1 && opponent == 3 || user == 2 && opponent == 1
					|| user == 3 && opponent == 2) {
				System.out.println("You win!!");
			} else
				System.out.println("You lose!!");

			{
				System.out.println("\nHow fun! Try again later!!");
				gameOn = true;
			}
		}
	}
} 
				System.out.println("\nYou lose!!");

			{
				System.out.println("\nHow fun! Try again later!!");
				gameOn = true;
			}
		}
	}
} 
