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

```
#Ejercicio 14
```Bash
n=$1
for ((i=0;i<=n;i++))
do
  echo $i
done
```
#Ejercicio 15
```Bash
n=$1
sum=0
for ((i=1;i<=n;i++))
do
  sum=$((sum+i))
done
echo $sum
```
#Ejercicio 16
```Bash
a=$1
b=$2
temp=$a
a=$b
b=$temp
echo "a: $a"
echo "b: $b"
```
#Ejercicio 17
```Bash
while true
do
  read -p "Ingrese una palabra (escriba ':q' para salir): " palabra
  if [ $palabra = ":q" ]
  then
    break
  fi
done
```
#Ejercicio 18
```Bash

```
#Ejercicio 19
```Bash
echo "Escribe palabras para guardar en un archivo (':q' para salir): "
read palabra

while [[ $palabra != ":q" ]]; do
    echo $palabra >> palabras.txt
    read palabra
done
echo "Las palabras han sido guardadas en 'palabras.txt'."
```
#Ejercicio 20
```Bash
echo "Escriba un número para comprobar si se encuentra en el archivo 'numeros.txt': "
read numero

if grep -Fxq "$numero" numeros.txt
then
    echo "El número $numero está en el archivo 'numeros.txt'."
else
    echo "El número $numero no está en el archivo 'numeros.txt'."
fi
```
