## Creación de entrada Serial Virtual 

* Instalar com0com  
  https://com0com.sourceforge.net


* Crear puerto Serial Virtual

  Ejecutar **Setup for com0com**

  ![alt text](/img/image.png)

* Uso 

  Si se escribe en COM6 se puede leer en COM5  
  Si se escribe en COM5 se puede leer en COM6

* Ejemplo con Python 

``` python
# Escribir en COM6
import serial   
import time

ser = serial.Serial('COM6', 9600)
while True:
    ser.write(b'Hola desde COM6\n')
    time.sleep(1)
``` 
``` python
# Leer en COM5 
import serial

ser = serial.Serial('COM5', 9600)
while True:
    data = ser.readline().decode(errors='ignore').strip()
    print(f"Recibido: {data}")
``` 
* Instalar libreria 

pip install pyserial

* Prueba 

![alt text](/img/image2.png)
