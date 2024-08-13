# **Sistemas Numéricos**

## [Diagrama de bloques](https://www.canva.com/design/DAGM1w6OFVg/VN4pSBaU0jzyD-zDFbis5g/edit?utm_content=DAGM1w6OFVg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## **Ejemplos**

1. El módulo de codificación solicita información de velocidad, altitud y temperatura al módulo de sensores, el cual envía como respuesta los siguientes tres datos en el orden respectivo: **00100101100**, **00110000110101000**, **0000000101101**. El módulo de codificación recibe la información y agrega bit de paridad y bits de encabezado así: **00000000000100101100**, **00010110000110101000**, **00100000000000101101**. Los datos son enviados al módulo de decodificación, el cual  determina la procedencia de los mismos, que estos no lleven errores y remueve los bits de encabezado y paridad y entrega los datos así: **00000000000100101100** (velocidad), **00000110000110101000** (altitud), **00000000000000101101** (temperatura). En este punto, el sistema se divide en tres procesos que se realizan uno luego del otro, uno para cada dato generado:
   - **(Velocidad):** el dato de velocidad es recibido por el módulo de conversión Bin2Dec y es reescrito como **300**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **350** y se produce un valor de error de **50**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000110010**. El módulo de control toma el dato y lo múltiplica por la constante **1100** así:

      | | | | | | | | | | |
      |-|-|-|-|-|-|-|-|-|-|
      | | | | |1|1|0|0|1|0|
      | | | | |x| |1|1|0|0|
      | | | | |-|-|-|-|-|-|
      | | | | |0|0|0|0|0|0|
      | |+| |0|0|0|0|0|0| |
      | | |1|1|0|0|1|0| | |
      | |1|1|0|0|1|0| | | |
      |-|-|-|-|-|-|-|-|-|-|
      |1|0|0|1|0|1|1|0|0|0|

     El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error.

    ‎ 


    - **(Altitud):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **25000**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **26000** y se produce un valor de error de **1000**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000001111101000**. El módulo de control toma el dato y lo múltiplica por la constante **1100** así:

      | | | | | | | | | | | | | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      | | | | |1|1|1|1|1|0|1|0|0|0|
      | | | | |x| | | | | |1|1|0|0|
      | | | | |-|-|-|-|-|-|-|-|-|-|
      | | | | |0|0|0|0|0|0|0|0|0|0|
      | |+| |0|0|0|0|0|0|0|0|0|0| |
      | | |1|1|1|1|1|0|1|0|0|0| | |
      | |1|1|1|1|1|0|1|0|0|0| | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      |1|0|1|1|1|0|1|1|1|0|0|0|0|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error. 
        
    ‎ 


    - **(Temperatura):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **45**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **50** y se produce un valor de error de **101**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000000101**. El módulo de control toma el dato y lo múltiplica por la constante **1100** así:

      | | | | | | |
      |-|-|-|-|-|-|
      | | |1|1|0|0|
      | | |x|1|0|1|
      | | |-|-|-|-|
      |+| |1|1|0|0|
      | |0|0|0|0| |
      |1|1|0|0| | |
      |-|-|-|-|-|-|
      |1|1|1|1|0|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error. 

‎ 

‎ 

2. El módulo de codificación solicita información de velocidad, altitud y temperatura al módulo de sensores, el cual envía como respuesta los siguientes tres datos en el orden respectivo: **00010010110**, **00010111011100000**, **0000000010100**. El módulo de codificación recibe la información y agrega bit de paridad y bits de encabezado así: **00000000000010010110**, **00010010111011100000**, **01100000000000010100**. Los datos son enviados al módulo de decodificación, el cual  determina la procedencia de los mismos, que estos no lleven errores y remueve los bits de encabezado y paridad y entrega los datos así: **00000000000010010110** (velocidad), **00000010111011100000** (altitud), **00000000000000010100** (temperatura). En este punto, el sistema se divide en tres procesos que se realizan uno luego del otro, uno para cada dato generado:
   - **(Velocidad):** el dato de velocidad es recibido por el módulo de conversión Bin2Dec y es reescrito como **150**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **160** y se produce un valor de error de **10**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000001010**. El módulo de control toma el dato y lo múltiplica por la constante **1010** así:

      | | | | | | | |
      |-|-|-|-|-|-|-|
      | | | |1|0|1|0|
      | | |x|1|0|1|0|
      | | |-|-|-|-|-|
      | | | |0|0|0|0|
      |+| |1|0|1|0| |
      | |0|0|0|0| | |
      |1|0|1|0| | | |
      |-|-|-|-|-|-|-|
      |1|1|0|0|1|0|0|

     El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error.

    ‎ 


    - **(Altitud):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **12000**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **20000** y se produce un valor de error de **8000**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000001111101000**. El módulo de control toma el dato y lo múltiplica por la constante **1100** así:

      | | | | | | | | | | | | | | | | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      | | | | |1|1|1|1|1|0|1|0|0|0|0|0|0|
      | | | | |x| | | | | | | | |1|0|1|0|
      | | | | |-|-|-|-|-|-|-|-|-|-|-|-|-|
      | | | | |0|0|0|0|0|0|0|0|0|0|0|0|0|
      | |+| |1|1|1|1|1|0|1|0|0|0|0|0|0| |
      | | |0|0|0|0|0|0|0|0|0|0|0|0|0| | |
      | |1|1|1|1|1|0|1|0|0|0|0|0|0| | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      |1|0|0|1|1|1|0|0|0|1|0|0|0|0|0|0|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error. 
        
    ‎ 


    - **(Temperatura):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **20**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **25** y se produce un valor de error de **101**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000000101**. El módulo de control toma el dato y lo múltiplica por la constante **1010** así:

      | | | | | | |
      |-|-|-|-|-|-|
      | | |1|0|1|0|
      | | |x|1|0|1|
      | | |-|-|-|-|
      |+| |1|0|1|0|
      | |0|0|0|0| |
      |1|0|1|0| | |
      |-|-|-|-|-|-|
      |1|1|0|0|1|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error. 

‎ 

‎ 

3. El módulo de codificación solicita información de velocidad, altitud y temperatura al módulo de sensores, el cual envía como respuesta los siguientes tres datos en el orden respectivo: **00001100100**, **00111010100110000**, **0000000011110**. El módulo de codificación recibe la información y agrega bit de paridad y bits de encabezado así: **01000000000001100100**, **00010111010100110000**, **01100000000000011110**. Los datos son enviados al módulo de decodificación, el cual  determina la procedencia de los mismos, que estos no lleven errores y remueve los bits de encabezado y paridad y entrega los datos así: **00000000000001100100** (velocidad), **00000111010100110000** (altitud), **00000000000000011110** (temperatura). En este punto, el sistema se divide en tres procesos que se realizan uno luego del otro, uno para cada dato generado:
   - **(Velocidad):** el dato de velocidad es recibido por el módulo de conversión Bin2Dec y es reescrito como **100**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **120** y se produce un valor de error de **20**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000010100**. El módulo de control toma el dato y lo múltiplica por la constante **1111** así:

      | | | | | | | | | |
      |-|-|-|-|-|-|-|-|-|
      | | | | |1|0|1|0|0|
      | | | | |x|1|1|1|1|
      | | | | |-|-|-|-|-|
      | | | | |1|0|1|0|0|
      | |+| |1|0|1|0|0| |
      | | |1|0|1|0|0| | |
      | |1|0|1|0|0| | | |
      |-|-|-|-|-|-|-|-|-|
      |1|0|0|1|0|1|1|0|0|

     El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error.

    ‎ 


    - **(Altitud):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **30000**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **28000** y se produce un valor de error de **2000**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000011111010000**. El módulo de control toma el dato y lo múltiplica por la constante **1111** así:

      | | | | | | | | | | | | | | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      | | | | |1|1|1|1|1|0|1|0|0|0|0|
      | | | | |x| | | | | | |1|1|1|1|
      | | |-|-|-|-|-|-|-|-|-|-|-|-|-|
      | | | | |1|1|1|1|1|0|1|0|0|0|0|
      | |+| |1|1|1|1|1|0|1|0|0|0|0| |
      | | |1|1|1|1|1|0|1|0|0|0|0| | |
      | |1|1|1|1|1|0|1|0|0|0|0| | | |
      |-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
      |1|1|1|0|1|0|1|0|0|1|1|0|0|0|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error. 
        
    ‎ 


    - **(Temperatura):** el dato de altitud es recibido por el módulo de conversión Bin2Dec y es reescrito como **30**. El dato es dirigido al módulo de cálculo de error donde se toma como SetPoint **28** y se produce un valor de error de **10**. El dato es recibido por el módulo de conversión Dec2Bin y reecrito como **00000000000000000010**. El módulo de control toma el dato y lo múltiplica por la constante **1111** así:

      | | | | | |
      |-|-|-|-|-|
      | |1|1|1|1|
      | |x| |1|0|
      | |-|-|-|-|
      |+|0|0|0|0|
      |1|1|1|1| |
      |-|-|-|-|-|
      |1|1|1|1|0|

        El dato arrojado por el módulo anterior es llevado al módulo de codificación de la CPU y de esta forma corregir el error.