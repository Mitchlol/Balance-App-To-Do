# Balance-App-To-Do
This is my personal list of changes or features for the balance app.

I may never do any of this, it is just a list.

Feel free to create an issue if you want me to add a feature to the list.


## DONE:
- Configureable Dead Zone
- Configureable Min current
- Clear all compiler warnings
- Proper external gyro wiring
- Ui display loop time
- Ui display state
- Ui display motor position
- Ui configure all new settings
- My MPU 9250 Reg 0x75: 01110011 (0x73)
- fix v6 external GYRO
- UI multiple pages
- configurable axies (Removed)
- foot sensors
- Low voltage tiltback
- high voltag tiltback
- can bus
- can stabilization
- can steering
- lock wheel at standstill
- adjustable wheel lock
- Dead delay
- fault delay
- elevated mode
- footpad voltage
- Can steering based on speed
- Can steering current clamp
- Info about pulldown on switches
- Min rpm for half switch state fault
- Soft mode tuning (pitch angle affinity, setpoint affinity, setpoint limit)
- Reset I value on faults issue #117
- fix startup tiltback
- Update defaults to better values
- Configureable overspeed shutoff (Will require a reboot after shutoff!(Nope, not anymore, it latches on angle faults ;-)))
- Configureable tiltback speed trigger
- Configureable tiltback angle
- Configureable tiltback degrees/s
- Configureable startup tilt to center degrees/s
- Configureable unlock Pitch angle
- Configureable unlock Roll angle
- Label every fault
- Timer for each fault
- Clear dead state by triggering another fault
- Setpoint filtering does NOT break tiltback
- D-term PT1 filter
- Change constant tiltback to have configurabe erpm
- Realtime IMU Data on mobile
- Realtime Balance data on mobile
- Multiple GYRO algorithm choices
- Remove smoothing
- Remove Current Boost
- Boost mode
- Torque tilt
- Turn tilt
- Why disable smoothing during centering
- High pass/band filter for D term
- Rename torquetilt Power to Strength
- Rename torquetilt start current toCurrent Threshold?
- Torque Tiltback Current Filter Help Text Improovments
- Reorder Strength Terms to Top of lists
- Rename turntilt Power to Strength
- Rename turntilt Cutzone to Roll Threshold?
- Fix turntilt speed boost % help text
- Make turntilt min erpm configurable
- Fix D term to use change in angle rather than error (which includes tilt steps)
- Switch TorqueTiltback filter to Biquad
- Split TorqueTiltback Relax speed
- Add Biquad filter to D term
- Add console command to graph specific variables
- Add console command to log to console
- Add console command to log to experiments tab
- Add brake current Timeout
- Cleanup initialization loop timing
- Add loop timing correction (Track average error)
- Graph toggleable data

## Done In beta
- Cascading PID
- 400khz i2c speed
- Fix IMU read loop timing
- Add support for imu filters on bmi160
- Set lsm6ds3 & tr-c ODR correctly
- Fix directionality of turntilt
- Clamp PID output to max currents
- I Term Current Limit
- Remove Unused D term filters
- Text display of imu values in desktop tool
- Accel low pass filter, split per axis
- IMU Configuration wizard

## Merge request placed


## TODO For sure
- switch to vescpkg
- Temperature Tiltback
- Improve dual switch startup for spotty switches (potnetially surestart)
- lsm6ds3tr-c filter configuration
- Time scaled PID maths
- Mini QML utilities
- App Configuration wizard
- Stop motor config wizard from setting voltage limits when EUC is selected.
- Maintain buzzer lisp script somewhere visible, perhaps add LEDs as well

## TODO Eventually
- Split faults from run states?
- Graph D term frequecy spectrum
- Cleanup centering logic
- Add minimum tiltback duration?
- realtime setpoint value? (Dupe with graph commands?)

## TODO Theoretical:
- Migrate app to lisp
- Shudder instead of tiltback
- Turntilt vairable based on hillclimb? ~hannes

## MAYDO:
- Exponential P?
- PPM & Balance app

## NODO:
- Steal betaflights gyro code
- Rewrite motor code to execute faster (PIDs can be tweaked)
- Perfect stability
- Polynomial motor value curves
- X-Reduce gyro/acc scale
- Multiple PID sets
- Find ways to reduce CPU load
- Reverse Stop (Figure out motor position conundrum)

## Done EXPIREMENTS:
- try lpf gyro
- try logic scaling PIDs
- Cascade controll with angle constrolling acceleration and acceleration controlling current? (or something like that)


## Videos done:
- intro: terms(fault, tiltback, imu, gyro, accel, pid, dead), things will change, you should experiment, safety (watch next), LOOK at the numbers on the bottom of the balance screen, how to enable the balance app
- How self balancing vehicles work:
- Safety: Faults, dead, tiltback, and delays
- IMU: How to configure, how to wire an external IMU, external requires reboots, dont use conflicting app
- Reccomended settings floatwheel: startup, fault, tiltback
- Reccomended settings euc: startup, fault, tiltback
- Tuning: PIDs
Can bus and steering:
- foot sesnors: adc, wiring, pulldown
- ACC Tuning
- Accelerometer calibration

## Videos todo:
- Safety tips
- IMU new new
