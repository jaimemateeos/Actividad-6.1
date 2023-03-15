# Actividad-6.1



#Ejercicio 1
echo "Ingresa un número:"
read numero

if [ $numero -ge "0" ]; then 
    echo "El número $numero es positivo"
else 
    echo "El numero $numero no es positivo"
fi

#Ejercicio 2
echo "Ingresa un número:"
read numero

if [ $numero -lt "0" ]; then 
    echo "El número $numero es negativo"
else 
    echo "El numero $numero no es negativo"
fi

#Ejercicio 3
echo "Ingresa un número:"
read numero

if [ $numero -eq "0" ]; then 
    echo "El número es igual a cero"
else
    echo "El número no es cero"
fi

#Ejercicio 4
echo "Ingresa un número:"
read numero

if [ $numero -ge "0" ]; then 
    echo "El número $numero es positivo"
elif [ $numero -lt "0" ]; then
    echo "El numero $numero es negativo"
else
    echo "El número es cero"
fi

#Ejercicio 5
if [ $# -eq "3" ]; then 
    echo "Numero de parámetros correcto"
else
    echo "ERROR."
fi

#Ejercicio 6
if [ $# -ne 2 ]; then
    echo "Error: Numero de parámetros incorrecto."
else
    suma=$(expr $1 + $2)
    echo "La suma es: $suma"
fi

#Ejercicio 7

#Ejercicion 8
if [ $# -ne 1 ]; then
    echo "Error: Se necesita 1 parámetro."
elif [ -e $1 ]; then
    echo "El archivo $1 existe"
else
    echo "El archivo $1 no existe"
fi
#Ejercicio 9
