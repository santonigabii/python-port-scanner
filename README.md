# python-port-scanner
#!/usr/bin/python3
# Inteiros
# Strings
# Float 

import sys

def somar (numero1, numero2):
        return numero1 + numero2

def dividir(numero1, numero2):
        try:
                resultado = numero1 / numero2
        except ZeroDivisionError:
                resultado = "indefinido"

        return resultado 

if len(sys.argv) >= 3:
    if sys.argv[1].isdigit() and sys.argv[2].isdigit():
        primeiro_numero = int(sys.argv[1])
        segundo_numero = int(sys.argv[2])

        print("A soma do primeiro numero com o segundo e:", somar(primeiro_numero, segundo_numero))
        print("A divisao do primeiro numero com o segundo e:",dividir( primeiro_numero, segundo_numero))
    else:
        print("Os valores precisam ser numericos")
else:
    print("Passe como argumento dois numeros")
