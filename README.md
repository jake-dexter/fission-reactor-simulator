# Nuclear Reactor Simulator ⚛️  
*An educational fission reactor visualisation built with Python and Pygame.*  

## Overview  
This project models a nuclear fission reactor both mathematically and visually.  
It combines **Monte Carlo nuclear calculations** with an **interactive Pygame interface**, allowing users to experiment with control rod depth and moderator choice to see how these parameters affect reactor stability and power output.  

The simulation was developed as part of a university group project (PHYS205, University of Liverpool).  
My primary contributions included writing and commenting the **Pygame code** (control rods, fuel rods, turbine animation, UI screens), restructuring the report, and editing the video/audio presentation.  

## Features  
- Calculates chain fission energy release using Monte Carlo methods  
- Models moderation efficiency for **H₂O, D₂O, and Graphite**  
- Interactive **control rod insertion depth** (0–100%)  
- Displays **reactor stability** (stable, unstable, dying out)  
- Real-time turbine animation reflecting power output  
- **Help screen** explaining nuclear fission theory for educational use  

## Physics Background  
- Models fission of **U-235**, summing Q-values from decay chains  
- Uses concepts of mean free path, logarithmic energy loss, and moderating ratio  
- Output scaled to reproduce realistic **1 GW power output** at ~20% rod insertion  
- Moderator choice affects neutron thermalisation efficiency (best result: heavy water)  

## Tech Stack  
- **Language:** Python 3.10  
- **Libraries:** Pygame, Numpy, Scipy, Pandas  
- **Environment:** Jupyter Notebook for nuclear calculations, Pygame for interactive UI  

## Controls  
- Select moderator (H₂O, D₂O, Graphite) on start screen  
- Adjust control rod insertion with increment buttons (0.1%, 1%, 5%)  
- View reactor stability indicator and turbine output  
- Access **Help Screen** for nuclear fission background  

## Results  
- Correctly simulates average power output of ~1 GW in line with real-world reactors  
- Demonstrates how rod insertion stabilises or destabilises chain reactions  
- Highlights the role of moderators in slowing neutrons to thermal energies  

## Installation  
Clone the repository and install dependencies:  

```bash
git clone https://github.com/jake-dexter/nuclear-reactor-simulator
cd nuclear-reactor-simulator
pip install -r requirements.txt
```

Run the simulator:  

```bash
python Fission_Reactor.ipynb
```

(Requires Jupyter Notebook and Python 3.10+)  

## Documentation  
The full written report is included in `/docs/PHYS205_Long_Project_Report.pdf` and explains the physics, methods, and results in detail.  

## Status  
Educational visualisation project (completed as part of a group).  
Planned extensions included fuel burnup, beta decay visualisation, and turbine efficiency calculations.  

---
