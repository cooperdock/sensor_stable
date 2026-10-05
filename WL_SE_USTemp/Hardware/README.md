# Sensor assembly procedures
This document details the procedures used to build a standard edition water level sensor which also reads the temperature on the Maxbotix internal thermistor.


# Stage 1 - prepare the PCB
<p align="center">
<img src="../../img/HTCC-AB02/PCB_TempConn.jpg" width="50%">
</p>

Create 2 8-pin and 1 2-pin female headers for connecting the microcontroller to the PCB
<p align="center">
<img src="../../img/HTCC-AB02/pcb_insert_header_TempConn.jpg" width="50%">
</p>

Insert the headers into the corresponding hole and flip over the board for soldering.
<p align="center">
<img src="../../img/HTCC-AB02/pcb_insert_header.jpeg" width="50%">
</p>

Solder each pin to the board.
<p align="center">
<img src="../../img/HTCC-AB02/pcb_header_finished_TempConn.jpg" width="50%">
</p>

Insert a 2-pin JST connector in the BAT IN location and a switch into the switch position.
<p align="center">
<img src="../../img/HTCC-AB02/pcb_bat_switch_temp.jpg" width="50%">
</p>

Flip over the board and solder (you may need to tape these components to the board).
<p align="center">
<img src="../../img/HTCC-AB02/pcb_bat_switch_temp2.jpg" width="50%">
</p>

Locate 4 2-pin and 1 3-pin terminals.
<p align="center">
<img src="../../img/HTCC-AB02/pcb_terminals_thermistors.jpg" width="50%">
</p>

Insert each terminal into the remaining locations, with the openings facing the text on the PCB, flip over and solder.

<p align="center">
<img src="../../img/HTCC-AB02/pcb_terminals2_thermistors.jpg" width="50%">
</p>


# Stage 2 - prepare the MCU

Create 2 8-pin and 1 2-pin male headers for soldering onto the MCU
<p align="center">
<img src="../../img/HTCC-AB02/MCU_headers_unconnected_thermistors.jpeg" width="50%">
</p>

Insert the headers into the bottom 8 holes of the MCU on each side (Vin through GPIO7 and VS through GPIO10) as well as ADC2 and ADC3. Then insert the pins into a breadboard for ease of soldering. Ensure the pins are flush with the MCU and solder.

<p>
<img src="../../img/HTCC-AB02/MCU_breadboard.jpeg" width="45%">
<img src="../../img/HTCC-AB02/MCU_breadboard_side_thermistors.jpeg" width="45%">
</p>

Insert the MCU into the PCB board, ensuring the correct pins are connected.

<p>
<img src="../../img/HTCC-AB02/MCU_PCB.jpeg" width="45%">
<img src="../../img/HTCC-AB02/MCU_PCB_side.jpeg" width="45%">
</p>

# Stage 3 - battery assembly

With the PCB switch turned off, remove the MCU and attach a 400 mAh battery to the BAT IN port.

<p align="center">
<img src="../../img/HTCC-AB02/pcb_w_battery.jpeg" width="50%">
</p>

Insert a 2-pin JST connector into the MCU and add a 2 character board label for MCU identification.

<p align="center">
<img src="../../img/HTCC-AB02/MCU_cable.jpeg" width="50%">
</p>

Insert the other end of the JST connector into the BAT OUT port. Ensure the red wire goes into VB and the black wire goes into G.

<p align="center">
<img src="../../img/HTCC-AB02/MCU_power_pcb.jpeg" width="50%">
</p>

Reinsert the MCU into the PCB, ensure you do not damage the battery. There should be plenty of space between the MCU and the battery if inserted correctly.

<p align="center">
<img src="../../img/HTCC-AB02/Battery_inplace.jpeg" width="50%">
</p>

To test power, move the switch to the ON position. If no sketch has been uploaded to the board, it should flash RGB Testing on the LCD screen, along with different lights, then show the text below. 

<p align="center">
<img src="../../img/HTCC-AB02/Testing_power.jpeg" width="50%">
</p>

Turn off power by moving the switch back to the OFF position.

# Stage 4 - Housing preparation

<p align="center">
<img src="../../img/ML22F/enclosure.jpeg" width="100%">
</p>

Secure the lid of the housing in a vice and, using a step-drill bit of at least 1-1/4", drill a hole of approximately 1-1/4". 
 
<p align="center">
<img src="../../img/ML22F/enclosure_w_bit.jpeg" width="50%">
</p>

Periodically check the size by threading a sensor into the hole. Once it is large enough to thread, remove it from the vice and clean up the cut with a razor.

<p>
<img src="../../img/ML22F/hole_in_top.jpeg" width="45%">
<img src="../../img/ML22F/sensor_in_top.jpeg" width="45%">
</p>

Secure the main housing in the vice with the opening facing away from you and drill a 1/4" hole in the right side of the housing, ~1" from the edge.

<p align="center">
<img src="../../img/ML22F/antenna_hole.jpeg" width="50%">
</p>

Flip the housing around and drill a 1/2" hole in the middle of the other side.

<p align="center">
<img src="../../img/ML22F/gland_hole.jpeg" width="50%">
</p>

Insert a 1/4" NPT gland into the 1/2" hole. It should be tight enough that you can get it in and secure it without the end nut.

<p align="center">
<img src="../../img/ML22F/gland_in_enclosure.jpeg" width="50%">
</p>

Insert the antenna cable into the 1/4" hole and secure with included nuts.

<p align="center">
<img src="../../img/ML22F/antenna_connector_in_enclosure.jpeg" width="50%">
</p>

# Stage 5 - Ultrasonic Sensor Assembly

Solder wires into the Ultrasonic sensor pins GND, V+, 5, 4, and 1.
<p align="center">
<img src="../../img/US-Sensor/soldering_sensor.jpeg" width="50%">
</p>

Gently twist wires, ensuring you do not put pressure on the pins.

<p align="center">
<img src="../../img/US-Sensor/sensor_soldered_therm.jpeg" width="50%">
</p>

Stack 2 gaskets that come with mounting hardware onto the sensor threads.

<p align="center">
<img src="../../img/US-Sensor/gaskets_therm.jpeg" width="50%">
</p>

Insert sensor into housing top and secure with mounting nut.

<p align="center">
<img src="../../img/ML22F/housing_on_sensor_therm.jpeg" width="50%">
</p>

Connect the wire leads to the PCB terminal. V+ - VE, GND - G, 5 - RX, 4 - G5, 1 - T Sensor INT/MB.

<p align="center">
<img src="../../img/HTCC-AB02/sensor_connected_therm.jpeg" width="50%">
</p>

# Interlude - set up software

If you have not done so already, this is a good time to set up the TTN connection and flash the software to the MCU. Follow the instructions [here](../Firmware/README.md).

# Stage 6 - Mount all components

Attach the antenna cable to the MCU.

<p align="center">
<img src="../../img/HTCC-AB02/attach_antenna_cable.jpeg" width="50%">
</p>

Insert the MCU by sliding the side with the sensor terminals under the antenna connector and pushing the opening past the gland.

<p align="center">
<img src="../../img/HTCC-AB02/insert_MCU.jpeg" width="50%">
</p>

Secure the MCU to the housing with two mounting screws.

<p>
<img src="../../img/HTCC-AB02/secure_MCU.jpeg" width="45%">
<img src="../../img/HTCC-AB02/MCU_secured.jpeg" width="45%">
</p>

Attach a 915 MHz LoRa antenna to the antenna connector. 

<p align="center">
<img src="../../img/HTCC-AB02/attach_antenna.jpeg" width="50%">
</p>

Ensure the antenna is connected correctly by checking the TTN console. If it is connected correctly your RSSI should increase substantially.

<p align="center">
<img src="../../img/firmware/RSSI.png" width="100%">
</p>

# Stage 7 - prepare and mount solar panel

Solder wire leads onto the back of the solar panel

<p align="center">
<img src="../../img/solar-panel/solar_solder.jpeg" width="50%">
</p>

Using a multimeter, test the voltage coming through the wire leads. With lab lighting and the panel pointing generally at the lights, you should read at least 1 v.

<p align="center">
<img src="../../img/solar-panel/solar_panel_test.jpeg" width="50%">
</p>

Add a generous amount of RTV to the connection to prevent water damage. Seal all electrical connections.

<p align="center">
<img src="../../img/solar-panel/solar_rtv.jpeg" width="50%">
</p>

Apply epoxy to the angled part of the solar panel stand and press firmly onto the solar panel as shown below. Let set overnight.

<p>
<img src="../../img/solar-panel/stand_epoxy.jpeg" width="45%">
<img src="../../img/solar-panel/solar_stand.jpeg" width="45%">
</p>

Once epoxy and RTV are set, thread the wire leads through the gland and connect the V+ wire to the Vs terminal and the V- wire to the G terminal.

<p>
<img src="../../img/HTCC-AB02/solar_connect_leads.jpeg" width="45%">
<img src="../../img/HTCC-AB02/solar_connected.jpeg" width="45%">
</p>

Test the voltage coming from the solar panel on the solar terminal as well as the Vs and Gnd pins of the MCU. If all connections are correct, the voltage should read at least 1 v as before.

<p align="center">
<img src="../../img/solar-panel/solar_test.jpeg" width="50%">
</p>

# Stage 8 - close up and mount sensor

Flatten and twist the sensor wires so they will not be in the way of any components when the cover is on. Close the cover, ensuring no wires are in between the housing and cover. Fasten four screws tightly.

<p align="center">
<img src="../../img/ML22F/close_cover.jpeg" width="50%">
</p>

Tighten gland around cable to ensure no water infiltration is possible.

<p align="center">
<img src="../../img/general/tighten_gland.jpeg" width="50%">
</p>

Add a label to both sides of the sensor housing.

<p align="center">
<img src="../../img/general/label.jpeg" width="50%">
</p>

Locate 2 mount plates and 4 6/32 screws.

<p align="center">
<img src="../../img/general/mount.jpeg" width="50%">
</p>

With the bubble level holes facing away from the housing, attach the mount plates by threading 2 screws each through the holes in the housing and into the interior threaded holes in the plates. Fasten tightly.

<p>
<img src="../../img/ML22F/mounted.jpeg" width="45%">
<img src="../../img/ML22F/mounted_top.jpeg" width="45%">
</p>
