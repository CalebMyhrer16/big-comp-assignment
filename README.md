# first need to import board specific tools
#every project for this board will need this statment
from adafruit_circuitplayground import cp
import time
#whn the program finishes hte board enters a waiting state

while True:
    cp.pixels.fill((0,10,0))
    time.sleep(.367)
    cp.pixels.fill((0,0,0))
    time.sleep(.367)
    
# first need to import board specific tools
#every project for this board will need this statment
from adafruit_circuitplayground import cp
import time
while True:
    if cp.switch:
        cp.pixels[1] = (0,10,0)
        cp.pixels[2] = (0,10,0)
        cp.pixels[3] = (0,10,0)
        cp.pixels[6] = (0,0,0)
        cp.pixels[7] = (0,0,0)
        cp.pixels[8] = (0,0,0)

    else:
        cp.pixels[6] = (0,10,0)
        cp.pixels[7] = (0,10,0)
        cp.pixels[8] = (0,10,0)
        cp.pixels[1] = (0,0,0)
        cp.pixels[2] = (0,0,0)
        cp.pixels[3] = (0,0,0)
# first need to import board specific tools
#every project for this board will need this statment
from adafruit_circuitplayground import cp
import time
while True:
    x, y, z = cp.acceleration

    if x > 5:
        cp.pixels[1] = (0,10,0)
        cp.pixels[2] = (0,10,0)
        cp.pixels[3] = (0,10,0)
        cp.pixels[6] = (0,0,0)
        cp.pixels[7] = (0,0,0)
        cp.pixels[8] = (0,0,0)

    elif x < -5:
        cp.pixels[6] = (0,10,0)
        cp.pixels[7] = (0,10,0)
        cp.pixels[8] = (0,10,0)
        cp.pixels[1] = (0,0,0)
        cp.pixels[2] = (0,0,0)
        cp.pixels[3] = (0,0,0)
    else:
        cp.pixels.fill((0,0,0))
from adafruit_circuitplayground import cp
import time
while True:
    if cp.button_a:
        cp.pixels[0] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[0] = (0,0,0)
        cp.pixels[1] = (0,0,25)
        time.sleep(.10)
        cp.pixels[1] = (0,0,0)
        cp.pixels[2] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[2] = (0, 0, 0)
        cp.pixels[3] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[3] = (0, 0, 0)
        cp.pixels[4] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[4] = (0, 0, 0)
        cp.pixels[5] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[5] = (0, 0, 0)
        cp.pixels[6] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[6] = (0, 0, 0)
        cp.pixels[7] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[7] = (0, 0, 0)
        cp.pixels[8] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[8] = (0, 0, 0)
        cp.pixels[9] = (0, 0, 25)
        time.sleep(.10)
        cp.pixels[9] = (0, 0, 0)
    else:
		     cp.pixels.fill((0,0,0)) # Off
# first need to import board specific tools
#every project for this board will need this statment
from adafruit_circuitplayground import cp
import time
while True:
    temp_c = cp.temperature
    temp_f = (temp_c * 9 / 5) + 32
    if temp_f < 78:  # Example threshold for cold
        cp.pixels[0] = (0, 0, 1)
    elif temp_f > 78:
        cp.pixels[0] = (0,0,1)  # Example threshold for hot
        cp.pixels[1] = (0,0,1)
    elif temp_f > 79:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
    elif temp_f > 80:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
    elif temp_f > 81:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
    elif temp_f > 82:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
        cp.pixels[5] = (1,1,0)
    elif temp_f > 83:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
        cp.pixels[5] = (1,1,0)
        cp.pixels[6] = (1,1,0)
    elif temp_f > 84:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
        cp.pixels[5] = (1,1,0)
        cp.pixels[6] = (1,1,0)
        cp.pixels[7] = (1,0,0)
    elif temp_f > 85:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
        cp.pixels[5] = (1,1,0)
        cp.pixels[6] = (1,1,0)
        cp.pixels[7] = (1,0,0)
        cp.pixels[8] = (1,0,0)
    elif temp_f > 84:
        cp.pixels[2] = (0,0,1)
        cp.pixels[1] = (0,0,1)
        cp.pixels[0] = (0,0,1)
        cp.pixels[3] = (1,1,0)
        cp.pixels[4] = (1,1,0)
        cp.pixels[5] = (1,1,0)
        cp.pixels[6] = (1,1,0)
        cp.pixels[7] = (1,0,0)
        cp.pixels[8] = (1,0,0)
        cp.pixels[9] = (1,0,0)
    else:
        cp.pixels.fill((0, 0, 0))  # Green for moderate
    time.sleep(0.5)
    cp.pixels[0] = (0,0,15)
    cp.pixels[1] = (0,0,15)
    cp.pixels[2] = (0,0,15)
    cp.pixels[3] = (0,0,15)
    cp.pixels[4] = (0,0,15)
    cp.pixels[5] = (0,0,0)
    cp.pixels[6] = (0,0,0)
    cp.pixels[7] = (0,0,0)
    cp.pixels[8] = (0,0,0)
    cp.pixels[8] = (0,0,0)
    
