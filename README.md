# CGx-Gcode-RobotArm
Gcode decoder for Arduino for robotic arms. Works together with InverseK library.

## Gcode Table
### G Codes
Gcode | Syntax | Definition
- | - | -
G0 | G0 Xnn.n Ynn.n Znn.n Wnn.n | Fast Movement to X Y Z [mm] position. [O*ptional*] set approach angle W.
G1 | G1 Xnn.n Ynn.n Znn.n Wnn.n Fnn.n | Controlled Movement at speed F [mm/s].
G28 | G28 | Home position.
G53 | G53 Ann.n Bnn.n Cnn.n Dnn.n Enn.n Fnn.n | Move each servo individually at nn.n [degrees]. Each parameter is optional.
G54 | G54 Ann Bnn Cnn Dnn Enn Fnn | [*Used for calibration*] Move each servo individually using nn [ms] pulse width. Each parameter is optional.

### M Codes
Gcode | Syntax | Definition
- | - | -
M100 | M100 | Close grip.
M101 | M101 | Open grip.
M103 | M103 | [*Used for calibration*] Enable calibration mode.
M104 | M104 | [*Used for calibration*] Disable calibration mode.
M105 | M105 | [*Used for calibration*] Go to first calibration position.
M106 | M106 | [*Used for calibration*] Save current position as first calibration position.
M107 | M107 | [*Used for calibration*] Go to second calibration position.
M108 | M108 | [*Used for calibration*] Save current position as second calibration position.