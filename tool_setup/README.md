# Tool Assembly!
We're going to put together an Opentrons Pipette toolhead! 

### Step 1: Assemble the Pipette
Put together the disassembled pipette! There are instructions [here](https://github.com/machineagency/science_jubilee/blob/main/tool_library/OT2_pipette/assembly_docs/OT2_Pipette_3D_Laser_cut_assembly_instructions.pdf), though some steps have already been completed.

### Step 2: Set the Parking Position
Use the [parking post calibration notebook](https://github.com/machineagency/POSE-workshop/blob/main/tool_setup/SetToolParkingPositions.ipynb) to
to set the pipette parking position. To launch the notebook, open a terminal and use the following commands:

```
cd POSE-workshop
source .venv/bin/activate
jupyter lab
```

Jupyter lab should open and you can navigate the `SetToolParkingPositions' notebook in the tool_setup folder.

### Step 3: Connect the Pipette Electronics
The pipette has a motor, an internal limit switch (for homing), and an external limit switch (for attaching tips).
The places where these should be plugged into the Duet board are defined in the Duet `config.g` file.
Check this file out to find out where you should plug things in.

You'll find the motor drive number in the "Motor Drive to Axis Mapping" section. Look for a `M584 V<board_number>.<drive_number>` command, where the [`M584`](https://docs.duet3d.com/User_manual/Reference/Gcodes#m584-set-drive-mapping)
command sets the drive mapping, board 0 refers to the main board, board 1 refers to the expansion board, and the drive number is the index
on this board that you should plug into. Uncomment this line (i.e. remove the semicolon at the beginning of it)!

You'll find the endstop information a bit further down in the "Endstops and Probes" section. Look for `M574` commands, where the `P` field will tell you the board number and port number to plug into. Look for some helpfule comments in the config file to 
There's more info about the other configuration options in the [docs](https://docs.duet3d.com/User_manual/Reference/Gcodes#m574-set-endstop-configuration).


Hooray! We have a pipette tool!
