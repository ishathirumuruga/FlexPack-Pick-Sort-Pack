
# FlexPack: Camera-Free Pick-Sort-Pack Workstation

## Project Overview
FlexPack is a proposed low-cost, 3-axis Cartesian pick-and-place workstation designed to automate repetitive sorting and packing tasks in small workshops.

## Objectives
- Reduce repetitive manual sorting and packing.
- Provide an affordable automation solution.
- Sort parts using weight and estimated width.
- Verify successful pickup and handle pickup failures.
- Automate packing into a configurable grid.

## Main Components
- Aluminium-extrusion frame
- X, Y and Z-axis motion system
- ESP32 controller
- Servo-powered gripper with flexible TPU fingers
- Load cell platform
- Pickup verification sensor
- Sorting bins and packing box
- OLED display and control buttons
- Emergency stop and limit switches

## Operating Workflow
1. Select Teach Mode.
2. Jog the gantry and save the pick point and bin positions.
3. Teach the packing-box corners.
4. Configure rows, columns and parts per box.
5. Select Run Mode.
6. Pick up a part and measure its weight.
7. Estimate part width from gripper position.
8. Select the appropriate bin or packing slot.
9. Verify pickup using a sensor.
10. Retry once if pickup fails.
11. Send the part to the reject bin if retry fails.
12. Stop when the required box count is complete.

## Project Status
Concept and workflow planning. Hardware implementation and performance validation are pending.

## Repository Structure
- `docs/` — workflow and documentation
- `design/` — mechanical drawings and illustrations
- `firmware/` — ESP32 code
- `simulation/` — simulation files

## Future Improvements
- Validate width estimation and pickup detection.
- Implement teach and run modes.
- Test sorting accuracy and packing reliability.
