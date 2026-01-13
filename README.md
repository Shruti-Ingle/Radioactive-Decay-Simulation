# Multi‑Isotope Radioactive Decay Analysis Using Synthetic Data

This project presents a comprehensive computational study of radioactive decay behavior across multiple isotopes using mathematical modeling, synthetic data generation, and statistical analysis in Python. The objective is to simulate real‑world radioactive decay experiments in a **safe, reproducible, and cost‑effective** manner while demonstrating strong foundations in physics, data analysis, and scientific programming.
The project models radioactive decay using the exponential decay law, estimates decay parameters from data, validates results through error analysis, and visualizes trends across isotopes with widely varying decay rates.

This work is suitable for:
* Academic evaluation (minor/major project)
* Research internship screening (physics/data science domains)
* Demonstrating applied scientific computing skills on GitHub
  
Real radioactive experiments involve:
* Safety hazards
* Expensive instrumentation
* Regulatory constraints

To overcome these limitations, this project uses synthetically generated datasets grounded in well‑established physical equations. This approach allows controlled experimentation, parameter estimation, and validation without compromising scientific rigor.

## Theory

### 1. Radioactive Decay Law
Radioactive decay is a random but statistically predictable process governed by the exponential decay equation:

[
N(t) = N_0 e^{-\lambda t}
]

where:
* (N(t)): Number of undecayed nuclei at time (t)
* (N_0): Initial number of nuclei
* (\lambda): Decay constant (probability of decay per unit time)
* (t): Time

### 2. Decay Constant (λ)
The decay constant (\lambda) is an intrinsic property of a radioactive isotope and determines how quickly it decays. Larger values of (\lambda) correspond to faster decay.

### 3. Half‑Life
The half‑life (T_{1/2}) is the time required for half of the radioactive nuclei to decay:

[
T_{1/2} = \frac{\ln(2)}{\lambda}
]

Half‑life provides an intuitive measure of isotope stability and is widely used in nuclear physics, medicine, archaeology, and environmental studies.

## Dataset Description

* **Type:** Synthetic dataset
* **Format:** CSV (`multi_element_radioactive_decay_dataset.csv`)
* **Isotopes:** 20 radioactive isotopes
* **Features:**

  * Isotope name
  * Atomic number
  * True decay constant (λ)
  * Time‑based decay observations

### Why Synthetic Data?

Synthetic data is used due to:
* Safety considerations
* Accessibility constraints
* Ability to control noise and parameters
* Reproducibility of experiments

Despite being synthetic, all data strictly follows **physically accurate decay equations**.

## Methodology

### Step 1: Data Generation
* Decay curves are generated using the exponential decay law.
* Noise can be added to simulate real experimental uncertainty.
* Data is stored in CSV format for reuse and reproducibility.

### Step 2: Parameter Estimation
* The decay constant (λ) is estimated from synthetic decay data.
* Estimated values are compared with theoretical constants.

### Step 3: Half‑Life Computation
* Half‑lives are calculated using both true and estimated λ values.

### Step 4: Validation & Error Analysis
* Percentage error is computed as:

[
\text{Error (%)} = \frac{|\lambda_{estimated} - \lambda_{true}|}{\lambda_{true}} \times 100
]

This validates the robustness of the estimation approach.

### Step 5: Visualization
The project includes multiple plots such as:
* Decay curves for multiple isotopes
* Activity vs time
* Half‑life comparisons
* Error distribution plots

Visualizations help interpret isotope behavior across different decay regimes.

## Technologies & Tools Used

* **Programming Language:** Python
* **Libraries:**
  * NumPy – numerical computation
  * Pandas – data handling
  * Matplotlib – data visualization
* **Environment:** Google Colab

## Results & Observations
* The exponential decay model accurately represents isotope behavior.
* Estimated decay constants closely match theoretical values.
* Error remains within acceptable bounds across isotopes with vastly different half‑lives.
* The approach scales well for large numbers of isotopes.

## Limitations
* Synthetic data cannot fully replicate real detector noise.
* Environmental effects (shielding, temperature) are not modeled.
* Assumes ideal decay conditions.

## Future Scope
* Incorporate real experimental datasets
* Apply machine learning regression for parameter estimation
* Add confidence intervals and uncertainty propagation
* Extend to decay chains and multi‑step reactions
* Deploy interactive visualization dashboards

## Key Learnings
* Practical application of nuclear decay theory
* Scientific data modeling and validation
* Reproducible research workflows
* Visualization‑driven analysis

## Author
Shruti Ingle
