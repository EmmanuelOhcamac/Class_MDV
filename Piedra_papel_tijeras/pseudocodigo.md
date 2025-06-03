Main
{
	int computerWin
	int playerWin
	int intentos = 3

	string[] opciones = {"piedra", "papel", "tijeras"}
	Random random = new Random()

While (intentos >=0)
{
	escribir "Elije piedra, papel o tijeras"
	leer intentoJugador
	eleccion = random opciones

	if (intentoJugador = eleccion)
	{
		escribir "Compu eligió: " elección " es un empate"
	}
	else if (intentoJugador = !eleccion)
	{
		While (eleccion = "piedra")
		{
			if (intentoJugador = papel)
			{
			Escribir "Compu elijió " eleccion " perdiste"
			}
			else if (intentoJugador = tijeras)
			{
				Escribir "Compu elijió " eleccion " ganaste"
			}
		}
		While (eleccion = "papel")
		{
			if (intentoJugador = piedra)
			{
				Escribir "Compu elijió " eleccion " perdiste"
			}
			else if (intentoJugador = tijeras)
			{
				Escribir "Compu elijió " eleccion " ganaste"
			}
		}
		While (eleccion = "tijeras")
		{
			if (intentoJugador = papel)
			{
				Escribir "Compu elijió " eleccion " perdiste"
			}
			else if (intentoJugador = piedra)
			{
				Escribir "Compu elijió " eleccion " ganaste"
			}
		}
	}
--intentos
}
if (intentos <=0)
{
	Escribir "Se acabó el juego. Loas puntajes son:"
	Escribir "Compu: " computerWin " | Jugador: " playerWin
	if (computerWin > playerWin)
	{
		Escribir "Compu gana"
	}
	else if (computerWin = playerWin)
	{
		Escribir "Es un empate"
	}
	else if (computerWin < playerWin)
	{
		Escribir "Tú ganas"
	}
}
FinMain