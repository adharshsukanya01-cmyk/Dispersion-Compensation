# Dispersion-Compensation
# Dispersion Compensation

## Objective
Design and simulate a fiber optic system using dispersion-compensating fiber to reduce chromatic dispersion.

## Theory
<img width="1398" height="500" alt="image" src="https://github.com/user-attachments/assets/a922bb4a-e871-4643-96a5-b78350cfb8d1" />


Therefore, given target values for chromatic dispersion and attenuation loss plus specifications of the transmitter, fiber, and receiver, one can determine the lengths of the transmission fiber and the DCF by solving the above two equations simultaneously.

---

## Specifications
- **Output power:** 0 dBm  
- **Spectral width:** To be determined  
- **Operating wavelength:** 1550 nm  
- **Transmitter bit rate:** 2.5 Gb/s  
- **Transmission Fiber:** Corning SMF-28  
- **DCF:** See below  
- **Receiver sensitivity:** -35 dBm  
- **System margin + coupling loss attenuation:** 6 dB  

**DCF Parameters:**  
- Chromatic dispersion factor: –200 ps/nm-km at 1550 nm  
- Attenuation: 0.5 dB/km at 1550 nm  

---

## Calculations
1. Determine the maximum allowable fiber loss  
2. Determine the maximum allowable chromatic dispersion  
3. Based on the results of (1) and (2), determine the lengths of the transmission fiber and the DCF  

---

## Layout
The main physical components of this layout are:
1. **Transmitter:** Bit sequence generator, non-return to zero (NRZ) pulse generator, and a laser  
2. **Transmission fiber**  
3. **Dispersion compensation fiber (DCF)**  
4. **Receiver:** PIN detector and electrical filter  

**Notes:**  
- The NRZ scheme is used here. The signal does not return to zero between successive 1 bits, resulting in a narrower spectral width than a return-to-zero scheme.  
- Visualizer components included:  
  - Three Optical Time Domain visualizers (at transmitter output, after transmission fiber, and at the end of DCF)  
  - One Optical Spectrum Analyzer (at transmitter output, used to estimate spectral width)  

---

## Procedure
- Adjust the laser power to obtain 0 dBm transmission output.  
- Use the optical spectrum analyzer to determine the spectral width of the signal.  
  - Expect uncertainty since the spectrum is not clean.  
  - Provide a screen capture showing markers used to determine spectral width.  
- Set appropriate fiber lengths based on pre-lab calculations.  
- Run the simulation with all parameters set according to specifications.  
- Generate screen captures for inclusion in the report.  
- Measure:  
  - Optical power at receiver input  
  - Maximum Q factor  
  - Minimum BER  
- Record:  
  - Eye diagram  
  - Optical waveforms at transmitter output, junction between fibers, and receiver input  

---

## Further Simulation and Analysis
- Set the DCF length to 0 and run the simulation again.  
- Record similar measurements for comparison.  
<img width="971" height="728" alt="84b548a6-19ff-455a-9ba0-b57af429742c" src="https://github.com/user-attachments/assets/f6bd90de-8dc9-4ed5-a36e-4dc75593fe67" />
<img width="975" height="729" alt="0af3e36e-5879-4770-9a79-52fb783ffe09" src="https://github.com/user-attachments/assets/d71e29a2-1d5b-4787-b5f1-e040eb5a7d7a" />
<img width="977" height="735" alt="fa963ddf-fbd8-4a12-8e32-785d67906a8a" src="https://github.com/user-attachments/assets/9b21ee11-0614-46c5-9d1e-83faaf047b53" />

---

## Conclusions
Discuss the effectiveness of dispersion-compensating fiber and the ability of the calculations to engineer a viable system.
<img width="899" height="1599" alt="d7cf5955-502d-44f7-acce-b285aedc749e" src="https://github.com/user-attachments/assets/934bdb8f-1439-47a5-a0d5-a5765d6d3ee9" />
