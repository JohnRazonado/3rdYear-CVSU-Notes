- An open-source electronic prototyping platform enabling users to create interactive electronic objects.
## History
- **2005** - **Massimo Banzi** needed a low-cost microcontroller platform
	- A community of engineers, hackers, and innovative people all came together to build the first Arduino board called <mark style="background: #ADCCFFA6;">Arduino Serial</mark>

### Timeline
- **2006** - First Arduino board was **Arduino Serial**, didn't have a USB port
- **2007** - Introduced **Arduino Diecimila**, predecessor to UNO having automatic software resets when uploading a sketch to no longer needed to press a reset button.
	- **Lilypad Snap Simple** is so easy to use, doens't need any soldering required. Uses the Atmega168 chip. But it is updated to use Atmega328 in 2009
- **2008** - **Arduino Nano**, **Arduino Mini**, **Arduino Mini Pro**, and **Arduino Duemilanove** was released.
- **2009** - **Arduino Mega** was released, having a bigger size and more pinouts.
- **2010** - **Arduino Uno** and **Fio** was released.
- **2011** - **Arduino Ethernet** was released with the capability of connecting to Internet.
- **2012** - **Arduino Leonardo** and **Arduino Micro** was released
## Parts of Arduino
![[Pasted image 20231025232217.png]]
#### Reset button
- Restart the code currently uploaded in your Arduino when pressed.
#### USB Port
>Note: the port type will be different to the model of Arduino. In Arduino UNO, USB Type-B is used (Similar to most printer cable connectors).
- Serves as connection to computer allowing to program a board.
- also, provide power to Arduino too (Only 5v [mostly]).

### Voltage Regulator
- Converts power power plugged into the power port (barrel plug) into 5 volts and 1A (one amp) standard used by Arduino.

#### Power Port
> This is the barrel plug (5mm) 

- Allows power either straight from wall (using a power supply) or from a battery (9v battery mostly).

#### Built-in LEDs
- Indicate that there's power and if Arduino is sending/receiving (TX/RX) data.
- The other pin can be programmed called `LED_BUILTIN` variable on the Arduino Library (which is connected to pin 13).

#### Digital I/O pins
- Used to either sense outside world (input)
- or control lights, sound or motors (output)

#### TX/RX pins
- Special pins which are <mark style="background: #ADCCFFA6;">pin 1 and pin 0</mark>
>Need more info

#### ATmega328p black chips
- Brain of the Arduino
- Interprets both inputs/outputs and programming code uploaded onto Arduino

#### Power and Ground pins
- All pins related to power are here
- Use to run power from Arduino to your Breadboard circuit
- `Vin` pin means **Voltage input** which only accepts 5v only.
- on Arduino Uno, it has a 5v and 3v pin to use as power to external objects.
- `GND` pins are ground. Just return and closed the loop for a circuit.

#### Analog pins
- Pins that take sensor reading in range of values
- Arduino uno uses a 10-bit variable resolution having a value up to 1024 (0-1023).

## Application for Arduino
1. Home Automation
2. Public Utility Automation
3. IoT