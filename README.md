Home Assistant configuration file modbus.yaml for reading data from Growatt offgrid inverter SPF6000ES plus.
To use this configuration file, you need to add this row to your configuration.yaml:
```
modbus: !include modbus.yaml
```
And you need change the host IP address and slave device address for each entties according to your hardware setup.

For communication with the inverter used WiFi serial server [NA611-SA](https://www.cdebyte.com/products/NA611-SA/2#Pin) from Ebyte. 

![NA611-SA](/NA611-SA.png =250x250)

On Invertor side used RS485 communication port (for expansion) - marked 17:

![bottom view](/spf6000es_bottom.png)

Port pinout:

![pinout](/RS485_expansion_pinout.png)

To connect invertor and wifi server used standard RJ45 patch cable, cutted one side and connected corresponding wires to pins A and B on NA611-SA server.

It is possible to use any suitable RS485 to Ethernet senvers instead NA611-SA. For server setup, please refer to original documentation.
