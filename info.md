# keymaster
Home Assistant Zwave keymaster package

**N.B.**  After you add your devices (Zwave lock, door sensor) to your Z-Wave network via the inclusion mode, use the Home Assistant Entity Registry to rename each entity that belongs to the device and append `_LOCKNAME` to it.  For example, if you are calling your lock `FrontDoor`, you will want to append _FrontDoor to each entity of the device.

`sensor.schlage_allegion_be469_touchscreen_deadbolt_alarm_level` 
would become 
`sensor.schlage_allegion_be469_touchscreen_deadbolt_alarm_level_frontdoor`

Do this step for each lock and door sensor.

This will automatically generate the keymaster files just as the `setup.sh` script would have.

**Important**
I make no claims to be good with programming. I made a fork of this project to implement some minor changes for my own needs. Use this fork at your own risk. I will try to keep good documentation of the changes I've made in case you're interested in using this fork.