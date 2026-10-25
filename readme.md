# [SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]

Parameter definition
Radar parameter calculation and setting
Simulation scene parameter settings
Antenna size
The azimuth angle of the antenna (Squint angle) is equal to 0, which means it is facing directly forward.
Antenna weighting form: rectangular weighting or sinc weighting
λ  
It is the wavelength of radar signals.
λ=cfc  
(Under the central frequency of 10GHz, $\lambda = 0.03m$).
R is the range to the target (10km).
L one z
It refers to the azimuth dimension of the antenna.
Affects the azimuth resolution, which is determined by the antenna aperture and the oblique angle:
Δx a z = λRL a z
Among them:
For 10m azimuth resolution:
L a z = 0.03 × 1000010 = 30m
For 1m azimuth resolution:
L a z = 0.03 × 100001 = 300 m
Therefore, to achieve a 10m azimuth resolution, the antenna size needs to be 30m; to achieve a 1m resolution, the antenna size requires 300m.
Δr=c2B  
Among them:
For 10m distance resolution:
B = c2 × 10 = 15 megahertz
For 1m resolution:
B = c2 × 1 = 150 megahertz
C is the speed of light.
B is the bandwidth of LFM signals.
Pulse Width: According to the SAR resolution requirements, the radar's range-directional resolution ($\Delta r$) can be determined by the following formula:
Antenna parameters:
Scenario parameters: The radar is 10 kilometers away from the scene center, with a bearing-distance of 120m×520m. The radar is at an elevation of 0 meters.
Target parameters: 25 RCS equal to 1 ideal point targets uniformly distributed within the range of azimuth-50m~+50m and distance-250m~+250m centered around the scene center.
(1) Input parameters:
Scenario parameters: The radar is 10 kilometers away from the scene center, with a bearing-distance of 120m×520m. The radar is at an elevation of 0 meters.
Target parameters: 25 RCS equals to 1 ideal point target, evenly distributed within a range of -50m~+50m and -250m~+250m around the scene center.
LFM signal parameters: Center frequency 10.0GHz, pulse width 30us.
SAR's azimuth angle is equal to 0, i.e., orthogonal side-looking.
Antenna weighting form: Rectangular weighting or sinc weighting.
Resolution has two situations: (1) 10m×10m; (2) 1m×1m.
(2) For the two resolutions, complete echo simulation:
Design the transmit LFM signal bandwidth, ensure the image resolution requirements, while not excessively increasing the amount of data in the simulation.
Design the antenna size, ensure the distance-coverage of the scene signal, the image resolution requirements, while not excessively increasing the amount of data in the simulation.
Design the radar receiver gate start time and end time, ensure that every target in the scene will be completely received, while not excessively increasing the amount of data in the simulation.
Design two directions of oversampling factor (best consistent), make the sampling ambiguity in distance and azimuth direction can be ignored, while not excessively increasing the amount of data in the simulation.
Simulate SAR echo signals by orthogonal demodulation reception method, observe the signal's time and frequency domain waveforms.
(3) Complete the analysis of echo signals, understand the characteristics of azimuth-direction signal:
Analyze the time-frequency distribution of echo signals in azimuth direction, from the perspective of signal understanding the principle of high resolution in azimuth direction.
Analyze the characteristics of echo signals in two-dimensional time domain, two-dimensional spectrum, and distance Doppler domain.
Analyze the distance-compressed echo data, understand the characteristics of distance migration (RCMC).
(4) Complete pulse compression for each distance-direction pulse.
MATLAB simulation results

## Images

![[SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]](01.jpg)
![[SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]](02.jpg)
![[SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]](03.jpg)
![[SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]](04.jpg)
![[SAR Imaging] Synthetic Aperture Radar (SAR) Backscatter Signal Simulation [with MATLAB Code]](05.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
