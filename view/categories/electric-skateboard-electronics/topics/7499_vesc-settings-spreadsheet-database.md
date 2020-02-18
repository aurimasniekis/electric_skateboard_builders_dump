# VESC Settings Spreadsheet/Database?

### Replies: 4 Views: 1149

## \#1 Posted by: sprocket12 Posted at: 2016-08-11T16:29:54.228Z Reads: 245

```
Is there one?  Yes, I know, many settings are personal 'preference' and based on variable like battery sizing, motor, remote etc.  But it sure would help everyone if we started collecting this information into something more than interspersed throughout the forum.  

Again, if there is one, please forgive me, I just haven't found any references.

This started because after my first build, and all the time spent researching VESC settings, @Glenn had his Enertion Raptor (single motor) fault.  While working through replacing it, our order for 2 new VESC's came in.  We've hooked up the new VESC (they were bought for new, non-Raptor builds) and found the settings not working with his Raptor.  So the research began... And interestingly, there aren't even 'default' settings posted anywhere that I can find.

So, how about starting with setting up a spreadsheet/database of VESC settings for motor 'x' with 'y' battery, and 'z' remote?  Maybe just defaults to start with tuned options that users like?

Minimum info would include:

* VESC (version/firmware rev)
* Motor (make/model and kv)
* Battery setup (ie 10s3p, 18650's)
* Remote (manufacturer, model, and version)

And then add your VESC settings (maybe the XML file?).

I don't know.  Maybe I'm way off here?  I don't mind cutting my teeth on reading the forum and learning but I've also been turned off by different boards that start promoting elitism...

If interested, start posting *WORKING* settings as described above and I'll collect.
```

---
## \#2 Posted by: makevoid Posted at: 2016-08-11T18:12:41.362Z Reads: 230

```
I did this http://config.esk8.it - that you can use to link to XML configurations, modify them and get a sharable link - if you go to the **Export** tab you can export the **XML** file you can import via the BLDC tool.

This is my config (probably BLDC motor detection values are different but pretty close)

Click on [this link](http://config.esk8.it/#{"pwm_mode":1,"comm_mode":0,"motor_type":0,"sensor_mode":0,"l_current_max":60,"l_current_min":-60,"l_in_current_max":25,"l_in_current_min":-15,"l_abs_current_max":130,"l_min_erpm":-100000,"l_max_erpm":100000,"l_max_erpm_fbrake":300,"l_max_erpm_fbrake_cc":1500,"l_min_vin":8,"l_max_vin":57,"l_battery_cut_start":35,"l_battery_cut_end":33,"l_slow_abs_current":1,"l_rpm_lim_neg_torque":1,"l_temp_fet_start":80,"l_temp_fet_end":100,"l_temp_motor_start":80,"l_temp_motor_end":100,"l_min_duty":0.005,"l_max_duty":0.95,"sl_min_erpm":150,"sl_min_erpm_cycle_int_limit":1100,"sl_max_fullbreak_current_dir_change":10,"sl_cycle_int_limit":105,"sl_cycle_int_limit_high_fac":0.8,"sl_cycle_int_rpm_br":80000,"sl_bemf_coupling_k":600,"hall_table_0":-1,"hall_table_1":1,"hall_table_2":3,"hall_table_3":2,"hall_table_4":5,"hall_table_5":6,"hall_table_6":4,"hall_table_7":-1,"hall_sl_erpm":2000,"foc_current_kp":0.03,"foc_current_ki":50,"foc_f_sw":20000,"foc_dt_us":0.08,"foc_encoder_inverted":0,"foc_encoder_offset":180,"foc_encoder_ratio":7,"foc_sensor_mode":0,"foc_pll_kp":2000,"foc_pll_ki":20000,"foc_motor_l":0.000007,"foc_motor_r":0.015,"foc_motor_flux_linkage":0.00245,"foc_observer_gain":90000000,"foc_duty_dowmramp_kp":10,"foc_duty_dowmramp_ki":200,"foc_openloop_rpm":1200,"foc_sl_openloop_hyst":0.5,"foc_sl_openloop_time":0.5,"foc_sl_d_current_duty":0,"foc_sl_d_current_factor":0,"foc_hall_table_0":255,"foc_hall_table_1":255,"foc_hall_table_2":255,"foc_hall_table_3":255,"foc_hall_table_4":255,"foc_hall_table_5":255,"foc_hall_table_6":255,"foc_hall_table_7":255,"foc_sl_erpm":2500,"s_pid_kp":0.0001,"s_pid_ki":0.015,"s_pid_kd":0,"s_pid_min_rpm":900,"p_pid_kp":0.03,"p_pid_ki":0,"p_pid_kd":0.0004,"p_pid_ang_div":1,"cc_startup_boost_duty":0.01,"cc_min_current":1,"cc_gain":0.0046,"cc_ramp_step_max":0.04,"m_fault_stop_time_ms":3000,"m_duty_ramp_step":0.02,"m_duty_ramp_step_rpm_lim":0.0005,"m_current_backoff_gain":0.5,"m_encoder_counts":8192,"m_sensor_port_mode":0}|)


These are my settings for a very conservative setup:

---

single motor RSPEC 6372
8S (x2 4S lipos in series) ~8A
ratio: 15/36T
97mm wheels
max speed 20mph (>200lbs load)
theoretical max 26.62mph 

vesc current limiting settings:

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

---

on a previous build (6S 10A lipos with a 6374 sensored esk8.de motor) I had these

    ----------------------------------------------------
    Motor max                                 : 85
    ----------------------------------------------------
    Motor min (regen)                         : -70
    ----------------------------------------------------
    Batt max                                  : 40
    ----------------------------------------------------
    Batt min (regen)                          : -30
    ----------------------------------------------------
    Absolute max                              : 130
    ---------------------------------------------------


then see the steps of how to use this thing they're in [this post](http://www.electric-skateboard.builders/t/vesc-configuration-web-tool-alpha/7171/8?u=makevoid)

---

@sprocket12  I don't think we should couple the remote settings because when trimmed remotes have completely different settings and on the remotes that use screws is practically impossible to determine the trim (I think it always should double checked because it must be set to the most accurate values as possible, and we have to remember that we're building a "vehicle" with RC grade stuff already...)
```

---
## \#3 Posted by: sprocket12 Posted at: 2016-08-11T19:08:57.929Z Reads: 201

```
I've read your previous post.  I'm suggesting the next steps. the database part that you are referring to. 

Let's do it!
```

---
## \#4 Posted by: lox897 Posted at: 2016-08-11T20:46:45.431Z Reads: 196

```
@evoheyax and @link5505 have made some spreadsheets.
```

---
