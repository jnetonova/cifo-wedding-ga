# Wedding Seating Optimization – Genetic Algorithm

This repository contains the final project for the Computational Intelligence for Optimization course (NOVA IMS). The goal is to design a Genetic Algorithm to arrange 64 guests across 8 tables in a way that maximizes group compatibility based on a predefined relationship matrix.

## Problem Context

Each guest has a score (positive or negative) reflecting their relationship with others. The objective is to seat them in a configuration that increases internal group harmony and avoids problematic pairings.

## Methodology

The algorithm was built in Python and includes:

- A solution represented as a list of 8 tables with 8 guests each (fully covering all 64).
- A fitness function based on summing pairwise relationship scores within each table.
- Three mutation operators and two crossover strategies adapted to the problem.
- Tournament and roulette selection to balance exploration and exploitation.
- Elitism to retain the best solutions across generations.

## Project Files

```
cifo-wedding-ga/
├── data/
│   ├── seating_data.csv
│   ├── relationships.png
│   ├── guests.png
│   └── best_seating_plan.csv     # Ignored in .gitignore
├── notebooks/
│   └── wedding_seating_optimization.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Final Result

The best solution found during testing achieved a fitness score of **65800**. This value reflects the total positive interaction within the chosen seating configuration. A copy of the seating arrangement was exported for inspection.

## Notes

This project was developed independently and iteratively. All parts of the algorithm, from representation to operators, were designed to match the problem context and ensure validity (no duplicated guests, all guests seated, fixed structure).

## Author

João Neto – 20222105  
MSc in Data Science and Advanced Analytics  
NOVA IMS, 2024/2025