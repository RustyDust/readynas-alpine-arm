# Serial USB connections

If you want to see what your ARM based ReadyNAS is doing during boot the
easiest way is to use the serial console on the back of the system. To 
connect it to your PC you'll need an USB-to-RS232 cable. I'm using a
[CP2102 based adapter](https://www.amazon.de/wwwwhocarede21/dp/B0773G2K92)
that works well on Linux, Mac OS and Windows 10/11.

I prefer a version that allows me to connect only the cables I need and also 
where I can see the description of the pins, that's why I use 
[this one](https://www.amazon.de/wwwwhocarede21/dp/B0773G2K92).

## PIN layout on the ReadyNAS
The left side is the port on the ReadyNAS, pin numbers go from left to right
when looking at the port.
Right side is the connector the pin needs to get connected to. If nothing is
noted there the pin doesn't need to be connected

### RN102
**Speed:** 115200 bps
```
1 2 3 4
| | | +->
| | +---> TxD
| +-----> Rxd
+------->
```

### RN204
```
TxD <- 1 2 -> RxD
    <- 3 4 ->
```
