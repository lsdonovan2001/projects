# Sequential Analysis and Martingales  
*A structured, teaching-oriented exploration of likelihood-ratio martingales, sequential testing, and time-uniform guarantees.*

This folder contains two complementary components:

- **Poster:** [*Sequential Methods with Martingales*](poster.pdf)

- **Write-Up:** [*Sequential Analysis and Martingales — A Conceptual Overview*](paper.pdf) 

Both materials aim to make modern sequential inference accessible by blending rigorous probability with clear, student-friendly exposition.

---

## Project Overview

Sequential analysis asks a simple but powerful question:

**Can we make statistical decisions *before* collecting all \(n\) samples?**

The classical Sequential Probability Ratio Test (SPRT) answers “yes.”  
Modern martingale methods show *why* the answer is yes, *how* we quantify uncertainty over time, and *what* breaks when the alternative hypothesis is composite.

This project presents these ideas at two levels:

- a **visual poster** optimized for talks and outreach  
- a **detailed write-up** that builds the mathematics step-by-step

---

## Topics Covered

###  **1. Likelihood Ratio Martingales**
- Under \(H_0\), the likelihood ratio process  
  \[
    M_t = \prod_{i=1}^t \frac{p(X_i)}{q(X_i)}
  \]  
  forms a nonnegative martingale.
- This structure enables early stopping.

###  **2. Optional Stopping & Ville’s Inequality**
- Key tool for controlling Type I error uniformly over time
- Shows why sequential tests can “peek” without invalidating inference

###  **3. Composite Hypotheses & Breakdown of Martingales**
- For general \(H_1\), LR no longer forms a martingale  
- Leads to new constructions:
  - **Mixture martingales**  
  - **Exponential-tilt (CGF) martingales**  
  - **Stitching martingales**

###  **4. Practical Experiments**
The write-up includes simulations for Bernoulli data, comparing:

- SPRT  
- Mixture martingales  
- CGF-based martingales  
- Stitched martingales  

and showing how each method balances:

- Type I error control  
- stopping time  
- computational cost  
- robustness to parameter misspecification  

---

##  Pedagogical Focus

The materials emphasize:

### **Intuition before algebra**
Students first see *why* martingales arise in sequential testing.

### **Layered explanation**
Poster → definitions, shapes, and key facts  
Write-up → derivations, proofs, and experiments

### **Tradeoffs & failure modes**
Each method is explained not only in theory, but in context:

- SPRT requires a fully specified alternate  
- Mixture martingales are principled but computational  
- CGF martingales rely on moment assumptions  
- Stitching martingales achieve uniform control but introduce tuning choices


---

##  Skills Demonstrated

- Martingale theory  
- Sequential hypothesis testing  
- Likelihood-based inference  
- Exponential families and CGF methods  
- Simulation and empirical validation  
- Scientific writing  
- Poster design (TikZposter)  
- Communicating abstract probability concepts clearly  

---


