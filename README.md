# MICROCONTROLADOR 

## 1. SEÑALES

|                        Digitales                       |                       Analógicas                      |
|:------------------------------------------------------:|:-----------------------------------------------------:|
| Solo 2 posibles valores o estados, su onda es cuadrada | Puede tomar cualquier valor en  el dominio del tiempo |

## 2. Puertos de entrada y salida

- Son el medio o la interfaz por medio del cúal el microcontrolador recibe y entrega información desde y hacia el entorno respectivamente
- Interfaz bidireccional
- Se hace a través de puertos de conexión físicos que permiten la conducción de señales eléctricas

## 3. I/O digitales

- Si se miden las señales de voltaje de entrada y salida con un multímetro, se observa una señal análoga con un valor determinado
  
- Desde el punto de vista del microcontrolador se tiene uno de dos valores lógicos “1”(nivel alto) o “0” (nivel bajo)

## 4. Se puede conectar

|       Entrada       | Procesamiento    |         Salida         |
|:-------------------:|------------------|:----------------------:|
| Receptor infrarrojo | Microcontrolador |         Motor          |
|   Foto resistencia  | Microcontrolador | Transmissor infrarrojo |
|      Microfono      | Microcontrolador |         Altavoz        |
|    Interruptores    | Microcontrolador |                        |

## 5. Puertos digitales I/O

- Generalmente el Puerto digital es un grupo de 8 pines de conexión (No es una regla)
- Pueden ser de entrada, salida o bidireccionales
- Un microcontrolador generalmente tiene varios puertos
- Estos pines tambien son utilizados por diferentes módulos del microcontrolador

### 5.1 Componentes típicos de los puertos digitales

>  🔑 Data direction register (DDR): Es un registro que almacena la configuración del Puerto. Si se quiere usar como entrada o como salida

>  🔑 Port Register (PORT): Este registro almacena el equivalente lógico de los niveles de tensión que se encuentran en los pines de conexión eléctrica

>  🔑 Port Input Register (PIN): Generalmente es solo de lectura y contiene el estado actual de todos los pines

  - En la mayoría de microcontroladores es posible accesar
  estos registros modificando el byte completo o solo uno
  de los bit. 
    - Por ejemplo el PIC

## 6. Entradas Digitales

Se usan para interpretar los niveles de tensión monitoreados (leídos) desde hardware interior: 
  - 1 lógico corresponde a un nivel alto ("HIGH")
  - 0 lógico corresponde a un nivel bajo ("LOW")

Rangos de tensión indefinidos 

## 7. Rangos de tensión indefinidos 

- Pueden haber valores indefinidos de voltaje, lo cual puede llevar a:
  - Nivel alto
  - Nivel bajo
  - Nivel indeterminado
  - Oscilación
    
Para evitar los 2 ultimos, los microcontroladores incluyen un Schmitt Trigger (Comparador)

## 8. Resistencias de pull

- La mayoría de los microcontroladores cuentan con resistencias de pull-up o pull-down para facilitar el uso de interruptores externos en los pines de conexión de los puertos de entrada
  - Se habilitan por medio de registros

## 9. Salidas Digitales

Maneja unos rangos y mínimos en la salida dependiendo de la familia de microcontrolador

- Por ejemplo ATmega16:
  - Máxima tensión en estado “low” es 0.7 V
  - Mínima tensión en estado “high” es 4.2 V

- En el caso de las salidas se recomiendo utilizar protecciones para evitar daños en los puertos

### 9.1 Caracteísticas 

- Si el registro DDR se configura como salida, se conecta el pin al registro PORT
- Es más critico usar los pines como salidas que como entradas, ya que los microcontroladores no tienen protecciones internas
- El diseñador debe establecer una estrategia de protección para que no se presenten cortos en los pines de salida
- " Estado seguro de arranque "

## 10. Conclusiones

- Entender el valor que pueden tomar el tipo de señales digitales
- Identificar la funcion de los puertos I/O y como se comunican con el exterior
- Analizar sus aplicaciones industriales para controlar dispositivos como motores, sensores y pantallas mediante señales digitales.

## 11. Autores

### Luis Fernando Pulido Salazar - 76257
### Heisen Jawer Diaz Ascencio - 137604
  
