# High-alitiude Univeral Gondola — Concept of Operations (CONOPS)

Version: Draft v0.1
Organization: Balloon Section, Students’ Space Association, Warsaw University of Technology
Project Status: Under Development

---

# 1. Introduction

HUG (High-Altitude Universal Gondola) is a modular stratospheric balloon platform under development by the Balloon Section of the Students’ Space Association at the Warsaw University of Technology. The project aims to provide a standardized, reusable, and extensible flight system for scientific and technological payloads operated during high-altitude balloon missions.

The platform addresses a common limitation of student balloon missions, where gondola structure, avionics, communication systems, and payload interfaces are redesigned for each individual experiment. Ognisty Rydwan introduces a unified flight platform architecture that separates reusable flight infrastructure from hosted experimental payloads.

The system is intended to support repeatable flight campaigns for both internal and external payload teams by providing standardized mechanical, electrical, and data interfaces together with shared telemetry and communication infrastructure.

The long-term objective of the project is to establish a reusable flight ecosystem capable of supporting increasingly complex scientific missions while maintaining low integration overhead for payload developers.

---

# 2. Mission Objectives

## 2.1 Primary Objectives

* Provide a reusable stratospheric balloon gondola platform.
* Standardize payload integration interfaces.
* Reduce mission-specific redesign effort.
* Support repeatable scientific flight campaigns.
* Enable centralized telemetry and communication services for hosted payloads.

## 2.2 Secondary Objectives

* Support educational and student research activities.
* Allow external institutions and teams to integrate payloads.
* Develop scalable flight software and telemetry infrastructure.
* Establish a long-term high-altitude balloon experimentation platform.
* Enable future expansion toward guided recovery and controlled-descent systems.

---

# 3. System Overview

The Ognisty Rydwan platform consists of a reusable flight gondola architecture designed to host multiple experimental payloads during a stratospheric balloon mission.

The core platform includes:

* Mechanical gondola structure
* Electrical power subsystem
* Main onboard computer
* RF communication subsystem
* Telemetry and tracking systems
* Environmental and housekeeping sensors
* Payload interface subsystem
* Flight termination capability

Hosted payloads interface with the platform through standardized integration interfaces that may include:

* Regulated 3.3 V, 5 V, and 12 V power rails
* Ethernet connectivity
* Wi‑Fi connectivity
* Shared telemetry infrastructure
* Mechanical mounting interfaces

The platform is intended to support payloads with varying operational concepts, including:

* Internally mounted payloads
* Thermally isolated payloads
* Externally exposed payloads
* Suspended payload configurations

The system architecture is designed around a payload-centric philosophy in which payload developers interact primarily with standardized interfaces rather than internal gondola implementation details.

---

# 4. Operational Concept

The Balloon Section acts as the primary mission operator and is responsible for launch preparation, flight operations, tracking, mission supervision, and recovery activities.

Payload developers provide experimental modules compliant with the platform integration interfaces and operational requirements.

Prior to flight, payloads are mechanically integrated into the gondola structure and connected to the required electrical and communication interfaces.

Payloads may:

* Operate autonomously
* Use platform-provided electrical power
* Exchange data with the onboard computer
* Access uplink and downlink communication services
* Utilize onboard telemetry and positioning data

The onboard flight computer aggregates telemetry and housekeeping data from both platform subsystems and hosted payloads. During flight, data may be transmitted through the RF communication subsystem to ground infrastructure.

Ground operators monitor mission status in real time using dedicated ground stations connected to a centralized software infrastructure responsible for telemetry distribution, mission monitoring, and payload data access.

The system is intended to support simultaneous operation of multiple payloads while maintaining centralized supervision and mission coordination.

---

# 5. Stakeholders and Roles

## 5.1 Balloon Section Operators

Responsible for:

* Flight preparation
* Gondola integration
* Balloon launch operations
* Mission supervision
* Recovery operations
* Platform maintenance

## 5.2 Payload Developers

Responsible for:

* Payload development
* Compliance with integration interfaces
* Payload testing
* Payload operational readiness

## 5.3 Ground Station Operators

Responsible for:

* Telemetry monitoring
* RF communication supervision
* Data forwarding and logging
* Operational coordination during flight

## 5.4 Recovery Team

Responsible for:

* Tracking the landing location
* Payload recovery
* Post-flight handling

---

# 6. Operational Phases

## 6.1 Payload Integration Phase (Approx. T‑1 h)

Payloads are integrated into the gondola structure according to previously established interface specifications and operational procedures.

Electrical power connections, communication interfaces, and telemetry links are verified.

## 6.2 System Verification Phase

The platform performs pre-flight verification procedures including:

* Power subsystem checks
* Communication link verification
* Payload connectivity verification
* Telemetry validation
* GPS and positioning checks
* Housekeeping sensor validation
* Flight termination system verification

Ground infrastructure connectivity and telemetry forwarding are also verified.

## 6.3 Final Launch Preparation (Approx. T‑30 min)

The gondola is closed and prepared for launch.

The balloon inflation process is initiated and continues until final launch readiness verification.

## 6.4 Launch Phase (T‑0)

The balloon system is released and the ascent phase begins.

The onboard system transitions into flight operation mode and continuous telemetry transmission is initiated.

## 6.5 Ascent and Flight Operations

During ascent and high-altitude operation:

* Payloads perform scientific or technological experiments
* The platform continuously gathers telemetry and housekeeping data
* RF uplink and downlink communication remain active
* Ground operators monitor mission status in real time
* Position, altitude, and environmental conditions are tracked

The system supports continuous monitoring of:

* Internal and external temperatures
* Power consumption
* Battery status
* GPS positioning
* Communication link status
* Payload telemetry

Mission operators may initiate an abort procedure and terminate the balloon flight if required.

## 6.6 Descent Phase

Following balloon burst or commanded termination, the gondola descends under parachute.

Tracking and telemetry systems remain active to support recovery operations.

## 6.7 Recovery Phase

Ground teams track and recover the gondola after landing.

Following recovery:

* Payloads are powered down
* Data is secured and extracted
* Post-flight analysis is performed
* Hardware condition is inspected

---

# 7. Ground Segment

The ground segment consists of dedicated ground stations and centralized telemetry infrastructure.

The system architecture is intended to support:

* Bidirectional RF communication
* Real-time telemetry monitoring
* Telemetry logging and archival
* Payload data distribution
* Mission supervision interfaces
* Remote monitoring capabilities

Ground stations communicate with a centralized server infrastructure responsible for aggregating telemetry and distributing mission data to operators and payload teams.

---

# 8. Payload Operations

Payload developers interact with the platform through standardized integration interfaces documented in dedicated integration manuals and Interface Control Documents (ICDs).

The platform is intended to support payloads with different operational requirements and integration approaches.

Payload teams may:

* Use platform-provided power distribution
* Operate independent internal power systems
* Exchange data with onboard software services
* Access platform telemetry data
* Transmit experiment data through the shared communication system

The project also intends to provide standardized mounting solutions for small or lightweight payloads to simplify integration.

---

# 9. Safety Philosophy

The platform is designed with emphasis on operational safety, mission supervision, and recoverability.

Safety-related operational concepts include:

* Continuous telemetry supervision
* Battery monitoring and protection
* Housekeeping data collection
* Flight termination capability
* Autonomous operation during communication loss
* Redundant tracking capability
* Controlled recovery procedures

The platform is intended to remain operational throughout the complete mission profile, including ascent, float, descent, and recovery phases.

---

# 10. Operational Assumptions and Constraints

The current design assumptions include:

* Payload mass capability up to approximately 2 kg
* Gondola mass of approximately 3 kg
* Operational duration up to approximately 4 h
* Operational altitude up to approximately 30 km
* Ambient external temperatures from +50 °C to −50 °C

Operational constraints may include:

* Weather conditions
* RF communication limitations
* Regulatory flight restrictions
* Battery energy limitations
* Recovery accessibility

Communication coverage may be intermittent depending on mission geometry and environmental conditions.

---

# 11. Future Extensions

The platform architecture is designed to support future capability growth including:

* Guided recovery systems
* Controlled descent mechanisms
* Increased payload mass capability
* Longer mission duration
* Expanded telemetry infrastructure
* Advanced onboard autonomy
* Additional communication subsystems

---

# 12. Conclusion

Ognisty Rydwan is intended to establish a reusable and extensible high-altitude balloon experimentation platform capable of supporting multiple payload types through standardized interfaces and centralized flight infrastructure.

By separating reusable flight systems from mission-specific payload development, the project aims to reduce integration complexity, improve repeatability of balloon missions, and enable broader participation in stratospheric experimentation activities.

The present Concept of Operations document defines the initial operational vision and serves as a foundation for subsequent requirements engineering, interface definition, architecture development, and subsystem implementation activities.
