# CS3081 Bayesian Network Lab: Likelihood and Inference

**Faisal Alburti — Effat University**

## Submission files

- [bn_lab.ipynb](bn_lab.ipynb): executed Python notebook with all outputs, the network and CPTs, joint probabilities, inference queries, enumeration, and answers to Q13, Q14, Q16, and Q18.
- [BN_Lab_Calculations.pdf](BN_Lab_Calculations.pdf): step-by-step calculations for steps 3, 4, and 6.

## Run

Use Python 3.10 or newer. Install `pip install -r requirements.txt`, open `bn_lab.ipynb` in VS Code with the Python and Jupyter extensions (or Google Colab), and run all cells in order. The notebook was verified with Python 3.13.18 and pgmpy 1.1.2.

The model uses Rain → Maintenance, Rain → Train, Maintenance → Train, and Train → Appointment. All CPT values follow the lab instructions.

## Verified results

| Calculation | Result |
| --- | --- |
| Normal-day joint probability | 0.3402 |
| Bad-day joint probability | 0.0024 |
| P(train delayed) | 0.213 |
| P(no rain given delayed train) | 0.4601 |
| P(heavy rain given missed appointment) | 0.1544 |
| P(maintenance yes given delayed train and heavy rain) | 0.1176 |

All nine code cells executed successfully. The final cell checks the model, the joint probabilities, and agreement between enumeration and variable elimination.
