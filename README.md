# Data Structures & Carbon Emission Analysis

A C++ data structures project that analyses resident transportation and carbon-emission data using both **arrays** and **linked lists**.

The project compares different data representations while performing searching, sorting, age-group analysis, and carbon-emission analysis across multiple city datasets.

## Overview

The system processes resident transportation data from three different datasets:

- City A — Metropolitan City
- City B — University Town
- City C — Suburban/Rural Area

Each resident record contains:

- Resident ID
- Age
- Mode of transport
- Daily travel distance
- Carbon emission factor
- Average travel days per month

The same datasets can be processed using either a custom array-based structure or a custom linked-list implementation.

## Key Features

### Data Structures

- Custom dynamic array implementation
- Custom singly linked list
- Dynamic memory management
- Node-based linked-list traversal
- CSV data loading into both structures

### Searching

Linear searching is implemented for both arrays and linked lists.

The system supports searching residents by:

- Resident ID
- Age
- Age group
- Mode of transport
- Daily-distance threshold

### Sorting

Bubble Sort is implemented independently for arrays and linked lists.

Datasets can be sorted by:

- Resident ID
- Age
- Daily distance
- Carbon emission

Execution time is measured using C++ `chrono` to support basic performance experimentation.

## Carbon Emission Analysis

Monthly carbon emissions are calculated using:

`Daily Distance × Carbon Emission Factor × Average Travel Days per Month`

The system provides:

- Total carbon emissions for each city
- Emissions grouped by transport mode
- Cross-city emission comparisons
- Carbon emissions grouped by age range
- Average emissions per resident

## Age Group Analysis

Residents are divided into five age groups:

- 6–17 — Children & Teenagers
- 18–25 — University Students / Young Adults
- 26–45 — Working Adults (Early Career)
- 46–60 — Working Adults (Late Career)
- 61–100 — Senior Citizens / Retirees

For each group, the program analyses transport usage, preferred transport mode, total emissions, and average emissions per resident.

## Project Structure

```text
Data-Structures/
├── data/
│   ├── dataset1-cityA.csv
│   ├── dataset2-cityB.csv
│   └── dataset3-cityC.csv
│
└── src/
    ├── algorithm/
    │   ├── searching.cpp
    │   ├── searching.h
    │   ├── sorting.cpp
    │   └── sorting.h
    │
    ├── analysis/
    │   ├── agegroup.cpp
    │   ├── agegroup.h
    │   ├── carbon.cpp
    │   └── carbon.h
    │
    ├── structures/
    │   ├── array.cpp
    │   ├── array.h
    │   ├── linkedlist.cpp
    │   ├── linkedlist.h
    │   ├── node.h
    │   └── resident.h
    │
    ├── utils/
    │   ├── loader.cpp
    │   └── loader.h
    │
    ├── main_array.cpp
    └── main_linkedlist.cpp
```

## Technologies & Concepts

- C++
- Data Structures
- Arrays
- Linked Lists
- Dynamic Memory Management
- Linear Search
- Bubble Sort
- CSV File Processing
- Algorithm Performance Measurement
- Data Analysis
- Carbon Emission Analysis

## Project Context

This project was developed as a **team academic project** focused on applying fundamental data structures and algorithms to a real-world data-analysis scenario.

The repository preserves the original Git history and contributor information from the collaborative project.
