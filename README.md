# Reconnaissance Robot — RGB-D Mapping & Remote Control

## Implementation at a glance

Designed, programmed, assembled, integrated and tested a four-motor reconnaissance rover with RGB-D mapping, sensing, telemetry and remote control.

| Responsibility | Documented implementation |
|---|---|
| 3D mapping | Kinect colour/depth acquisition over USB feeds RTAB-Map on Linux. |
| 2D mapping | Ultrasonic sensing forms a separate mapping path. |
| Control and telemetry | Touchscreen control, nRF commands, XBee sensor telemetry and Bluetooth mapping data serve distinct channels. |
| Location reporting | GPS/GSM provides location reporting. |
| Integration decision | Linux builds and Kinect drivers required compatibility work; the wired USB depth-data path was retained. |

The implemented scope is documented in the public project description. Physical-build photographs, raw maps and source code are not in this public repository; the diagrams below explain the system without posing as build photographs.

### Architecture and implementation workflow

![Explanatory functional architecture](docs/overview/architecture.svg)

![Explanatory engineering workflow](docs/overview/workflow.svg)

*Documentation diagrams based on the project scope; original source images and results are captioned separately.*

[Full engineering guide](docs/engineering-guide.md) · [Illustrated case study](https://mahyoub88.github.io/projects/proj-reconnaissance-robot/)

---



**Author:** Mohammed Mahyoub.

Designed, programmed, integrated and tested a reconnaissance rover combining Kinect-based 3D mapping, ultrasonic 2D mapping, environmental sensing, GPS/GSM reporting and remote control.

## Role

End-to-end implementation: system design, programming, assembly, integration, testing and documentation.

## Mapping

Integrated a Microsoft Kinect RGB-D sensor with RTAB-Map on Linux; built the required software and sensor drivers. Used ultrasonic sensing for 2D mapping.

## Interfaces

Integrated a four-motor rover, a touchscreen controller, XBee sensor telemetry, nRF control, Bluetooth mapping data and GPS/GSM location reporting.

## Integration

Resolved software-build and Kinect-driver compatibility issues; retained a wired USB connection for Kinect depth data.

## Technologies

RGB-D, Kinect, RTAB-Map, Linux, Embedded Systems, Telemetry, GPS / GSM

## Links

- [Portfolio project](https://mahyoub88.github.io/projects/proj-reconnaissance-robot/)

## Illustrated project pages

Project-specific diagrams, source media and implementation context:

- [Reconnaissance Robot — RGB-D Mapping & Remote Control](https://mahyoub88.github.io/projects/proj-reconnaissance-robot/)

[Browse all engineering case studies](https://mahyoub88.github.io/projects/)
