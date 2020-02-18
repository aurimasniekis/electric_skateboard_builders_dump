# VESC Configuration web tool (ALPHA)

### Replies: 11 Views: 2122

## \#1 Posted by: makevoid Posted at: 2016-08-05T16:46:08.749Z Reads: 245

```
Hi, 

I'm working on a bigger tool than the calc one, this time around VESC configurations:

Check this out:

### **http://config.esk8.it**

---

---

Features:

- Sharable link
- simplified configs for BLDC
- Loads and Exports VESC XML config from/to the BLDC tool



Features to add:

- List FOC mode simplified params
- Choose battery S and chemistry (lipo/li-ion) to automatically set battery voltages
- Compare two configurations 
- Explain all the configs in detail
- something cool with Chrome extensions USB support maybe? ( ;] )
- you name it!

if it's easy to do I will be happy to code it


These are [my VESC configs](http://config.esk8.it/#{"pwm_mode":1,"comm_mode":0,"motor_type":0,"sensor_mode":0,"l_current_max":60,"l_current_min":-60,"l_in_current_max":30,"l_in_current_min":-20,"l_abs_current_max":20,"l_min_erpm":-100000,"l_max_erpm":100000,"l_max_erpm_fbrake":300,"l_max_erpm_fbrake_cc":1500,"l_min_vin":8,"l_max_vin":57,"l_battery_cut_start":28,"l_battery_cut_end":26.4,"l_slow_abs_current":1,"l_rpm_lim_neg_torque":1,"l_temp_fet_start":80,"l_temp_fet_end":100,"l_temp_motor_start":80,"l_temp_motor_end":100,"l_min_duty":0,"l_max_duty":0,"sl_min_erpm":150,"sl_min_erpm_cycle_int_limit":1100,"sl_max_fullbreak_current_dir_change":10,"sl_cycle_int_limit":105,"sl_cycle_int_limit_high_fac":0,"sl_cycle_int_rpm_br":80000,"sl_bemf_coupling_k":600,"hall_table_0":-1,"hall_table_1":1,"hall_table_2":3,"hall_table_3":2,"hall_table_4":5,"hall_table_5":6,"hall_table_6":4,"hall_table_7":-1,"hall_sl_erpm":2000,"foc_current_kp":0,"foc_current_ki":50,"foc_f_sw":20000,"foc_dt_us":0,"foc_encoder_inverted":0,"foc_encoder_offset":180,"foc_encoder_ratio":7,"foc_sensor_mode":0,"foc_pll_kp":2000,"foc_pll_ki":20000,"foc_motor_l":7,"foc_motor_r":0,"foc_motor_flux_linkage":0,"foc_observer_gain":9,"foc_duty_dowmramp_kp":10,"foc_duty_dowmramp_ki":200,"foc_openloop_rpm":1200,"foc_sl_openloop_hyst":0,"foc_sl_openloop_time":0,"foc_sl_d_current_duty":0,"foc_sl_d_current_factor":0,"foc_hall_table_0":255,"foc_hall_table_1":255,"foc_hall_table_2":255,"foc_hall_table_3":255,"foc_hall_table_4":255,"foc_hall_table_5":255,"foc_hall_table_6":255,"foc_hall_table_7":255,"foc_sl_erpm":2500,"s_pid_kp":0,"s_pid_ki":0,"s_pid_kd":0,"s_pid_min_rpm":900,"p_pid_kp":0,"p_pid_ki":0,"p_pid_kd":0,"p_pid_ang_div":1,"cc_startup_boost_duty":0,"cc_min_current":1,"cc_gain":0,"cc_ramp_step_max":0,"m_fault_stop_time_ms":3000,"m_duty_ramp_step":0,"m_duty_ramp_step_rpm_lim":0,"m_current_backoff_gain":0,"m_encoder_counts":8192,"m_sensor_port_mode":0}|) for an 8S system, feel free to edit and link yours :)


---

Making this tool took me ~3 days (nights ^^ ). Bare in mind that this hasn't been fully yested! Please recheck the configs thouroughly before loading them into your VESC! Open the XML files sides by sides (your current configuration and the one you exported from the web tool) and make sure the values that you wanted modify changed and NOTHING ELSE did! :)


Do you think that it can be useful? Which features may be quick to add (quick wins)?

note (if you have to edit decimal values you need to type them fast, there's currently a bug, sorry about that :D)
```

---
## \#2 Posted by: ikjahaa Posted at: 2016-08-05T16:55:09.858Z Reads: 207

```
looks neat, but why would we use this ? We still need to use the BLDC tool to upload to our VESC...

Still +1 for your efforts mate !
```

---
## \#3 Posted by: makevoid Posted at: 2016-08-05T16:59:40.763Z Reads: 198

```
Mainly to **share configurations** (I hate opening screenshots :D) and to see if values are out of bounds or maybe to generate a config based on presets (battery / etc) also to highlight wich values need to be changed and maybe for having good defaults... I don't know... :D maybe somebody can come up with good ideas... actually I needed a side project to test if this javascript framework/coding-environment was any good ^^
```

---
## \#4 Posted by: Lizardking0069 Posted at: 2016-08-05T17:06:51.288Z Reads: 183

```
I'm new to VESC and will get them literally today. This looks very easy to use. Thank you for taking time and developing this.
```

---
## \#5 Posted by: JLabs Posted at: 2016-08-05T22:06:13.492Z Reads: 160

```
This would be insanely helpful, it would allow people like @hummie to give specific settings for his hubs so we can get all of the right settings. That is the one thing that is keeping me from getting a VESC
```

---
## \#6 Posted by: Hummie Posted at: 2016-08-06T01:35:57.000Z Reads: 143

```
the settings I do are pretty standard.  I forget what I've changed the brakes to but other than those and the battery and motor amp limits, and the max and min voltage set for 12s, and the two shut down voltages for low batteries.  did the foc test and applied them.  get someone to talk you through getting it up and running and then it's like having learned to read.
```

---
## \#7 Posted by: jrpwit Posted at: 2016-08-07T05:32:22.856Z Reads: 131

```
Keep up the good work!!! We all benefit from it :slight_smile:
```

---
## \#8 Posted by: makevoid Posted at: 2016-08-11T18:13:39.473Z Reads: 126

```
I have wrote a guide on how to use this thing:

## How to use the Web Tool

Once you loaded the "VESC Web Config Tool" (name subject to change) with the desired settings here's how to try them: 

On the 'vesc config web tool' (I probably need a short name for it like BLDC_C) do:

**Export > XML**

then you have your VESC XML file, if you want to import it in BLDC tool you need to hit the **Load XML** button at the bottom (bottom-center-right, so many buttons on that interface lol!) of the BLDC tool window.

Please compare the two files with a diff tool (http://www.mergely.com/editor) to see if other values changed that you didn't want to modify. 

also it's highly recommended if you load the XML exported from the BLDC tool first, so you are sure you're modifying only the right values

we probably need a vesc settings comparison tool lol
 

main VESC settings (my conservative settings):

    ----------------------------------------------------
    Motor max                                 : 60
    ----------------------------------------------------
    Motor min (regen)                         : -60
    ----------------------------------------------------
    Batt max                                  : 25
    ----------------------------------------------------
    Batt min (regen)                          : -15
    ----------------------------------------------------
    Absolute max                              : 130
    ---------------------------------------------------

this snippet is taken from **Export > Text**

---

for devs:

also I included a JSON format that we can use maybe instead of XML and that option of loading/exporting the configs in JSON could be integrated in the BLDC tool

then the web tool could write firmware files as well potentially so that you install it via firmware upgrade but the compilation process probably needs a server... this app generates XMLs on the client (in the browser) and it uses only local data


man I wrote too much... sorry guys! :smiley:
```

---
## \#9 Posted by: Goombaacez84 Posted at: 2016-10-15T21:23:51.933Z Reads: 80

```
Where's the progress of this web tool? I was thinking of the same idea a few days ago and then remembered that I may or may not have read about someone else doing this. I think this tool has some really cool potential!
```

---
## \#10 Posted by: makevoid Posted at: 2016-10-16T00:01:13.855Z Reads: 72

```
hmm, well it works, it's not perfect but it generates good XMLs (especially if you import yours as a base, so it has exactly your settings as base). I use it sometimes to make modifications, save the XML to be able to try them quickly just by loading the XMLs in the vesc tool, I do that when I need to change more than 1-2 parameter.

As Benjamin is doing the new vesc tool that will have a different XML formats and configurable fields I paused the project and will probably restart it later when that will be out (also I have limited time lately ^^). As the project is open source you're free to fork it, improve it or take inspiration (and code) from it and make something else / something similar. :)
```

---
## \#11 Posted by: y.k Posted at: 2018-10-27T07:30:48.777Z Reads: 18

```
Hi.i have a 220kv 2200w alien power motor with a 8s lit ion battery pack and a Vesc. i wan to programmate my vesc. could you help me to fill in the parametrs in bldc tool program?
```

---
