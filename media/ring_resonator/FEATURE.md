## Feature: Ring Resonator

![Ring resonator FDTD animation](ring_resonator_showcase.gif)

### What this shows

A bus waveguide coupled to an all-pass ring resonator — a standard
building block in integrated photonics (filters, modulators, sensors).
The animation shows a guided wave launched into the bus, evanescently
coupling into the ring through a narrow gap, and building up inside the
ring as the drive wavelength is tuned to one of its resonances.

### How it was produced

- The device is built from primitive geometry (bus waveguide + ring) and
  simulated with OpticLUME's native 2D time-domain electromagnetic solver.
- A wavelength sweep first locates the ring's resonant wavelengths from
  the through-port transmission spectrum and the in-ring energy spectrum —
  standard resonator characterization.
- The animation re-runs the same device at one resonance with a
  continuous-wave source, recording the field at intervals — the same
  field-movie export available for any device in the app.
- Frames are stylized (dark background, glow rendering) for presentation;
  the underlying field values are raw simulation output.

### Why it matters

This exercises the field solver, guided-mode source injection, boundary
absorption, resonance search, and transient-to-steady-state dynamics —
through the same workflow available in the app (template → run → export
movie).

---
*Implementation details of the solver are not included in this repository.*
