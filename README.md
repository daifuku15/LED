# Blink LED using device driver on Rasberry Pi  
## Demo Video  
https://youtu.be/ME4jk6MAx8A  
## Dependency  
C  
## Setup  
Hardware: Rasberry Pi 3 Model B V1.2  
Software: Raspbian 3.2.1  
## Usage  
Connect LEDs to pins 22 and 39 on the Rasberry Pi  
Compile myled.c with Makefile  

    sudo insmod myled.ko  
    sudo chmod 666 / dev / myled0  
    echo 0> / dev / myled0  //Turn off LED  
    echo 1> / dev / myled0  //Turn on LED  

## License  
This software is released under the GNU GENERAL PUBLIC LICENSE, see LICENSE.  
## References  
https://github.com/ryuichiueda/robosys2019.git
