[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ZHlrD2sU)

# **En una computadora**
## *Mapa conceptual*
![Texto alternativo](https://www.canva.com/design/DAGL62geJ8A/VYUKzAKizNXZ7kGqR1XaTA/view?utm_content=DAGL62geJ8A&utm_campaign=designshare&utm_medium=link&utm_source=editor)

## *Veamos más a fondo*
### ¿Cómo interactúa el hardware con el software, cuál es la función de cada uno?
Debemos entender a hardware y software como la esencia musma de la computador. El hardware tiene como trabajo principal recibir, procesar, almacenar y entregar datos. A su vez, el software se encarga en primera medida de gestionar los recursos del sistema, interactuar con el ususario y ejecutar tareas y aplicaciones.

![Texto alternativo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fes.pinterest.com%2Fpin%2Fdiagnostico-informtica--140878294586942798%2F&psig=AOvVaw2egKaBhJOlwOFWnrZCimhn&ust=1721964899251000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCPCipKihwYcDFQAAAAAdAAAAABAK)

El Kernel o núcleo, es una parte fundamental del sistema operativo que se encarga de conceder el acceso al hardware de forma segura para todo el software que lo solicita, el Kernel es una pequeña e invisible parte del sistema operativo, pero la más importante, ya que sin esta no podría funcionar. Todos los sistemas operativos tienen un Kernel. **Ejemplifiquemos:** el usuario interactúa con el hardware a través de dispositivos de entrada (teclado, ratón) y salida (monitor) y el sistema operativo.  Este último y las aplicaciones envían instrucciones al procesador (CPU) para realizar tareas específicas que a su vez utiliza la memoria RAM para almacenar temporalmente los datos que está procesando. Estos datos al igual que las aplicaciones se almacenan de manera permanente en discos duros o SSD. Al finalizar todos estos procesos, Los resultados son enviados a los dispositivos de salida (monitor, impresora) para que el usuario los vea y utilice.

### ¿Cuál es la función de la CPU y cuáles son sus partes más importantes?

La CPU (Unidad Central de Procesamiento) es el cerebro de la computadora. Sus funciones principales se centran en la ejecución de instrucciones y el procesamiento datos. Lo anterior trae consigo interpretar las instrucciones de los programas de software; coordinar los datos que se mueven entre la memoria, los perífericos y otros componentes de la computadora; realizar operaciones aritméticas y lógicas necesarias para la ejecución de programas. Las partes más importantes de la CPU son:

- **Unidad de Control (CU):** se encarga de dirigir las operaciones, por lo tanto, realiza las funciones principales  de la CPU. Además, controla el flujo de datos entre la CPU y otros componentes del sistema.

- **Unidad Aritmético-Lógica (ALU):** como su nombre lo indica, realiza operaciones aritméticas y lógicas, siendo así responsable de todos 0los cálculos y decisiones lógicas dentro de la CPU.

- **Registros:** son pequeñas áreas de almacenamiento de alta velocidad para datos temporales y direcciones de memoria que son necesarios para la ejecución de instrucciones.

- **Cache:** es una memoria de alta velocidad que se ubicada cerca del núcleo de la CPU y se encarga de almacenar copias de datos e instrucciones frecuentemente utilizados para acelerar el acceso a la memoria.

- **Bus de Datos:** es el canal de comunicación que transporta datos entre la CPU y otros componentes del sistema.

![Texto alternativo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fconcepto.de%2Fcpu%2F&psig=AOvVaw2w3kz-oAWJm3kWjDESsPnl&ust=1721966191640000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCLiwiZCmwYcDFQAAAAAdAAAAABAE)

### ¿Qué es la velocidad de la CPU?

La velocidad de la CPU, también conocida como velocidad del reloj, es la medida de cuántas operaciones básicas puede realizar la CPU por segundo. Se mide en hercios (Hz), generalmente en gigahercios (GHz) para las CPUs modernas.

![Texto alternativo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.datacentermarket.es%2Fdcm-xl%2Fcpu-unidad-central-de-procesamiento-guia-completa%2F&psig=AOvVaw2w3kz-oAWJm3kWjDESsPnl&ust=1721966191640000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCLiwiZCmwYcDFQAAAAAdAAAAABAJ)

### ¿Cuál es la secuencia de pasos que ocurre, desde el momento en que presionas el botón de encendido de la computadora, hasta que se muestra el sistema operativo listo para funcionar?

La secuencia que la computador debe realizar solo para iniciar su sistema operativo es largo y complejo:

1. **Presión del Botón de Encendido:** se activa la fuente de alimentación (PSU), que suministra energía eléctrica a todos los componentes de la computadora.

2. **POST (Power-On Self Test):** la BIOS realiza una serie de pruebas de diagnóstico básicas para verificar que los componentes de hardware estén funcionando correctamente.
Se verifica la memoria RAM, la CPU, los dispositivos de almacenamiento, el teclado y otros componentes esenciales.

3. **Carga de la BIOS:** la BIOS configura el hardware de la computadora y prepara el entorno necesario para que el sistema operativo se cargue. Configura los controladores básicos y establece la configuración inicial del hardware.

4. **Detección de Dispositivos de Almacenamiento:** la BIOS detecta los dispositivos de almacenamiento conectados. 

5. **Carga del Bootloader:** dependiendo del Bootloader con el que cuente la compuadora se iniciará una u otra parte del disco.

6. **Ejecutar el Bootloader:** el bootloader se carga en la memoria RAM. Este se responsabilizada de cargar el núcleo del sistema operativo en la memoria.

7. **Carga del Kernel del Sistema Operativo:** el bootloader carga el kernel del sistema operativo en la memoria y transfiere el control a este. El kernel inicializa los controladores de hardware y configura el entorno de ejecución.

8. **Inicialización del Sistema Operativo:** el kernel del sistema operativo inicia los procesos y servicios esenciales necesarios para el funcionamiento del sistema.

9. **Carga de Controladores y Servicios:** el sistema operativo carga los controladores necesarios para el hardware detectado e inicia los servicios del sistema.

10. **Inicio de la Interfaz de Usuario:** el sistema operativo inicia la interfaz gráfica de usuario (GUI).

11. **Autenticación del Usuario:** se presenta la pantalla de inicio de sesión, donde el usuario ingresa sus credenciales, el sistema verifica las credenciales y carga el perfil del usuario.

12. **Preparación del Escritorio:** una vez autenticado, el sistema operativo carga las configuraciones personales del usuario, los programas de inicio, y los iconos del escritorio.

![Texto alternativo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcomputerhoy.com%2Ftutoriales%2Ftecnologia%2Ftres-maneras-acceder-opciones-arranque-windows-10-windows-11-1077031&psig=AOvVaw3Sch84sTboSx6-jaXC-0qc&ust=1721967726065000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJj-4vCrwYcDFQAAAAAdAAAAABAE)

### **DATO CURIOSO**

Primer "Bug" Informático:

El término "bug" para referirse a un error en el software tiene una historia curiosa. En 1947, mientras trabajaba en la computadora Mark II en Harvard, los ingenieros encontraron una polilla atrapada en uno de los relés de la máquina, lo que causaba un mal funcionamiento. La polilla fue removida y pegada en el libro de registro con la nota "First actual case of bug being found" (primer caso real de un "bicho" encontrado). Desde entonces, el término "bug" se ha utilizado para describir errores o fallos en los programas de computadora.

![Texto alternativo](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.adslzone.net%2Fnoticias%2Ftecnologia%2Fpor-que-fallo-informatica-llama-bug%2F&psig=AOvVaw223Jr6SHe2ViBu98cNEqEf&ust=1721967933491000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCNik0cyswYcDFQAAAAAdAAAAABAE)

## REFERENCIAS BIBLIOGRÁFICAS

