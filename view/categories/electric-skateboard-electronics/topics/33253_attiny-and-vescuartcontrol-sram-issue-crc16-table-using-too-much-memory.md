# Attiny and VescUartControl SRAM issue. CRC16 table using too much memory

### Replies: 1 Views: 229

## \#1 Posted by: gazwoo123 Posted at: 2017-09-16T08:20:12.619Z Reads: 40

```
Hey,
        So currently I have an Attiny87 + NRF24L01 to send Nunchuk values to VESC. The VescUartControl library uses too much SRAM for the Attiny87. This is due to the crc16() function in crc.cpp which uses a very large hash table. What is the purpose of this table and how can I make this smaller in memory?
```

---
