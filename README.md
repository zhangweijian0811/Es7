void fibonacci() {
	printf("Insert the index of Fibonacci element\n");
	int num1 = 1, num2 = 1, num3 = 0, n;
	scanf("%d", &n);
	if (n <= 2) {
		printf("Fibonacci(%d) = %d\n", n ,num1);
	}
	else
	{
		int i = 2;
		while (i < n)
		{
			i++;
			num3 = num1 + num2;
			num1 = num2;
			num2 = num3;
			}
		printf("Fibonacci(%d) = %d\n",n, num3);
	 }
}

void is_prime() {
	printf("Enter an integer number\n");
	int number;
	scanf("%d", &number);
		int i = 0;
		while (i <	 number) {
			i++;
			if (number%i == 0);
			{
				if (i == number)
					printf("The number %d is prime\n",number);
				else
					printf("The number %d isn't prime\n",number);
				break;
			}
		}
}

void triangle_Floyd() {
	printf("Enter an integer number\n");
	int numero;
	int riga, colonna;
	int cifra;
	scanf("%d", &numero);
	if (numero <= 0)
		printf("Errore, il lato deve essere maggiore di zero\n");
	else{
		riga = 0;
		cifra = 1;
	}
	while (riga < numero)
	{
		colonna = 0; 
		while (colonna <= riga)
		{
			printf("%d ", cifra);
			colonna = colonna + 1;
			cifra = cifra + 1;
		}
		printf("|\n");
		riga = riga + 1;
	}
}
