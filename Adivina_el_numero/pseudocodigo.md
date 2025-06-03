Main

	int intentos = 7;
	bool adivinado = false;
	Random random = new Random ();
	int numeroSecreto = random.Next(1, 100);

	write "Bienvenido jugador escribe un número para empezar"
	leer "numeroJugador"
	
	while (intentos > 0 && !adivinado)
	{
		if (numeroJugador <= numeroSecreto)
		{
			write "Muy bajo, te quedan" intentos "intentos. Prueba de nuevo"
			leer "numeroJugador"
		}
		else if (numeroJugador >= numeroSecreto)
		{
			write "Muy alto, te quedan" intentos "intentos. Prueba de nuevo"
			leer "numeroJugador"
		}
		--intentos
	}
	if (intentos <= 0 && !adivinado)
	{
		write "Haz perdido, el número era:" numeroSecreto
	}
	else if (intentos <= 0 && adivinado)
	{
		write "Felicidades, lo haz decubierto"
	}
FinMain