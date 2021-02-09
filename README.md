# Develop_board_CC2652R_v1
Development and universal sensor board, with zigbee RF-BM-2652B1 module. 

Устройство разработано на основе беспроводного модуля компании RF-Star, и включает в себя радиочастотный микроконтроллер ARM Cortex M4F поддерживающий протоколы: Thread,
Zigbee®, Bluetooth® 5.1 Low Energy, IEEE 802.15.4, IPv6-enabled (6LoWPAN), а также проприетарные протоколы включая TI 15.4-Stack (2,4 ГГц), и одновременную многопротокольную работу через Dynamic Multiprotocol Manager (DMM).  

Основная схемотехника функционально повторяет плату разработчика LAUNCHXL-CC26X2R1 Evaluation board, исключая средства отладки и мониторинга. Это позволяет использовать стандартные примеры программного обеспечения и библиотеки от указанной платы. 

![alt tag](https://github.com/co-Palko/Develop_board_CC2652R_v1/blob/main/images/TOP_assem.JPG)


Форм-фактор платы расчитан как на применение в качестве  самостоятельного устройства с батарейным (батарея CR2032) либо внешним питанием (microUSB либо разъем), так и в качестве встраиваемого устройства для обеспечения сбора и передачи информации от различных датчиков и ввод внешних сигналов.  
Микроконтроллер имеет на борту стандартные порты ввода-вывода с 3.3 вольтовой логикой, выводы с повышенной нагрузочной способностью, выводы с возможностью АЦП и поддерживает набор стандартных интерфейсов (I2C, UART, SPI).  
По периметру платы располагаются контактные площадки с шагом 2,54мм, на которые выведены большинство выводов контроллера, включая питание, выводы программирования и отладки JTAG.  
Разработанная плата разведена на 2-х стороннем текстолите,  для заказа на производстве прилагаются [GERBER](https://github.com/co-Palko/Develop_board_CC2652R_v1/tree/main/gerber/) и BOM файлы, а размер компонентов подходит для самостоятельной сборки.  
Изначально предусмотрены три стандартных 4-х контактных разъема 3.5мм, на которые выведены основные интерфейсные выводы микроконтроллера, а так же выводы питания подключаемых устройств (при этом есть возможность выбора его типа - постоянное питание 3.3В, либо питание от вывода с повышенной нагрузочной способностью для контроля и управления потреблением).  
При необходимости есть возможность отделения половины платы с интерфейсными разъемами 3.5мм для уменьшения внешних габаритов устройства.   

Конфигурация платы подразумевает возможность установки ее в фабрично изготовленный корпус типа [AK-W-48](https://myszomk.ru/product/ak-w-48) (SZOMK factory) либо [BMW50032-A1](https://aliexpress.ru/item/Wall-mounting-junction-box-for-electronic-plastic-enclosure-connector-diy-plastic-box-for-electronics-project-81/32906762106.html) (RTKLM factory). 
