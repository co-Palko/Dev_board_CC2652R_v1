# Devboard_CC2652R_v1 (on development stage)
Development and universal sensor board, with zigbee RF-BM-2652B1 module. 

Устройство разработано на основе беспроводного модуля компании RF-Star, и включает в себя радиочастотный микроконтроллер ARM Cortex M4F поддерживающий протоколы: Thread,
Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4, IPv6-enabled (6LoWPAN), а также проприетарные протоколы включая TI 15.4-Stack (2,4 ГГц), и одновременную многопротокольную работу через Dynamic Multiprotocol Manager (DMM).  

Основная схемотехника функционально повторяет плату разработчика LAUNCHXL-CC26X2R1 Evaluation board, исключая средства отладки и мониторинга. Это позволяет использовать стандартные примеры программного обеспечения и библиотеки от указанной платы. 


![alt tag](https://github.com/co-Palko/Develop_board_CC2652R_v1/blob/main/images/TOP_assem.png)  

Форм-фактор платы расчитан как на применение в качестве  самостоятельного устройства с батарейным (батарея CR2032) либо внешним питанием (microUSB либо разъем), так и в качестве встраиваемого устройства для обеспечения сбора и передачи информации от различных датчиков и ввод внешних сигналов.  
Микроконтроллер имеет на борту стандартные порты ввода-вывода с 3.3 вольтовой логикой, выводы с повышенной нагрузочной способностью, выводы с возможностью АЦП и поддерживает набор стандартных интерфейсов (I2C, UART, SPI).  
По периметру платы располагаются контактные площадки с шагом 2,54мм, на которые выведены большинство выводов контроллера, включая питание, выводы программирования и отладки JTAG.  
Разработанная плата разведена на 2-х стороннем текстолите,  для заказа на производстве прилагаются [GERBER](https://github.com/co-Palko/Develop_board_CC2652R_v1/tree/main/gerber/) и BOM файлы, а размер компонентов подходит для самостоятельной сборки.  Принципальная схема устройства представлена по [ССЫЛКЕ](https://github.com/co-Palko/Develop_board_CC2652R_v1/blob/main/images/Devboard_mini_cc2652r-1.png).  
  
  
Изначально предусмотрены три стандартных 4-х контактных разъема 3.5мм, на которые выведены основные интерфейсные выводы микроконтроллера, а так же выводы питания подключаемых устройств (при этом есть возможность выбора его типа - постоянное питание 3.3В, либо питание от вывода с повышенной нагрузочной способностью для контроля и управления потреблением).  
При необходимости есть возможность отделения половины платы с интерфейсными разъемами 3.5мм для уменьшения внешних габаритов устройства.   
  
  
Конфигурация платы подразумевает возможность установки ее в фабрично изготовленный корпус типа [AK-W-48](https://myszomk.ru/product/ak-w-48) (SZOMK factory) либо [BMW50032-A1](https://aliexpress.ru/item/Wall-mounting-junction-box-for-electronic-plastic-enclosure-connector-diy-plastic-box-for-electronics-project-81/32906762106.html) (RTKLM factory) с минимальной доработкой для вывода разъемов.  
Исходные файлы для сборки прошивки находятся по [ССЫЛКЕ](https://github.com/diyruz/SensBoard)


# In English

The device is based on the RF-Star wireless module and includes an ARM Cortex M4F RF microcontroller supporting the following protocols: Thread,
Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4, IPv6-enabled (6LoWPAN), as well as proprietary protocols including TI 15.4-Stack (2.4 GHz), and simultaneous multi-protocol operation via Dynamic Multiprotocol Manager (DMM).

The main functionally repeats the LAUNCHXL-CC26X2R1 Evaluation board, excluding debugging and monitoring tools. This allows the use of standard software samples and libraries from the specified board.

The form factor of the board is designed both for use as an independent device with battery (CR2032 battery) or external power supply (microUSB or PIN connector), and as a built-in device for collecting and transmitting information from various sensors and inputting external signals.
The microcontroller has a standard I/O ports with 3.3 V logic, pins with increased load capacity, pins with ADC capability and supports a set of standard interfaces (I2C, UART, SPI).
Along the perimeter of the board, there are contact pads with a pitch of 2.54 mm, to which most of the controller pins are brought out, including power, programming and JTAG debugging pins.
The developed board is wired on a 2-sided PCB, [GERBER] (https://github.com/co-Palko/Develop_board_CC2652R_v1/tree/main/gerber/) and BOM files are attached to the production order, and the size of the components is suitable for independent assembly. The schematic diagram of the device is presented at [LINK] (https://github.com/co-Palko/Develop_board_CC2652R_v1/blob/main/images/Devboard_mini_cc2652r-1_2021-02-091.jpg).
  
  
Initially, there are three standard 4-pin 3.5mm connectors, to which the main interface pins of the microcontroller are brought out, as well as the power pins of the connected devices (while there is a choice of its type - a constant 3.3V power supply, or power from an output with increased load capacity for consumption control and management).
If necessary, it is possible to separate half of the board with 3.5mm interface connectors to reduce the external dimensions of the device.
  
  
The configuration of the board implies the ability to install it in a factory-made case like [AK-W-48] (https://myszomk.ru/product/ak-w-48) (SZOMK factory) or [BMW50032-A1] (https: // aliexpress.ru/item/Wall-mounting-junction-box-for-electronic-plastic-enclosure-connector-diy-plastic-box-for-electronics-project-81/32906762106.html) (RTKLM factory) with minimal revision for output connectors.  

Source files for building the firmware are located at the [LINK](https://github.com/diyruz/SensBoard)
