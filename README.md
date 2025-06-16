Home Assistant configuration file modbus.yaml, I'm using for data reading from Growatt offgrid inverter SPF6000ESplus.
For communication with the inverter i use WiFi serial server NA611-SA from Ebyte.

![NA611-SA](/NA611-SA.png)

To use this configuration file, you need to add this row to your configuration.yaml:
```
modbus: !include modbus.yaml
```
And you need change the host IP address and slave device address for each entties according to your hardware setup.
