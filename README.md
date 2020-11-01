# GMLAN Definition
This repositority defineds GMLAN CANBUS messages that are used by General Motors to communication information between control modules in GM vehicles.

All of this information (so far) is from a vehicle with a E38 PCM (Powertrain COntrol Module) and T43 TCM (Transmission Control Module). The information is likely to be relevant to many other GM ECU's as the GM standard GMW8762 applies to many vehicles.

Specifically, I am attempting to understand the message content and structure of high speed (HS) 11 bit canbus data maessages with the following message IDs:

- 0C7
- 0F1
- 199
- 0C9
- 1EF
- 191
- 1E1
- 1F9
- 19D
- 0F9
- 1F5
- 1F3
- 1ED
- 189
- 388
- 1AF
- 380
- 3C9
- 280
- 12A
- 2D1
- 1C3
- 1F1
- 1A1
- 2C3
- 4C1
- 3E9
- 2F0
- 3F1
- 3FB
- 3C1
- 3F9
- 3D1
- 771
- 4D1
- 4C9
- 4E1
- 514
- 138
- 130
- 4E9
- 52A
- 77F
- 772
- 4C1
- 671
- 120
- 641
- 4F1
- 241
- 244
- 644
- 544


## Message ID 0C9
Accelerator acutal position
Accelerator actual position validity
Engine run active
Engine speed
Engine speed status
Platform engines speed command inhibit request
Power takeoff powertrain Run aborted
Powertrain brake pedal descrete input
Powertrain brake pedal descrete input validity
Powertrain crank aborted
Powertrain crank active
Powertrain run aborted
Remote vehicle start engine running
Cylinder deactivation mode
Engine Idle active
Driver throttle overide detected
Cruise control enabled
Cruise control active status

## Message ID 0F9
Transmission Output shaft angular velocity
Transmission Output shaft angular velocity sensor present
Transmission Output shaft angular velocity validity
Transmission overall estimated torque ratio
Transmission overall estimated torque ratio validity"


## Message ID 1F3	
(GW tx)
Overdrive disable requested
Platform transmission tap up/tap down enable switch state
Platform transmission tap up/tap down switch state
Platform transmission tap up/tap down switch status rolling count
Transmission oil life reset request
Transmission platform shift pattern switch 1 active
Transmission platform shift pattern switch 2 active
Transmission platform shift pattern switch 3 active
Transmission platform shift pattern switch 4 active
Transmission platform shift pattern switch alive rolling count


