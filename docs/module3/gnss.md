# GNSS signal and observations

Generally, the signal coming from satellites is composed by

- carrier wave (sinusoid)
- a spreading code (a sequence of 0 and 1 bits/chips)
- low-rate navigation data message.

Both the code and navigation message are phase-modulated on the carrier wave. There are more carrier phases on different frequencies on each satellite.

![GNSS signal](./img/gnss_signal.gif "GNSS signal")[[image source]](https://www.tudelft.nl/citg/over-faculteit/afdelingen/geoscience-remote-sensing/education/bsc-education/reader-on-gps-positioning)

The spreading code is usually publicly available and is embedded in receivers to properly observe it.
There are two kinds of observations: code observations (pseudo-range) or phase observations.

## Code observations (pseudo-range)

The time shift between the received signal and the receiver internal replica is observed. The observed time Is converted in terms of distance by considering the speed of light (), determining the so-called pseudo-range. This observation has an accuracy in the range 30 cm – 3 m.

![Pseudo-range](./img/pseudo_range.png "Pseudo-range")

Nevertheless, the carrier phase is travelling at a lower speed than the one of light c, due to the presence of troposphere and ionosphere and satellite and receiver clocks are not synchronized with GPS time (and the error of receiver clock is usually larger). Therefore, the pseudo-range observation can be written as

\[ {P}_{R}^{S} = c \, \Delta t = \rho + c \left( d{t}_{R} + d{t}^{S} \right) + {I}_{R}^{S} + {T}_{R}^{S} \]

where $\rho$ is the satellite-receiver distance, $d{t}_{R}$ is the receiver clock error, ${I}_{R}^{S}$ and ${T}_{R}^{S}$ are the ionospheric and tropospheric delay, respectively. $\rho$ is expressed as follows:

\[\rho = \sqrt{{\left({X}^{S} - {X}_{R}\right)}^{2} + {\left({Y}^{S} - {Y}_{R}\right)}^{2} + {\left({Z}^{S} - {Z}_{R}\right)}^{2}}
\]

The unknown of the problem are represented by the coordinates of the receiver , , , since the coordinates of the satellites are known from the ephemerides.

![Pseudo-range](./img/pseudo_range2.png "Pseudo-range")
