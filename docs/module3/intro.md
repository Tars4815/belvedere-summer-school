# Introduction

Nowadays there are many positioning systems, owned and managed by different nations / government.
In particular, the main GNSS are:

- GPS (Global Navigation Satellite System) – USA
- GLONASS – Russia
- GALILEO – European Union
- BeiDou – China
- QZSS (Quasi-Zenith Satellite System) – Japan
- IRNSS (Indian Regional Navigation Satellite System) – India

![GNSS constellations](./img/gnss_constellations.png "GNSS constellations")

## Components of a satellite positioning system

A satellite position system is generally composed by the space segment, the control segment, and the user segment.

### Space segment

It is constituted by the satellites orbiting around the Earth, usually guaranteeing an almost global ground coverage. Therefore, the visibility of a minimum number of satellites is possible almost everywhere.
The main satellite tasks are:

- Transmit their positions (ephemeris) as well as the signal required to user segment for navigation / positioning applications,
- Receive and store information from control segment,
- Correct the orbits by on-board rockets, which managed by control segment.

![Space segment](./img/space_segment.png "Space segment")

### Control segment

It is composed by the ground stations used to control and manage the entire satellite
constellation.
Main tasks of the control segment are:

- Tracking the satellites of the space segment
- Determination, prediction, and distribution of satellite ephemeris.

![Control segment](./img/control_segment.png "Control segment")

### User segment

It is composed by the users that would know their position on the Earth. They need a receiver and an antenna.
There are many «level» of instruments, depending on the quality of the on-board electronics:

Geodetic type receivers:

- for monitoring / long static survey purposes

  ![geodetic_receiver_1](./img/geodetic_receivers_1.png "geodetic_receiver_1")

- for real time applications

  ![geodetic_receiver_2](./img/geodetic_receivers_2.png "geodetic_receiver_2")

Low-cost receivers:

- with the possibility of accessing to raw-data

  ![low_cost_receiver_1](./img/lowcost_receivers_1.png "low_cost_receiver_1")

- Embedded in other devices:

  ![low_cost_receiver_2](./img/lowcost_receivers_2.png "low_cost_receiver_2")
