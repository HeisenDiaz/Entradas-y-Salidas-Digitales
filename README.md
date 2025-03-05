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
