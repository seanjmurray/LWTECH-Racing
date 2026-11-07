# Design

### 📌 Design Standards

[CAD naming conventions](Design/CAD%20naming%20conventions%202efff0e90a7b80d299ded3c3ee097e14.md)

- Units (inches)
- Revision control rules
- File storage rules

### 📌 Geometry Reference

- Wheelbase: 62 in
- Track: 48 in
- Ride height: 1.75 in
- Camber targets, etc.

### 📌 Design Deliverables

- Suspension sketch + motion study
- Upright model
- Steering rack layout
- Chassis tube layout

### 📌 throttle requirements

- Mechanical throttle
    - IC3.3.3 pg 82
    - Smooth can bind or stick
    - 50mm away from exhaust out of exhaust stream
    - Can't be kinked by driver when operating, entering or exiting vehicle
    - Must fail closed.
    - 2 return springs each capable of closing throttle
        - Throttle position sensor doesn’t count
        
         
        

### 📌 brake requirements

- 64 to 65
- Brake system encoder T.4.3
    - Basically same requirements as the APPS
    - Only one sensor required
    - Switch ok Can measure pressure or pedal position as well
- Two independent circuits
- Must act on all four wheels
- If A leak occurs system must maintain pressure to two wheels.
- Single control (one pedal)
- Two separate reservoirs or an OEM style resistor
- Single rotor acceptable when using limited slip diff
- No brake by wire
- No unarmored plastic brake lines
- Brakes lines must be protected by scatter shield in case of drive train failure
- Any brake systems must be above the lower surface of the chassis if on a sprung portion of the vehicle
- Brake fasteners are critical fasteners see t.8.2
    - Minimum grade 5 sae, class 8.8, an/Ms or greater
    - Positive locking mechanism see t.8.3
    - Thread retaining compound, washers are not positive retaining mechanism
- pedal box t.3.2
    - Must be steel aluminum or TI
    - Must withstand 2000n of force (450 lbs)
    - inspector can try and test it
- Brake over travel switch BOTS
    - If brake pedal exceed normal range there must be a permanent, not momentary, switch that will be operated
    - Must trigger the shutdown circuit (see IC.9.2.2)
- Brake light t.3.4 pg 65
    - Visible in daylight
    - Red
    - Surface area for 15cm^2
    - Mounted center line at driver shoulder level
    - Rectangular, triangle, or semi circular shape ok
    - If using line of leds must be 150mm long
    - Individual LED must be less than 20mm apart without a diffuser
- Shutdown circuit IC.9.2.2
    - stop engine
    - Disconnect power to
        - Fuel pump
        - Ignition
        - Electronic throttle (ETC only)
- Electronic throttle
    - https://www.fsaeonline.com/cdsweb/gen/DownloadDocument.aspx?DocumentID=278fd4d7-aa27-4e33-bc4a-090148e662a0
        - Page 65 to 66
    - Accelerator pedal (AP) must have positive stop
    - AP must control prower train output
    - Two return springs each strong enough to return accelerator pedal position sensor (APPS) to 0%
    - At least Two electrically separated sensors for APPS reading (two sensors in one OEM unit is acceptable)
    - AAPS requirements
        - See t.4.2.3
    - implausibility T.4.2.4
        - If APPS differ by more than 10% for 100ms power to the electronic throttle must be stopped. Deffined as
    - T.4.2.7 APPS must be inspectable and able to isolated electrically during inspections
    - Annolgoue or digital (can) data signal acceptable
    - Any failure of APPS or wiring must be treated as a implausibility and detectable by engine management

service manuals, parts diagram [https://www.partzilla.com/catalog/honda/motorcycle/2010/cbr600rr-2a](https://www.partzilla.com/catalog/honda/motorcycle/2010/cbr600rr-2a)

[07-12_600RR Service Manual unindexed.pdf](Electrical/07-12_600RR_Service_Manual_unindexed.pdf)

[honda_2013-2015_cbr600rr indexed.pdf](Electrical/honda_2013-2015_cbr600rr_indexed.pdf)

# WIP

[Chain driven diff using off the shelf parts ](Design/Chain%20driven%20diff%20using%20off%20the%20shelf%20parts%202f9ff0e90a7b8090a8ebe6cd419d1435.md)

[cbr600rr-engine-with-oil-sump-1-1.snapshot.1.zip](Design/cbr600rr-engine-with-oil-sump-1-1.snapshot.1.zip)

[Tube Frame 1.SLDPRT](Design/Tube_Frame_1.sldprt)

MULE FRAME:

[M01-04 v1.f3z](Design/M01-04_v1.f3z)