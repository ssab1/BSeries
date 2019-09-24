# BSeries
:alien:    :zzz:  :bike: 

## Somos una pagina encargada de entrega reseñas sobre series ya sea estas recientes, al igual que dar a conocer sobre sus actores

![Captura](https://user-images.githubusercontent.com/51329760/64754230-d3b1c200-d4fc-11e9-9f74-441775b8b5ea.PNG)



![Captura5](https://user-images.githubusercontent.com/51329760/64754343-53d82780-d4fd-11e9-9b4c-eb4b85df5cf0.PNG)

![Captura4](https://user-images.githubusercontent.com/51329760/64754251-ee843680-d4fc-11e9-8ebc-01a52ed60270.PNG)
Bastian Santibañez :alien:
Bruny Vidal :zzz:
#!/bin/bash



SUMAR() {
echo "ingrese el primer numero"
read n
echo "ingrese el segundo mumero"
read s
oper=$(( $n + $s ))
echo "El resultado es:" $oper
}

RESTAR() {
echo "ingrese el primer numero"
read n
echo "ingrese el segundo mumero"
read s
oper=$(( $n - $s ))
echo "El resultado es:" $oper

}
MULTIPLICAR() {
echo "ingrese el primer numero"
read n
echo "ingrese el segundo mumero"
read s
oper=$(( $n * $s ))
echo "El resultado es:" $oper

}
DIVIDIR() {
echo "ingrese el primer numero"
read n
echo "ingrese el segundo mumero"
read s
if [ $s -eq 0 ] ; then
echo "no se puede dividir por cero" 
else
oper=$(( $n / $s ))
echo "El resultado es:" $oper

fi

}

opc=0
while [ $opc -ne 5 ] ; do
clear
echo "-----------"
echo "Calculadora"
echo "-----------"
 
echo "Ingrese opcion de lo que desea realizar:
1.-sumar
2.-restar
3.-multiplicar
4.-dividir
5.-salir"
read opc
echo "---------------------------------------"


case $opc in

1)SUMAR;;
2)RESTAR;;
3)MULTIPLICAR;;
4)DIVIDIR;;
esac
sleep 2

done

