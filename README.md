# calculadora-case-shellbox

  GNU nano 6.2                                                                                   calculadora3.sh *                                                                                          
!/bin/bash

echo "digite o primeiro numero"

read n1

echo "digite o segundo numero"

read n2

echo "voce deseja fazer soma, divisao, subtracao ou multiplicacao?"
echo "1 = add; 2=sub; 3=multi; 4=div"

read resp

case $resp in
1)
cal=$((n1+n2))
echo "a resposta e $cal"
;;
2)
cal=$((n1-n2))
echo  "a resposta e $cal"
;;
3)
cal=$((n1*n2))
echo  "a resposta e $cal"
;;
4)
cal=$((n1/n2))
echo  "a resposta e $cal"
;;
*)
echo  "digite algo valido"
;;
esac
