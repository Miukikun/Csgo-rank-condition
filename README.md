# Csgo-random-ranked-condition








#include <iostream>
int main()
{	int W = 0;
	std::cout << "How many match did you win :";
	std::cin >> W;
	int L = 0;
	std::cout << "How many match did you Lose :";
	std::cin >> L;
	if (W<=L)
	{
		std::cout << "The player is thrown to lvl 1 Faceit." << std::endl;
	}
	else
	{
		std::cout << "Good Job, you start at lvl 3 Faceit" << std::endl;
		std::cout << "Then..." << std::endl;
	}
	
		float KD = 0.0f;
	std::cout << "Enter your Kill/Death ratio :";
	std::cin >> KD;
	std::cin.ignore();

	 if (KD >= 3.0f)
	{
		std::cout << "Jump to lvl 5 Faceit" << std::endl;
	}
	 else if (2.0f < KD < 3.0f)
	 {
		 std::cout << "+150elo" << std::endl;
	 }
	 else if (1.0f < KD < 2.0f)
	 {
		 std::cout << "+50elo" << std::endl;
	 }
	 else if (KD < 1.0f)
	 {
		 std::cout << "Maybe try valorant..." << std::endl;
	 }

	return 0;
}
