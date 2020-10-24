Tool for scan PLC devices over modbus protocol.

This project is forked from https://github.com/meeas/plcscan and updated for Python 3. S7 protocol was removed.

## Usage examples:
```
plcscan.py 192.168.0.1
plcscan.py --timeout 2 192.168.0.1:102 10.0.0.0/24
plcscan.py --hosts-list hosts.txt'
```
where file hosts.txt looks like:
```
 192.168.1.15
 192.168.1.107:102
 example.host:502'
```
## Output examples:
### Modbus device
```
127.0.0.1:502 Modbus/TCP
   Unit ID: 0
     Response error: ILLEGAL FUNCTION
     Device info error: ILLEGAL FUNCTION
   Unit ID: 255
     Response error: GATEWAY TARGET DEVICE FAILED TO RESPOND
     Device: Lantronix I WiPo V3.2.25`
```
