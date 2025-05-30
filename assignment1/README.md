# Galaxy Rotation Curve Simulation

This project simulates the rotation curve of a spiral galaxy by combining the contributions from a stellar disk and a dark matter halo. The simulation uses realistic parameters for a Milky Way-like galaxy and follows proper unit handling throughout the calculations.

## Problem-Solving Approach

1. **Model Components**
   - Exponential disk for the stellar component
   - NFW (Navarro-Frenk-White) profile for the dark matter halo

2. **Implementation Details**

   ### Disk Component
   - Used an exponential surface density profile: Σ(R) = Σ₀ exp(-R/Rd)
   - Calculated rotation curve using Bessel functions (following Binney & Tremaine 2008)
   - Parameters:
     * Total mass: 5×10¹⁰ M☉
     * Scale length: 3.5 kpc

   ### Dark Matter Halo
   - Implemented NFW density profile: ρ(r) = ρs/[(r/rs)(1 + r/rs)²]
   - Parameters:
     * Scale radius: 20 kpc
     * Characteristic density: 10⁷ M☉/kpc³

3. **Technical Implementation**
   - Used Python 3.12 following PEP-8 standards
   - Leveraged key libraries:
     * `astropy.units` for consistent unit handling
     * `scipy.special` for Bessel functions
     * `matplotlib` for visualization
   - All calculations maintain proper units throughout

4. **Numerical Considerations**
   - Careful handling of small radii to avoid numerical instabilities
   - Used appropriate array operations for efficiency
   - Implemented proper unit conversions for consistent results

5. **Visualization**
   - Created a clear plot showing:
     * Total rotation curve
     * Individual disk contribution
     * Individual halo contribution
   - Proper labeling and units on axes
   - Saved high-resolution output

## Results

The simulation produces a realistic galaxy rotation curve showing:
- Rising rotation curve in the inner regions (disk-dominated)
- Flat rotation curve in the outer regions (halo-dominated)
- Total curve matching typical observations of spiral galaxies

## Requirements
- Python 3.12
- NumPy
- Astropy
- SciPy
- Matplotlib
