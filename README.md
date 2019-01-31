# 3DPrintProfile
3d Printer Profiles

Folgertech 2020:
x=200
y=190
z=180 Modified

Start Code:
M280 P0 S45 ; Rotate Z Probe
M280 P0 S45; Rotate Z Probe again
M280 P0 S120; Stow Z Probe
G28 ; home all axes
G29 ; bed level check
G1 Z5 F5000 ; lift nozzle

End Code:
M104 S0 ; turn off temperature
G28 Y0  ; home Y axis
G28 X0  ; home X axis
M400    ; wait for buffer to clear (finish homing)
M84     ; disable motors
