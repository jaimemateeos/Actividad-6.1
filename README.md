# Actividad-6.1



#Ejercicio 1
```Bash
echo "Ingresa un número:"
read numero

if [ $numero -ge "0" ]; then 
    echo "El número $numero es positivo"
else 
    echo "El numero $numero no es positivo"
fi
```
#Ejercicio 2
```Bash
echo "Ingresa un número:"
read numero

if [ $numero -lt "0" ]; then 
    echo "El número $numero es negativo"
else 
    echo "El numero $numero no es negativo"
fi
```
#Ejercicio 3
```Bash
echo "Ingresa un número:"
read numero

if [ $numero -eq "0" ]; then 
    echo "El número es igual a cero"
else
    echo "El número no es cero"
fi
```
#Ejercicio 4
```Bash
echo "Ingresa un número:"
read numero

if [ $numero -ge "0" ]; then 
    echo "El número $numero es positivo"
elif [ $numero -lt "0" ]; then
    echo "El numero $numero es negativo"
else
    echo "El número es cero"
fi
```
#Ejercicio 5
```Bash
if [ $# -eq "3" ]; then 
    echo "Numero de parámetros correcto"
else
    echo "ERROR."
fi
```
#Ejercicio 6
```Bash
if [ $# -ne 2 ]; then
    echo "Error: Numero de parámetros incorrecto."
else
    suma=$(expr $1 + $2)
    echo "La suma es: $suma"
fi
```
#Ejercicio 7
```Bash
```
#Ejercicion 8
```Bash
if [ $# -ne 1 ]; then
    echo "Error: Se necesita 1 parámetro."
elif [ -e $1 ]; then
    echo "El archivo $1 existe"
else
    echo "El archivo $1 no existe"
fi
```
#Ejercicio 9
```Bash
if [ $# -ne 1 ]; then
  echo "Error: se necesita exactamente 1 parámetro"
elif [ -f $1 ]; then
  echo "$1 es un archivo"
elif [ -d $1 ]; then
  echo "$1 es un directorio"
else
  echo "No se pudo determinar si $1 es un archivo o un directorio"
fi
```
#Ejercicio 10
#Ejercicio 11
```Bash
for i in {1..50}
do
  echo "hola"
done
```
#Ejercicio 12
```Bash
for i in {1..10}
do
  read -p "Introduce una palabra: " palabra
  echo "La palabra introducida es: $palabra"
done
```
#Ejercicio 13
```Bash
if [ -z "$1" ]; then
  echo "Debes indicar un número como parámetro"
else
  n=$1
  for i in $(seq 1 $n)
  do
    echo "hola"
  done
fi
```
#Ejercicio 14

#Ejercicio 15
#Ejercicio 16
#Ejercicio 17
#Ejercicio 18
#Ejercicio 19
#Ejercicio 20
