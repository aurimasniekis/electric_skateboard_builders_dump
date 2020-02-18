# Asking help from the coders

### Replies: 1 Views: 127

## \#1 Posted by: chuttney1 Posted at: 2018-11-24T06:26:36.990Z Reads: 61

```
This section of the code was taken from drv8301.c. I have 0 understanding of what has been typed in the source code. 

I am having trouble understanding what the 2 and 0x0430 stands for. My current understanding is I believe the 2 refers to the address 0x02 in the datasheet and the hexadecimal value of 430 refers to the binary value for 0x02. 

    // Disable OC
    	drv8301_write_reg(2, 0x0430);
    	drv8301_write_reg(2, 0x0430);

I need an explanation on the code below.


     * @param val
     * The value to use. Range [0 31]. A lower value corresponds to a lower current limit. See
     * the drv8301 datasheet for how to convert these values to currents.
     */
    void drv8301_set_oc_adj(int val) {
    	int reg = drv8301_read_reg(2);
    	reg &= 0x003F;
    	reg |= (val & 0x1F) << 6;
    	drv8301_write_reg(2, reg);
    }
```

---
