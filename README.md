# Airfoil Aerodynamic Performance Surrogate Model in Incompressible Flow Regime

## Overview

Optimal airfoil design traditionally relies on expert knowledge, resource-intensive CFD simulations, and manual iteration—often without guaranteeing optimal results. To overcome this, a surrogate modeling framework was developed to rapidly estimate aerodynamic performance for incompressible flow conditions. Four regression-based surrogate models were trained—Deep Neural Network (DNN), Random Forest (RF), Gradient Boosting Regression (GBR), and Multiple Polynomial Regression (MPR)—to predict aerodynamic coefficients (lift coefficient, drag coefficient, and moment coefficient). A total of 12,10,657 samples were used to train the models that were generated using Xfoil simulations [10]. The input features for all models consisted of Mach number, Reynolds number, Angle of Attack, and airfoil geometry (MPT and coordinate-based). Among the developed models, the random forest model consistently demonstrated the highest predictive accuracy, achieving the lowest mean square error of 0.00033 for Cl, 0.00002 for Cd, and 0.00001 for Cm on the MPT-based dataset. The results highlight the capability of random forest to serve as an efficient surrogate for aerodynamic analysis, significantly reducing the time required for estimation of aerodynamic performance without signs of overfitting. Furthermore, these surrogate models can train generative AI to automatically produce optimal airfoil designs for target flight conditions, eliminating the need for manual iteration.

## Getting Started

### Prerequisites

- Python 3.10
- Dependencies listed in `requirements.txt`

Install all required packages:
```bash
pip install -r requirements.txt
```

## Applications

- Airfoil design optimization
- Real-time aerodynamic predictions for control systems
- Educational demonstrations of surrogate modeling concepts


## License

This project is open source under the MIT License. See [LICENSE](LICENSE) for details.

## Contact

For questions or collaborations, please reach out via GitHub issues or directly contact the repository owner.
