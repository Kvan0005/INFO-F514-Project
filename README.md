# INFO-F514: Visual Cryptography 

## About The Project
This repository contains the implementation and critical analysis of the Visual Cryptography scheme originally introduced by Moni Naor and Adi Shamir in 1994[cite: 1]. 

The core idea of this scheme is to share a secret image among $n$ participants in such a way that any $k$ participants can recover the image simply by stacking their printed shares (transparencies) together[cite: 1]. This process requires absolutely no computational power or cryptographic keys for decryption, relying entirely on the human visual system[cite: 1]. 

This project explores the theoretical foundations of the scheme (information-theoretic security) and evaluates its practical limitations in real-world scenarios, specifically regarding pixel expansion ($m$) and visual contrast ($\alpha$) degradation[cite: 1].

## Repository Structure
*   **`src/`**: Contains the main implementation code.
    *   `main.ipynb`: The Jupyter Notebook containing the Python implementation and visual results of the schemes.
    *   `holo_chibi.png`: Sample image used for testing the cryptographic schemes.
*   **`paper/`**: Contains the full project report detailing the mathematical background, manual verifications, and critical analysis.
*   **`doc/`**: Additional project documentation.
*   **`requirement.txt` & `pyproject.toml`**: Dependency management files.

## Implementation Status & Results
Our implementation focuses on a functional, non-OOP approach to directly translate the paper's mathematical concepts into Python code[cite: 1]. 

Current progress is as follows:
*   **3-out-of-3 scheme:** Fully implemented and works as expected[cite: 1].
*   **$k$-out-of-$k$ scheme (Construction 2):** Fully implemented and functioning correctly[cite: 1].
*   **$k$-out-of-$n$ scheme (Construction 1):** Implemented, but currently does not work as expected due to missing mathematical details and confusing nomenclature within the original paper[cite: 1].
*   **$k$-out-of-$n$ scheme (Construction 2):** Not implemented, as it serves as a relaxation of the broken Construction 1[cite: 1].

## Tech Stack
The project is built using:
*   **Python 3.14**[cite: 1]
*   **Jupyter Notebook** (for interactive execution and visualization)[cite: 1]
*   **NumPy** (for efficient array and matrix handling)[cite: 1]
*   **Matplotlib** (for plotting and rendering the visual shares)[cite: 1]
*   **Galois** (for finite field arithmetic)[cite: 1]

## Getting Started
To run the implementation locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Kvan0005/INFO-F514-Project.git](https://github.com/Kvan0005/INFO-F514-Project.git)
    cd INFO-F514-Project
    ```

2.  **Install dependencies:**
    Using `pip` and the provided requirements file:
    
```bash
    pip install -r requirement.txt
    ```

3.  **Run the notebook:**
    Navigate to the source folder and launch Jupyter:
    ```bash
    cd src
    jupyter notebook main.ipynb
    ```

## Authors
**Group U (ULB - INFOF514 - 2026)**[cite: 1]
*   Erwan Reynders[cite: 1]
*   Theo Deville[cite: 1]
*   Tristan Bricusse[cite: 1]
*   Kevin Vandervaeren[cite: 1]
*   Nkweya Tofeun Constance[cite: 1]
