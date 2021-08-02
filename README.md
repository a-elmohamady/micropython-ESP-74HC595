# micropython-ESP-74HC595
MicroPython on ESP module with ESP8266 for 74HC595 shift registers 





```python
from shiftregister import SR

while True:
    for i in range(0 , 16):
        sh.setOutput(i,True)
        sh.latch()
        print(i)
        time.sleep(1)
        
    sh.setOutputs([0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0])
    sh.latch()



```
