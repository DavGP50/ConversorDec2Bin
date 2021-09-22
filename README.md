# ConversorDec2Bin
s="Python syntax highlighting"
print s
def dec2bin(numero_decimal, numero_bits):
    numero_binario = bin(numero_decimal)
    numero_binario = numero_binario[2:len(numero_binario)]  # quita el "0b" del principio
    while len(numero_binario) < numero_bits:      # añade 0's a la izquierda si hace falta
        numero_binario = "0" + numero_binario
    if numero_decimal>=0:
        numero_binario = numero_binario[2:len(numero_binario)]  # quita el "0b" del principio
        while len(numero_binario) < numero_bits:      # añade 0's a la izquierda si hace falta
            numero_binario = "0" + numero_binario
    else:
        numero_binario=numero_binario[3:len(numero_binario)]    #quita el "-0b" del principio
        while len(numero_binario)<numero_bits:  #añade 1's a la izquierda si hace falta
            numero_binario="1"+numero_binario
    return numero_binario
