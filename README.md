![Visitor](https://visitor-badge.laobi.icu/badge?page_id=a-elmohamady.micropython-ESP-74HC595)
<img src="https://img.shields.io/badge/made%20with-python-blue.svg?style=flat-square" alt="made with python">

<a href=https://www.linkedin.com/in/elmohamady>![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)</a>
<a href=https://www.facebook.com/elmohamady>![Facebook](https://img.shields.io/badge/facebook-0077B5?style=for-the-badge&logo=facebook&logoColor=white)</a>

# micropython-ESP-74HC595
MicroPython on ESP module with ESP8266 for 74HC595 shift registers 


### Example
| NodeMCU  |   74HC595     | 
|----------|:-------------:|
| D1       |      14       |
| D2       |      12       |
| D5       |      11       |


```python
from shiftregister import SR

sh = SR(data_pin= 5, latch_pin=4, clock_pin = 14 ,units =2 )

while True:
    for i in range(0 , 16):
        sh.setOutput(i,True)
        sh.latch()
        print(i)
        time.sleep(1)
        
    sh.setOutputs([0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0])
    sh.latch()



```
 
 



 https://youtu.be/G6ShLs1QGXg 
 

https://youtu.be/gGsjGB4JzLE
                            

                       
