# numberPyramid

            Console.Write("Enter your pyramide number: ");
            int n = int.Parse(Console.ReadLine());

            int curent = 1;

            bool isBigger = false;

            for (int col = 1; col <= n; col++)
            {
                for (int row = 1; row <= col; row++)
                {

                    if (curent > n)
                    {
                        isBigger = true;
                        break;
                    }
                    Console.Write(curent + " ");
                    curent++;
                }
                if (isBigger)
                {
                    break;
                }
                Console.WriteLine();
            }
