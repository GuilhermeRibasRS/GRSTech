# GRSTech
Automotive OBD2/CAN data logger and real-time dashboard for Raspberry Pi.
Car Logger
Automotive data logger and real-time telemetry dashboard designed to run on Raspberry Pi.

The project is designed to acquire vehicle data through OBD2 and CAN Bus, display engine parameters in real time, and record data for later analysis.

Features
Real-time engine data monitoring

OBD2 communication

CAN Bus support

RPM monitoring

MAF monitoring

MAP monitoring

Throttle Position (TPS)

Ignition timing

Engine Coolant Temperature (ECT)

Intake Air Temperature (IAT)

Fuel trims

Lambda / AFR when available

Vehicle speed

Battery voltage

Data recording

CSV export

Real-time dashboard

Raspberry Pi support

Architecture
                 VEHICLE
                    │
                    │ OBD2 / CAN
                    ▼
              ┌─────────────┐
              │     ECU     │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ CAN / OBD2  │
              │  Interface  │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ Raspberry   │
              │    Pi      │
              └──────┬──────┘
                     │
             ┌───────┴────────┐
             ▼                ▼
        Data Logger       Dashboard
             │                │
             ▼                ▼
           CSV            Real-time
                          telemetry

Hardware
The initial target platform is Raspberry Pi.

Possible hardware configurations include:

Raspberry Pi 3 / 4 / 5

OBD2 interface

CAN Bus interface

MicroSD card

Display or touchscreen

Hardware requirements may vary depending on the vehicle and ECU.

Software
The project is primarily developed in Python.

Main components:

OBD2 communication

CAN Bus communication

Parameter decoding

Data acquisition

Data logging

Dashboard

CSV export

Data Logging
Example recorded parameters:

Parameter	Example
RPM	3247 rpm
MAF	42.3 g/s
MAP	102 kPa
TPS	37 %
Ignition	28.5°
ECT	91 °C
IAT	38 °C
AFR	14.2
Speed	82 km/h
Battery	13.8 V

Actual parameters depend on the vehicle ECU and available OBD2/CAN data.

Project Status
🚧 Early development

The project is currently being developed and tested on Raspberry Pi hardware.

Planned development includes:

 OBD2 communication

 CAN Bus communication

 Real-time dashboard

 Data recording

 CSV export

 Configurable dashboards

 Graphs and data analysis

 Automatic startup

 Touchscreen interface

 Multiple vehicle profiles

 External sensor support

 GPS telemetry

 Wideband lambda integration

Disclaimer
This project is intended for development, testing, diagnostics and motorsport applications.

Vehicle communication and available parameters vary between manufacturers, models and ECUs.

Always verify the electrical and communication requirements of the target vehicle before connecting hardware.

License
License to be defined.
