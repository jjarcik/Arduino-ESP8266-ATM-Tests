# Arduino Test ESP8266 by ATM

## Wiring diagram
<img src='https://raw.githubusercontent.com/jjarcik/Arduino-ESP8266/master/WiringDiagramEsp8266.png' width=450/>

### Best wiring
try this: http://www.instructables.com/id/Cheap-Arduino-WiFi-Shield-With-ESP8266/?ALLSTEPS

## Test
- Run Arduino IDE
- Open tools / Serial monitor
- Set your Module Baud rate (115200) and Both NL and CR 

```
use "AT" for check Communication
Response "OK"

use "AT+RST" for Software Reset Module
Response "OK"

use "AT+GMR" for check Firmware Version
Response "Firmware Version xxxxxxx"
Response "OK"

use "AT+CWMODE=1" for Set Mode 1 ( Station )
Response "OK"

use "AT+CWLAP" for check WiFi Network Available 
Response "Network Detail"
Response "OK"
```

## Source

http://microcontrollerkits.blogspot.cz/2015/02/wifi-module-esp8266-at-command-test.html

http://allaboutee.com/2014/12/27/esp8266-arduino-code-and-circuit/
