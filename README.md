# Bark Beetle Planning

This work follows on scientific work for the draft article:

Planning for bark beetle disturbance in production forests: A regional forest optimization case study in Norway

Kyle Eyvindsonᵃᵇ*, Victor F. Strîmbuᵃ, Joyce Machado Nunes Romeiroᶜ, Tron Eidᵃ, Annika Kangasᵈ

*Author for correspondence

ᵃ Faculty of Environmental Sciences and Natural Resource Management, Norwegian University of Life Sciences, P.O. Box 5003 NMBU 1432 Ås Norway  
ᵇ Department of Forest Sciences, Faculty of Agriculture and Forestry, University of Helsinki, P.O. Box 27, 00014 University of Helsinki  
ᶜ Division of Biotechnology and Plant Health, Norwegian Institute of Bioeconomy Research, Høgskoleveien 8, Ås 1433, Norway  
ᵈ Natural Resources Institute Finland (Luke), Yliopistokatu 6 B, FI-80100 Joensuu, Finland


This repository provides a research-oriented environment for exploring **bark beetle disturbance simulations** and integrating them with **optimization-based forest planning**. It is designed to support experimentation, comparison of optimization approaches, and analysis of disturbance‑driven management decisions.

The project centers on running stochastic bark beetle simulations, formulating optimization problems around forest management, and evaluating how different planning strategies perform under disturbance risk.

---

## Repository Structure

```
Bark_Beetle_Planning/
│
├── data/                         # Input datasets and simulation outputs
├── Barkbeetle_stochastic.ipynb   # Main notebook: simulation + optimization workflows
├── README.md                     # Project overview (this file)
├── requirements.txt              # A list of python packages needed
└── LICENSE                       # MIT License
```

---

## Project Goals

This repository is intended for researchers, students, and practitioners interested in:

- **Simulating bark beetle dynamics** using stochastic processes  
- **Formulating and solving forest planning problems** under disturbance risk  
- **Comparing optimization paradigms**, including:  
  - Deterministic optimization  
  - Robust optimization  
  - Stochastic optimization  
- **Analyzing and visualizing simulation and optimization results**  
- **Developing reproducible workflows** for disturbance‑aware forest management

The notebook (`Barkbeetle_stochastic.ipynb`) serves as the central workspace for running simulations, building optimization models, and evaluating outcomes.

---

## Getting Started

### Prerequisites

- Python 3.9+
- Jupyter Notebook or JupyterLab
- A linear/integer programming solver  
  (CBC, CPLEX, or Gurobi—install separately if needed)

### Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install numpy pandas matplotlib seaborn pyomo pulp scipy scikit-learn jupyterlab
```

### Running the Notebook

1. Clone the repository:

   ```bash
   git clone https://github.com/eyvindson/Bark_Beetle_Planning.git
   ```

2. Enter the project directory:

   ```bash
   cd Bark_Beetle_Planning
   ```

3. Launch Jupyter:

   ```bash
   jupyter lab
   ```

4. Open and run:

   ```
   Barkbeetle_stochastic.ipynb
   ```

---

## Data Management

Place all input datasets in the `data/` directory.

For large simulation outputs, consider:

- Keeping raw data outside version control  
- Using Git LFS for large files  
- Documenting external data sources clearly  

---

## Tools & Technologies

This project uses:

- **Python** for simulation, modeling, and analysis  
- **Jupyter Notebook / JupyterLab** for interactive workflows  
- **Pyomo** and **PuLP** for optimization modeling  
- **CBC / CPLEX / Gurobi** as external solvers  
- **NumPy, Pandas, Matplotlib, Seaborn** for data handling and visualization  
- **Scikit‑learn** for optional analysis or clustering tasks  

---

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository  
2. Create a feature branch  
3. Commit your changes  
4. Open a pull request  

Please ensure additions are well‑structured, documented, and reproducible.

Questions or comments can be directed to: kyle.eyvindson [at] helsinki.fi

---

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.
