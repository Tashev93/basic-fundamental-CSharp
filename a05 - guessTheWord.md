# guessTheWord

            string secretWord = Console.ReadLine();
            string guess = "";
            int guessCnt = 0;
            int guessLim = 3;
            bool outOfGuesses = false;

            while (guess != secretWord && !outOfGuesses)
            {
                if(guessCnt < guessLim)
                {
                    Console.Write("Enter guess: ");
                    guess = Console.ReadLine();
                    guessCnt++;
                }
                else
                {
                    outOfGuesses = true;
                }
            }
            if (outOfGuesses)
            {
                Console.WriteLine("You Lose!");
            }
            else
            {
                Console.WriteLine("You Win!");

            }
