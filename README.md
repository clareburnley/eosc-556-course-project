# eosc-556-course-project
This is my course project on detecting weak clay layers in landslide slopes by simulating a low resistivity layer in a slope.

## Background
This research aims to determine whether surficial geophysical methods can be used to identify and delineate weak clay layers in the subsurface of potential landslide slopes. 

Glaciomarine clays often have a higher conductivity than adjacent units due to the sodium ions in the matrix. DC resistivity methods, which involve injecting a known steady current into the subsurface and measure voltage differences at electrodes, can detect resistivity contrasts in a survey area. This research applies the principles of DC resistivity to a uniform half-space with a thin, continuous layer of highly conductive glaciomarine clay.

## Directory
This repository contains:

- "LICENSE" MIT license
- "environment.yml" conda environment for reproducibility
- "scenario0-resistivity-slope-inversion-initial.ipynb" this is the analysis and inversion on the initial synthetic slope
- "scenario0-resistivity-slope-inversion-smoothest.ipynb" this is the analysis and inversion containing the smoothest recovered model on the initial synthetic slope
- `additional-scenarios` this folder contains analyses and inversions on additional scenarios:
    - "additional-scenario-1-thinner-clay.ipynb" this scenario considers a thinner clay layer than the initial scenario
    - "additional-scenario-2-two-clay-layers.ipynb" this scenario considers two clay layers in the subsurface
    - "additional-scenario-13-lower-conductivity-clay.ipynb" this scenario considers a lower clay conductivity than the initial scenario
    

## Installation Instructions
1. Clone the repository: 
```bash
git clone https://github.com/clareburnley/eosc-556-course-project.git
```
2. Congifure the environment:
```bash 
conda env create -f environment.yml
conda activate eosc-454
```

## Suggested File Navigation
1. Begin by opening and reading the notebook "scenario0-resistivity-slope-inversion-initial.ipynb" to understand the initial model, forward problem, and inversion setup.
2. Run the notebook to conduct the analysis.
3. Open the notebook "scenario0-resistivity-slope-inversion-smoothest.ipynb" and note the different beta/tradeoff parameter used in construction the smoothest inversion.
4. Run the notebook to conduct the analysis.
5. Navigate to the `additional-scenarios` folder.
6. Open each additional scenario notebook and note the changes to the true model geometry and conductivity.
7. Run the notebooks to conduct the analyses.

## AI Use
During this research, generative AI (ChatGPT) was consulted in certain instances of “de-bugging” code and troubleshooting errors such as invalid syntax or outdated commands.  
