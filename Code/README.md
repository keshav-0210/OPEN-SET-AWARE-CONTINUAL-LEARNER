# Code

This folder contains the Jupyter notebooks used during the development of the open-world / open-set continual learning algorithm.

## Notebooks Explanation

### 1. `cifar-10-open-set-learner.ipynb`  
**(Main and current reference notebook)**
This is the **primary notebook** and the one to focus on.

- Uses **only the CIFAR-10 dataset**.
- Implements the **proper open-world / open-set continual learning setup** that is aligned with the **pseudo-algorithm we have written**.
- This notebook represents our **current target formulation** of the problem.

All further development and validation of the method is centered around this notebook.

---

### 2. `dataloader-thesis-ofcl-paper-setting.ipynb`  
**(Earlier / supporting notebook)**

This notebook was created earlier, under the assumption that the experimental setup would closely follow the **OFCL paper**.

- Contains dataloader and dataset settings inspired by the OFCL experimental protocol.
- Was initially prepared as a base implementation for dataset handling.
- Does **not yet reflect the final open-world setup** used in the CIFAR-10 notebook.

Once the CIFAR-10 open-world setup is fully validated, this dataloader notebook can be **modified and extended** to match the same open-world formulation (as implemented in `cifar-10-open-set-learner.ipynb`) and then used for other datasets.

---

## Summary
- `cifar-10-open-set-learner.ipynb` → **current, correct open-world implementation**
- `dataloader-thesis-ofcl-paper-setting.ipynb` → **earlier OFCL-based dataloader, to be adapted later**
