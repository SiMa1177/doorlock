# MuMaLab DoorLock

## Schema
```
                      +----+                                        
                      |    |                          +-----------+
                      |    |                          | RFID      | 
                      |    |                       +--+ Reader    | 
                      |    |                       |  +-----------+ 
  +--------------+    |    |    +---------------+  |                
  |              |    |    |    |               |  |  +-----------+ 
  | RaspberryPi  +----(UART)----+  Arduino      +--+--+ Keypad    | 
  |              |    |    |    |   (frontend)  |  |  +-----------+ 
  +------+-------+    |    |    +---------------+  |                
         |            |    |                       |  +-----------+ 
         |            |    |                       +--+ Display   | 
   +-----+------+     |    |                          +-----------+ 
   | Door lock  |     |    |                                        
   +------------+     |    |                                        
                      +----+                                        
```
This project concept is amazing!