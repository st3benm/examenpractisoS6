
        Proceso examenpractico
	//Primero leemos el problema 
	//Pedimos al usuario los valores de cuanto es su sueldo y cuantos años de servicio tiene el usuario y el porcentaje del objetivo cumplido 
	//primero utilizamos el SI y el SINO que son condicionales que se encargan de comprobar las bonificaciones  y el tiempo de servicio 
	//Realizamos calculos m,atematiucos para obtener los aumentos , porcentajes y el total del sueldo mensual 
	//Al final mostramos al usuario los resultados de su aumento de salario segun su porcentaje 
	
	// desarrollar un algoritmo que calcule la bonificación que cada empleado recibirá según las siguientes condiciones
	
	// ENTRADA
	Definir tiemp_serv, salario, aument_bonifi, aument_bonifi_adicc, porcentaj, porcentaj_adic, porcentaj_objetiv Como Real
	tiemp_serv = 0; salario = 0; aument_bonifi = 0
	Escribir "Ingrese su tiempro de servicio:"; Leer tiemp_serv
	Escribir "Ingrese su salario actual:"; Leer salario
	Escribir "Ingrese el porcentaje del cumplimiento de sus objetivos:"; Leer porcentaj_objetiv
	Si tiemp_serv <= 1 Entonces
		porcentaj = 5
	SiNo
	Si tiemp_serv > 1 y tiemp_serv < 3 Entonces
	porcentaj = 12
	SiNo
	Si tiemp_serv >= 3 y tiemp_serv < 7 Entonces
	porcentaj = 18
	SiNo
	Si tiemp_serv >= 7 y tiemp_serv < 10 Entonces
	porcentaj = 22
	SiNo
	Si tiemp_serv >= 10 Entonces
	porcentaj = 25
	FinSi
	FinSi
	FinSi
	FinSi
	FinSi
	Si porcentaj_objetiv < 70 Entonces
	porcentaj_adic = 0
	SiNo
	Si porcentaj_objetiv >= 70 y  porcentaj_objetiv <= 85 Entonces
	porcentaj_adic = 3
	SiNo
	Si porcentaj_objetiv >= 86 y  porcentaj_objetiv <= 95 Entonces
	porcentaj_adic = 7
	SiNo
	Si porcentaj_objetiv > 96 Entonces
	porcentaj_adic = 10
	FinSi
	FinSi
	FinSi
	FinSi
	// SALIDAS
	aument_bonifi = salario + (salario * (porcentaj / 100))
	Escribir "Su salario base era: " salario "$"
	Escribir "Y su tiempo de servicio fue de: " tiemp_serv " años"
	Escribir "Usted tuvo un cumplimiento de objetivos del " porcentaj_objetiv "% por su tiempo de servicio"
	Escribir "=============================================================="
	Escribir "Usted ha recibido un aumento del " porcentaj "% que es igual a " (salario * (porcentaj / 100)) "$"
	
	aument_bonifi = aument_bonifi + (aument_bonifi * (porcentaj_adic / 100))
	Si porcentaj_adic = 0 Entonces
		Escribir "Usted no recibio una bonificacion adicional por el cumplimiento de sus obejtivos"
	SiNO
		Escribir "Adicionalmente usted ha recibido una bonificacion del " porcentaj_adic "% que es igual a " (aument_bonifi * (porcentaj_adic / 100)) "$ por el cumplimiento de sus obejtivos"
	FInSi
	Escribir "=============================================================="
	
	Escribir "Su nuevo sueldo mensual total de: " aument_bonifi "$"
	
FinProceso
