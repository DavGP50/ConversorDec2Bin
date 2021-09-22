# ConversorDec2Bin
Con este código podemos pasar de un número decimal a un número binario, además de poder elegir la cantidad de cifras con las que se nos devolverá la respuesta.
```python
    def dec2bin(numero_decimal, numero_bits):
        numero_binario = bin(numero_decimal)
        numero_binario = numero_binario[2:len(numero_binario)]  
        while len(numero_binario) < numero_bits:      
            numero_binario = "0" + numero_binario
        if numero_decimal>=0:
            numero_binario = numero_binario[2:len(numero_binario)
            while len(numero_binario) < numero_bits:      
                numero_binario = "0" + numero_binario
        else:
            numero_binario=numero_binario[3:len(numero_binario)]    
            while len(numero_binario)<numero_bits:  
                numero_binario="1"+numero_binario
        return numero_binario
 ```
