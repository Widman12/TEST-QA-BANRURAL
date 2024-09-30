
--Primer error (Linea 91)
    guessSubmit.addeventListener('click', checkGuess);
--SOLUCION: Cambiar addeventListener por addEventListener (La letra e tiene que estar en mayuscula)


--Segundo error (Linea 49)
    const lowOrHi = document.querySelector('lowOrHi');
--SOLUCION: Le falta el punto antes de "lowOrHi" que esta en parentesis, seria ('.lowOrHi') 


--Tercer error (Linea 95)
	resetButton.addeventListener('click', resetGame);
--SOLUCION: Cambiar addeventListener por addEventListener (La letra e tiene que estar en mayuscula)


--Cuarto error (Linea 45)
    let randomNumber = Math.random() * 10;
--SOLUCION: Usamos Math.floor para que el numero se genere bien del 1 al 100 y como entero,


--Quinto error (Linea 65 y 70)
    lastResult.textContent = '!!!Pérdistes!!!'; (Linea 65)
    lastResult.textContent = 'Felicitaciones! adivinaste el número!'; (Linea 70)
--SOLUCION: Invertimos el orden de fila de estos codigos, ya los codigos estan cruzados en cuestiones de logica


--Sexto error (Linea 46)
const ATTEMPS = 5; 
--SOLUCION: Se cambio el total de numeros solicitados a 10 como lo pide el programa (const ATTEMPS = 10; )


--7mo error (Linea 58 a la 61)
A este codigo: let userGuess = Number(guessField.value);
Se le agrego:
            let userGuess = Number(guessField.value);
            if (isNaN(userGuess)) {
            alert("Por favor ingresa un numero entero.");
            return;
            }
--SOLUCION:: Se le agrego el codigo con el fin de asegurarse que la entrada sea si o si numero entero


------------------Se agregaron 2 validaciones extras-----------------------------
(Linea 69)
Cuando el usuario Adivina indicar cual era el numero que adivino:  El numero es: ' + randomNumber;
SOLUCION: Esto se agrego con el fin de que el usuario sepa que numero adivino, podria ser confuso no resaltar el numero que adivino
(Linea 74)
Cuando el usuario no Adivina indicar cual era el numero que no adivino:  El numero era: ' + randomNumber;
SOLUCION: Esto se agrego con el fin de que el usuario sepa que numero no adivino, se ve mejor indicar que numero no adivino.




