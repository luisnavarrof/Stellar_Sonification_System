# Stellar Sonification System
_A Rule-Based Framework for Generating Structured Sound from Stellar Data_

## Description

**Stellar Sonification System** is a Python-based tool that transforms astrophysical data into algorithmically structured MIDI compositions. By querying real stellar parameters from the [SIMBAD astronomical database](http://simbad.u-strasbg.fr/simbad/), the system maps attributes like effective temperature, spectral type, visual magnitude, and radial velocity into musical elements such as tempo, key, harmonic progression, instrumentation, and rhythmic structure.

Each star produces a unique sonic output shaped by its physical characteristics. The system emphasizes **structured sonification**, using musical form (intro, verse, chorus, bridge) and genre-informed harmonic logic rather than generating arbitrary melodies.  

This tool serves both creative and pedagogical purposes, bridging astronomy and sound design through a deterministic, reproducible mapping pipeline.

## Features

- Query any star from SIMBAD by name (e.g., "Vega", "Lesath", "Sirius")
- Rule-based mapping of stellar attributes to musical parameters
- Automatic generation of structured MIDI files (intro, chorus, bridge, etc.)
- Timbre and rhythm vary by spectral type (O-M classes)
- Continuous tempo modulation from stellar radial velocity
- Deterministic outputs (same star = same MIDI)
- Clean, modular Python code ready for extension

## Output

- `.mid` file for each star, musically shaped by its data
- Sectioned composition (e.g., intro, chorus, outro)
- Optional `.csv` export with structured note data

## Example

```bash
# Set the target star inside the script (e.g., "target = 'Lesath'")
python Stellar_Sonification_System.py
# Output: lesath_sonification.mid
```

## Dependencies
Install required Python packages:
```bash
pip install numpy pandas astroquery astropy pretty_midi pygame
```

## 🙋‍♂️ Author
Developed by Luis (GitHub: @luisnavarrof)

✉️ luis.navarrof@usm.cl

## 📄 License
This project is licensed under the MIT License. Feel free to use, modify, and expand upon it — just provide attribution where appropriate.
