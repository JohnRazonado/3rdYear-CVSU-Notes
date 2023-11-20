## C++
- Developed by **Bjarne Stroustrup** at Bell Labs in **1979**
- A High Level Programming Language
- Attempt to add OO (object-oriented) features
	- Since the whole language is really derived from the C language which focus the structure functional programming.
### Uses of C++
C++ has a lot of uses due to being a general programming language focusing on somewhat bare metal talk to the hardware components.
- System Software
- Game Development
- Embedded Systems
- Scientific Computing
- High Performance Applications

### Variables in C++
- Containers for storing data values.
	- `int x`
	- `float speed`
	- `double velocity`

### Data Types in C++
These are the static data types in C++ (since you can create a new one and there's a new smart data types).
- Integer
- Boolean
- Character
- Float
- String
- Byte
- Double
- Long


## Rules in Naming Variable
- Name variables based on terms of subject area
- Create variable names by deleting spaces that separate words
	- `addProperty`
	- `remove_property`
	- `update-variable`
- Do not begin variable names w/ underscore
	- `_update` as a variable name is a "no no"
- Do not use variable names that consist of single character
	- variable names need to be concise but still holds meaning
	- this can be exempted to variables used in looping 
- Name variables that describe binary states (true or false)
	- `isOpen`
	- `doKill`

## Functions in Arduino C++
### Input and Output
#### pinMode()
- configures the specified pin to behave either as an input or an output.
Syntax:
`pinMode(pin,mode)`
Ex:
```c++
void setup() {
	pinMode(inPin, INPUT);
}
void loop () {
	digitalWrite(13,HIGH);
	delay(1000);
	 digitalWrite(13,LOW);
	delay(1000);
}
```

#### digitalRead()
- reads the value from a specified digital pin, either `HIGH` or `LOW`.
Syntax:
`digitalRead(pin)`
Ex:
```c++
int inPin = 7;
void setup() {
	pinMode(inPin, INPUT);
}
```

#### digitalWrite()
- write a `HIGH` or `LOW` value of digital pin.
Syntax:
`digitalWrite(pin, value)`
Ex:
```c++
void setup() {
	pinMode(13, OUTPUT);
}

void loop() {
	digitalWrite(13, HIGH);
	delay(100);
	 digitalWrite(13, LOW);
	delay(100);
}
```

#### analogRead()
- reads the value from a specified analog pin.
Syntax:
`analogRead(pin)`
Ex:
```c++
int analogPin = A3;
Int val = 0;
void setup() {
	Serial.begin(9600);
}

void loop() {
	val = analogRead(analogPin);
	Serial.println(val);
}
```

#### analogWrite()
- writes an analog value to a pin.
Syntax:
`analogRead(pin)`
Ex:
```C++
int analogPin = A3;
Int val = 0;
void setup() {
	Serial.begin(9600);
}

void loop() {
	val = analogRead(analogPin);
	Serial.println(val);
}
```

### Control Structure
#### If Statement
- checks the condition and executes the following statements or set of statements if the condition is ‘true’.

Syntax:
```c++
if (condition) {
	//statement(s);
}
```
Ex:
```C++
if (x>120) digitalWrite(LEDpin, HIGH);

if (x>120)
digitalWrite(LEDpin, HIGH);

if (x>120) { digitalWrite(LEDpin, HIGH) };

if (x>120) {
digitalWrite(LEDpin, HIGH);
}
```

#### Switch Case
- specify different code that should be executed in various conditions.

Syntax:
```C++
switch (var) {
   case label1:
   //statement(s);
   break;
   case label2:
   //statement(s);
   break;
   default:
   //statement(s);
   break;
}
```

Ex:
```C++
switch (var) {
	case 1:
        //do something when var equals 1
        break;
	case 2:
        //do something when var equals 2
        break;
}
```

#### For Loop
- used to repeat block of statement enclosed in curly braces.
Syntax:
```C++
for (initialization; condition; increment) {
	//statement(s);
}
```
Ex:
```C++
int PWMPin = 10;

void setup(){
	//no setup needed
}
void loop() {
	for (int I =0 ; I <=255; i++) {
		analogWrite(PWMpin, I );
		delay(10);
	}
}
```
