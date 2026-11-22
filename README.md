# msc-mathematical-modelling

This repository contains computational work from my MSc in Mathematical Sciences at the African Institute for Mathematical Sciences (AIMS), Ghana.

It mainly presents the computational work associated with my MSc research project, **Modelling the Spread of Infectious Disease in Forest**, supervised by Professor Alex Best of the University of Sheffield.

The project used mathematical modelling and computer simulations to investigate how spatial structure influences the spread of infectious diseases in forest populations and how different management strategies can help control disease outbreaks.

## 1. MSc Research Project: Modelling the Spread of Infectious Disease in Forest

### Background

Trees are fixed in one location and mainly interact with nearby trees. Because of this, infectious diseases in forests often spread through local interactions rather than through random contact across the entire population.

Many traditional epidemic models assume that individuals mix freely. This assumption may not describe how diseases spread among trees. My MSc research addressed this problem by incorporating spatial structure into a classical SEI disease model using a lattice-based pair approximation approach.

### Research Objectives

The main objectives of the project were to:

- Develop a deterministic SEI pair approximation model for infectious disease spread in forest populations.
- Investigate how local interactions and spatial structure influence epidemic dynamics.
- Examine how the balance between local and global transmission affects the size and speed of an epidemic.
- Extend the model to include disease control strategies.
- Compare the effectiveness of continuous and annual surveillance in managing forest disease outbreaks.

## 2. Mathematical Approach

The study developed a spatial SEI pair approximation model.

The model divides trees into three disease classes:

- **S – Susceptible:** Healthy trees that can become infected.
- **E – Exposed:** Trees that have contracted the disease but are not yet showing symptoms.
- **I – Infected:** Trees showing symptoms and able to transmit the disease.

Trees are arranged on a regular square lattice, where each tree has four immediate neighbours.

Unlike a standard mean-field model, which tracks the proportions of individuals in each disease class, the pair approximation model also tracks relationships between neighbouring trees. This allows the model to represent how local interactions influence disease transmission.

The model uses ordinary differential equations to describe changes in both individual tree classes (singlet densities) and neighbouring tree pairs (pair densities).

A pair approximation closure is then used to close the system of equations and make numerical analysis possible.

## 3. Spatial Structure and Disease Transmission

An important part of the research was investigating the role of local and global transmission.

The parameter L represents the proportion of disease transmission that occurs locally.

- When L = 0, transmission is entirely global.
- When L = 1, transmission occurs entirely between neighbouring trees.
- Values between 0 and 1 represent a mixture of local and global transmission.

By varying L, the simulations examined how different patterns of transmission affect epidemic development and final epidemic size.

## 4. Disease Control Strategies

The model was extended to investigate two management strategies.

### Roguing

Roguing involves detecting and removing symptomatic infected trees from the forest to reduce further disease transmission.

The model considers imperfect detection, meaning that not every infected tree is found during surveillance.

### Buffer-zone clearance

Buffer-zone clearance involves removing neighbouring trees around detected infected trees. This includes susceptible and exposed trees that may already have contracted the disease but are not yet showing symptoms.

The study examined how these two strategies work separately and together under different levels of detection and management effort.

### Continuous and annual surveillance

Two surveillance approaches were considered:

1. **Continuous surveillance:** Infected trees are detected and removed throughout the simulation.
2. **Discrete annual surveillance:** Forest surveys are conducted once a year, with the model running freely between surveys.

Comparing these approaches helped investigate how the timing and frequency of surveillance affect disease control.

## 5. Computational Simulations and Analysis

The computational work was used to solve and explore the mathematical model under different parameter values and management scenarios.

The simulations investigated:

- Disease dynamics in the absence of control.
- The effect of different levels of local transmission.
- The effectiveness of roguing.
- The additional effect of buffer-zone clearance.
- The influence of imperfect disease detection.
- The effect of different management intensities.
- Differences between continuous and annual surveillance.

The results were examined using numerical simulations, graphical outputs and comparisons across different scenarios.

The parameter values used in the simulations were taken from estimates reported in the existing study by Best and Cunniffe. The project therefore focused on mathematical modelling and simulation rather than fitting the model directly to a new forest disease dataset.

## 6. Main Findings

The study showed that spatial structure has an important influence on forest disease dynamics.

Some of the main findings were:

- Highly local transmission slowed disease spread and reduced epidemic size compared with more global transmission.
- The relationship between local transmission and epidemic size was nonlinear.
- Combining roguing with buffer-zone clearance reduced disease prevalence more than roguing alone.
- The effectiveness of control depended strongly on the probability of detecting infected trees.
- Improving detection could be more important than simply increasing the speed at which trees were removed.
- Continuous surveillance generally performed better than annual surveillance because it reduced the time available for undetected infections to spread.

These results highlighted the importance of considering both spatial structure and surveillance frequency when developing forest disease management strategies.

## 7. Research Skills and Methods

Through this project, I gained experience in:

- Mathematical modelling of infectious disease dynamics.
- Formulating systems of ordinary differential equations.
- Spatial modelling using pair approximation.
- Understanding local and global transmission processes.
- Numerical simulation of mathematical models.
- Investigating model behaviour under different parameter values.
- Comparing disease control strategies.
- Interpreting computational results in a biological context.

## 8. Repository Contents

This repository contains the original computational codes associated with my MSc research.

The code files are provided in their original form. The README describes the research questions, mathematical approach and simulation work carried out in the project.

## 9. Research Supervision

**Student:** Owusu Agyemang  
**Programme:** MSc Mathematical Sciences  
**Institution:** African Institute for Mathematical Sciences (AIMS), Ghana  
**Research Supervisor:** Professor Alex Best, University of Sheffield  
**Research Project:** Modelling the Spread of Infectious Disease in Forest  
**Year:** 2026

## 10. Thesis

The full research is presented in my MSc thesis:

**Agyemang, O. (2026). _Modelling the Spread of Infectious Disease in Forest._ MSc Thesis, African Institute for Mathematical Sciences (AIMS), Ghana.**
