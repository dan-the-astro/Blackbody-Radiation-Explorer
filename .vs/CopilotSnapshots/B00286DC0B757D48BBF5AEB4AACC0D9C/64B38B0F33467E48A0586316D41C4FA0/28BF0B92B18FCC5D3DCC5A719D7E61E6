# Blackbody Radiation Explorer

A Windows Forms application for visualizing blackbody emission spectra at different temperatures using Planck's law.

## Features

### 1. **Interactive Spectrum Visualization**
- Displays spectral radiance vs. wavelength for blackbody radiation
- **Toggle between linear and logarithmic Y-axis** - switch scales instantly!
- Automatic tight auto-scaling based on displayed data
- Multiple temperature curves can be plotted simultaneously

### 2. **Temperature Control**
- Add temperatures from 100 K to 50,000 K
- Default temperatures include:
  - 3000 K (Incandescent light bulb)
  - 5778 K (Sun's surface temperature)
  - 8000 K (Hot star)
- Remove individual temperature curves
- Each curve is color-coded with a legend

### 3. **Wavelength Range Adjustment**
- Customize the X-axis range (1-10,000 nm)
- Default range: 100-3000 nm (UV to near-IR)
- Automatically updates all curves and Y-axis scaling when range changes

### 4. **Display Options**
- **Logarithmic Y-Axis** (default): Shows log₁₀ of spectral radiance
  - Best for viewing data spanning many orders of magnitude
  - 5% padding for optimal viewing
- **Linear Y-Axis**: Shows actual spectral radiance values
  - Better for comparing absolute differences
  - 10% padding for clearer visualization

### 5. **Spectral Radiance Comparison**
- Compare spectral radiance values at any specific wavelength
- Results displayed in scientific notation
- Sorted from highest to lowest radiance

## Physics Background

The application uses **Planck's Law** to calculate spectral radiance:

```
B(λ,T) = (2hc²/λ⁵) × 1/(e^(hc/λkT) - 1)
```

Where:
- B(λ,T) = Spectral radiance (W·sr⁻¹·m⁻³)
- λ = Wavelength (m)
- T = Temperature (K)
- h = Planck's constant (6.626 × 10⁻³⁴ J·s)
- c = Speed of light (2.998 × 10⁸ m/s)
- k = Boltzmann constant (1.381 × 10⁻²³ J/K)

## How to Use

1. **Adding a Temperature Curve:**
   - Enter a temperature value in the "Temperature (K)" field
   - Click "Add Temperature"
   - The curve will appear on the plot with a legend entry
   - **Y-axis automatically scales to fit all curves!**

2. **Removing a Temperature Curve:**
   - Select a temperature from the list
   - Click "Remove Selected"
   - **Y-axis rescales to remaining data**

3. **Changing Wavelength Range:**
   - Enter minimum and maximum wavelength values (nm)
   - Click "Update Range"
   - All curves will be recalculated and redrawn
   - **Y-axis rescales to show only data in the new range**

4. **Switching Y-Axis Scale:**
   - Check "Logarithmic Y-Axis" for log₁₀ scale (default)
   - Uncheck for linear scale
   - **All curves instantly update to new scale**
   - Y-axis label automatically updates

5. **Comparing at a Specific Wavelength:**
   - Enter a wavelength value in the comparison section
   - Click "Compare"
   - View the spectral radiance for all plotted temperatures at that wavelength

## Technical Details

- **Framework:** .NET 8 (Windows Forms)
- **Charting Library:** ScottPlot 5.0
- **Y-Axis Modes:**
  - **Logarithmic**: Displays log₁₀(spectral radiance) with tight auto-scaling
  - **Linear**: Displays actual spectral radiance values
- **Auto-scaling:** Dynamic padding (5% for log, 10% for linear)
- **Units:**
  - Temperature: Kelvin (K)
  - Wavelength: Nanometers (nm)
  - Spectral Radiance: W·sr⁻¹·m⁻³

## Applications

This tool is useful for:
- Understanding blackbody radiation physics
- Astronomy and astrophysics education
- Thermal radiation analysis
- Comparison of stellar temperatures
- Visualizing Wien's displacement law and Stefan-Boltzmann law

## Notes

- **Logarithmic scale** is recommended for most cases as blackbody radiation spans many orders of magnitude
- **Linear scale** can be useful for focusing on absolute differences in specific wavelength ranges
- Y-axis adjusts based only on data within the current wavelength range
- Auto-scaling ensures curves always fill the plot optimally
- Colors are automatically assigned from a predefined palette
- Up to 8 different colors are available before they repeat
