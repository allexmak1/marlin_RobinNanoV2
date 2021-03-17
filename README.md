# marlin_RobinNanoV2
прошивка моего принтера
исходник:
https://github.com/makerbase-mks/Mks-Robin-Nano-Marlin2.0-Firmware

//стартовый код
M140 S{print_bed_temperature}
M104 S{print_temperature}
G1 F200 E-3 ;retract 3mm
G28 ; home all axes
G90
G1 X170 Y20 Z0 F1800

//конец кода
G28 X10
M104 S0
M140 S0
G92 X10
M84
