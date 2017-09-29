# GMX-CARRIER
The GMX Carrier is a companion board for GMX modules.<br/>
<br/>
<img src="/docs/carrier1.png"/>
<br/>
<br/>
It breakouts the GMX bus enabling quick prototyping of your next IoT module. But it doesn't stop here, the GMX Carries adds an USB/Serial bridge allowing the connection of the GMX serial port to your computer USB port. A LiPO battery section, including battery recharge when you connect the USB connector. Power ON/OFF pushbutton to turn on and off the module ( auto on is available with a jumper ). Last but not least an 10 pin ARM programming header that will enable the programming GMX modules that have a programmanle MCU on board ( GMX-LR1 for example).
<br/>
<br/>
Here the back side of the board, with the label of the GMX bus breakout.<br/>
<br/>
<img src="/docs/carrier_back_2.png"/>
<br/>
<br/>
The carrier board has been designed for ultra low power nodes. When connected to the battery the overall power footpring of the module is around 3uA.<br/>
<br/>
The carrier board has 4 jumpers that allow different behaviours.
<img src="/docs/carrier1_label.png"/>
<br/>
* A => auto power on. When connected the board turns on automatically when power is applied. If removed you need to push the push button to turn on the board.
* B => handles the STM32 bootloader. When connected GMX modules that have an STM32 MCU  (like the GMX-LR1) will enter bootloader mode.
* C => connects the Power On LED. Normally is not connected to save power.
* D => enables the step-up converter for 5V on the GMX bus, normally this voltage is not necessary, to save power it is recommended to keep it removed.
