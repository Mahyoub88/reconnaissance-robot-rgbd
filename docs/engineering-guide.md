# Reconnaissance Robot — RGB-D Mapping & Remote Control — Engineering Guide

Designed, programmed, integrated and tested a reconnaissance rover combining Kinect-based 3D mapping, ultrasonic 2D mapping, environmental sensing, GPS/GSM reporting and remote control.

## Visual overview

![Functional overview](overview/architecture.svg)

*New explanatory diagram; grouped responsibilities, not an as-built schematic or test result.*

![Engineering workflow](overview/workflow.svg)

*New explanatory workflow; a documentation aid, not evidence that every proposed check was performed.*

## Two mapping paths

Kinect supplies colour and depth to RTAB-Map on Linux for 3D mapping. Ultrasonic sensing supplies a separate 2D mapping path. These are complementary interfaces; Bluetooth mapping data is not described as carrying the Kinect depth stream.

## Control and reporting interfaces

The four-motor rover and touchscreen controller are integrated with nRF control, XBee sensor telemetry, Bluetooth mapping data and GPS/GSM location reporting. Separate channels make it necessary to document which data uses which link.

## The integration constraint

Software builds and Kinect drivers required compatibility work. The retained wired USB connection is a documented engineering decision for the depth-data path. The new diagram is a functional overview rather than a circuit schematic or a claim about undocumented motor-driver wiring.

## Evidence and extension

The public description records design, programming, assembly, integration and testing. Source code, raw maps and physical-build photographs are not present in the inspected repository. The acceptance checklist below is a suggested way to document those artifacts when available.

## Evidence to review or collect

The following are suggested review checks. A checklist entry is not a claimed pass result.

- Driver compatibility and USB depth acquisition.
- RTAB-Map output with scene context.
- Command and telemetry channel mapping.
- Motor/sensor response and location reporting.

## Sources and provenance

- [Published portfolio description](https://mahyoub88.github.io/projects/proj-reconnaissance-robot/).
- [Project README](../README.md) and existing repository files.
- [LinkedIn projects](https://www.linkedin.com/in/mohammed-mahyoub/details/projects/): supplementary descriptions and project media.
- New SVG figures and explanatory text were authored for this documentation update; they are not original photographs or new measured results.
- Original implementation photos and raw results were not available in the inspected public repository; the new diagrams provide explanation without substituting for that evidence.
