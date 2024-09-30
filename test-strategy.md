
--primer error
    guessSubmit.addeventListener('click', checkGuess);
--Solucion: Cambiar addeventListener por addEventListener (La letra e tiene que estar en mayuscula)


--Segundo error
    const lowOrHi = document.querySelector('lowOrHi');
--Solucion: Le falta el punto antes de "lowOrHi" que esta en parentesis, seria ('.lowOrHi') 


--Tercer error (Linea 95)
	resetButton.addeventListener('click', resetGame);
--Solucion: Cambiar addeventListener por addEventListener (La letra e tiene que estar en mayuscula)

--Cuarto error (Linea 45)
    let randomNumber = Math.random() * 10;
--Usamos Math.floor para que el numero se genere bien del 1 al 100 y como entero,


--Quinto error (Linea 65 y 70)
    lastResult.textContent = '!!!Pérdistes!!!'; (Linea 65)
    lastResult.textContent = 'Felicitaciones! adivinaste el número!'; (Linea 70)
--Solucion: Invertimos el orden de fila de estos codigos, ya los codigos estan cruzados en cuestiones de logica

--Sexto error
const ATTEMPS = 5;
--Solucion: Se cambio el total de numeros solicitados a 10 como lo pide el programa

--7mo error
A este codigo: let userGuess = Number(guessField.value);

Se le agrego:
            let userGuess = Number(guessField.value);
            if (isNaN(userGuess)) {
            alert("Por favor ingresa un numero entero.");
            return;
            }
--Solucion: Se le agrego el codigo con el fin de asegurarse que la entrada sea si o si numero entero


------------------Se agregaron 2 validaciones extras-----------------------------

Cuando el usuario Adivina indicar cual era el numero que adivino:  El numero es: ' + randomNumber;
Cuando el usuario no Adivina indicar cual era el numero que no adivino:  El numero era: ' + randomNumber;




