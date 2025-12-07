# WirelessCharger-PCB-IE0408
Repositorio para el proyecto final del curso IE0408 sobre el diseño de una PCB de un cargador inalambrico. Contiene el circuito esquemático, el diseño de la PCB en *KiCad* y documentación sobre los componentes a utilizar, el procedimiento de diseño y otros detalles. 

Este repositorio y sus contenidos fueron diseñados durante el curso IE0408 durante el periodo II-2025 por los siguientes integrantes del equipo:

<div align="center">

|        **Integrantes**      | **Carné** | **Correo electrónico**|
|:---------------------------:|:---------:|:---------------------:|
|    Anthony Calvo García     |   C11433  |  anthonycalvo50@gmail.com |
|   Rodrigo Madrigal Montes   |   C24458  | rmadrigalmontes@gmail.com |

</div>

## Agradecimientos a PCBWay

El proyecto presentado fue posible gracias al valioso respaldo de PCBWay, a quienes deseamos extender nuestro más sincero agradecimiento. Las PCBs entregadas mostraron ser de una excelente calidad durante las pruebas realizadas, además de que el acabado en cada una de ellas es sencillamente perfecto, superando todas nuestras expectativas.

Agradecemos, de igual manera, al equipo encargado de la atención al cliente, los cuales están siempre disponibles para brindar el apoyo solicitado de la forma más profesional, lo que nos dio mucha seguridad y tranquilidad durante todo el proceso de elaboración y entrega de las PCBs.


### Lista de componentes

A continuación se incluye una lista con los componentes utilizados en el diseño, con el mismo número que se les asignó en el diseño final de PCB:

<div align="center">

| Componente | Valor / Modelo | Descripción |
|:---:|:---:|:---:|
| C1, C8 | 10uF, 2.2uF | Capacitor de montaje superficial (SMD) |
| C2, C3 | 100nF | Capacitor de montaje superficial (SMD) |
| C4, C5 | 10nF | Capacitor de montaje superficial (SMD) |
| C6, C7 | 2nF | Capacitor de montaje superficial (SMD) |
| D1, D2 | 1N4148 | Diodo THT |
| D3, D4, D5, D6 | SS14 | Diodo Schottky SMD |
| J1, J2 | Screw_Terminal_01x02 | Terminal de tornillo (2 pines) |
| L1, L2 | Conn_01x02_Socket | Conector hembra (Socket) 1x02, paso 2.54mm |
| Q1 | BD139 | Transistor NPN de potencia (THT) |
| Q2 | IRFZ44N | Transistor MOSFET de potencia |
| R1 | 100Ω | Resistor de montaje superficial (SMD) |
| R3 | 150Ω | Resistor de montaje superficial (SMD) |
| R2| 1kΩ | Resistor de montaje superficial (SMD) |
| RV1, RV2 | 1kΩ | Resistor variable/Potenciómetro |
| U1 | NE555D | Circuito Integrado Temporizador NE555 (SMD) |
| TP1, TP3, TP6 | GND | Punto de prueba (Test Point) para Tierra (GND) |
| TP2 | OutTim | Punto de prueba (Test Point) para Salida del Temporizador |
| TP4 | RX | Punto de prueba (Test Point) para Recepción (RX) |
| TP5 | TX | Punto de prueba (Test Point) para Transmisión (TX)

</div>


## Diseño de la PCB

Una vez definido el circuito final, se diseñó la PCB en *KiCad* con una arquitectura de **cuatro capas**, las cuales se distribuyen de la siguiente manera:

- **F.Cu**: Ruta de señales
- **In1.Cu**: Plano de alimentación +9V
- **In2.Cu**: Plano de tierra (GND)
- **B.Cu**: Ruta de señales

### Capas de la PCB

<div align="center">

| ![Capa F.Cu](images/F_Cu.png) |
|:-----------------------------:|
|    *Capa superior (F.Cu)*     |

</div>

<div align="center">

| ![Capa B.Cu](images/B_Cu.png) |
|:-----------------------------:|
|    *Capa inferior (B.Cu)*     |

</div>

<div align="center">

| ![In1.Cu - Alimentación](images/In1_Cu.png) |
|:-------------------------------------------:|
|      *Capa interna 1 - +9*         |

</div>

<div align="center">

| ![In2.Cu - Tierra](images/In2_Cu.png) |
|:-------------------------------------:|
|        *Capa interna 2 - GND*         |

</div>

Además, se agregaron zonas de serigrafía, agujeros de montaje, así como textos identificativos y logotipos en el *silkscreen* con el nombre del proyecto y los autores. Como resultado final se muestra la PCB en el visor 3D de *KiCad* con y sin los modelos 3D 

<div align="center">

| ![Vista 3D Frontal de la PCB sin 3D](images/Front_3D_nc.png) |
|:--:|
| *Vista 3D Frontal de la PCB en KiCad* |

</div>

<div align="center">

| ![Vista 3D Frontal de la PCB sin 3D](images/Back_3D_nc.png) |
|:--:|
| *Vista 3D Frontal de la PCB en KiCad* |

</div>

<div align="center">

| ![Vista 3D Frontal de la PCB con Modelos](images/Front_3D.png) |
|:--:|
| *Vista 3D Frontal de la PCB en KiCad con modelos 3D* |

</div>

<div align="center">

| ![Vista 3D Trasera de la PCB con Modelos](images/Back_3D.png) |
|:--:|
| *Vista 3D Trasera de la PCB en KiCad con modelos 3D* |

</div>

<div align="center">

| ![Vista 3D Lateral Izquierda de la PCB con 3D](images/side_3D.png) |
|:--:|
| *Vista 3D Lateral Izquierda de la PCB en KiCad con modelos 3D* |

</div>
