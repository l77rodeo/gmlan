# GMLAN Definition
This repositority defineds GMLAN CANBUS messages that are used by General Motors to communication information between control modules in GM vehicles.

All of this information (so far) is from a vehicle with a E38 PCM (Powertrain COntrol Module) and T43 TCM (Transmission Control Module). The information is likely to be relevant to many other GM ECU's as the GM standard GMW8762 applies to many vehicles.

Specifically, I am attempting to understand the message content and structure of high speed (HS) 11 bit canbus data maessages with the following message IDs:

0C7   0F1   199   [0C9](#message-id-0c9)   1EF   191   1E1   1F9   19D   [0F9](#message-id-0cf9)   [1F5](#message-id-1f5)   [1F3](#message-id-1f3)
1ED   189   388   1AF   380   3C9   280   12A   2D1   1C3   1F1   1A1
2C3   4C1   3E9   2F0   3F1   3FB   3C1   3F9   3D1   771   4D1   4C9
4E1   514   138   130   [4E9](#message-id-4e9)   52A   77F   772   4C1   671   120   641
4F1   241   244   644   544

## Message ID 0C9
1. Accelerator actual position
2. Accelerator actual position validity
3. Engine run active
4. Engine speed
5. Engine speed status
6. Platform engines speed command inhibit request
7. Power takeoff powertrain Run aborted
8. Powertrain brake pedal discrete input
9. Powertrain brake pedal discrete input validity
10. Powertrain crank aborted
11. Powertrain crank active
12. Powertrain run aborted
13. Remote vehicle start engine running
14. Cylinder deactivation mode
15. Engine Idle active
16. Driver throttle override detected
17. Cruise control enabled
18. Cruise control active status

## Message ID 0F9
1. Transmission Output shaft angular velocity
2. Transmission Output shaft angular velocity sensor present
3. Transmission Output shaft angular velocity validity
4. Transmission overall estimated torque ratio
5. Transmission overall estimated torque ratio validity"


## Message ID 1F3	
(GW tx)
1. Overdrive disable requested
2. Platform transmission tap up/tap down enable switch state
3. Platform transmission tap up/tap down switch state
4. Platform transmission tap up/tap down switch status rolling count
5. Transmission oil life reset request
6. Transmission platform shift pattern switch 1 active
7. Transmission platform shift pattern switch 2 active
8. Transmission platform shift pattern switch 3 active
9. Transmission platform shift pattern switch 4 active
10. Transmission platform shift pattern switch alive rolling count

## Message ID 1F5
(TCM,ECM tx)
1. Automatic transmission commanded gear
2. Automatic transmission gear shift direction
3. Driver shift control request denied indicator on
4. Driver shift control target gear
5. Engine recommended upshift indicator on
6. Overdrive Disable Granted
7. Top of travel clutch switch active
8. Top of travel clutch switch active validity
9. Transmission creep mode active
10. Transmission estimated gear
11. Transmission estimated gear validity
12. Transmission range inhibit status
13. Transmission shift lever lock requested
14. Transmission shift lever position
15. Transmission shift lever position validity
16. Transmission shift mode status
17. Transmission shift pattern active status
18. Transmission skip shift indicator on
19. Transmission Tap up/Tap down mode status

example message
- 1F5 0F0F000100000300 = Park
- 1F5 0F0F000200000300 = Reverse
- 1F5 0F0F000300000300 = Neutral
- 1F5 0F0F000400000300 = Drive

## Message ID 4E9
(GW tx)
1. Ac compressor type
2. Elapsed time count
3. Elapsed time count reset occurred
4. Antilock braking system present
5. Platform engine speed commend system type
6. Traction control system present
7. Vehicle speed control system type
8. Vehicle stability enhancement system present

example message
- 4E9	01003C11C6
- 4E9	01003C13A2


