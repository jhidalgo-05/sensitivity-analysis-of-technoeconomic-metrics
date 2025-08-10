# sensitivity-analysis-of-technoeconomic-metrics
Model-agnostic permutation feature importance to analyze solar PV technoeconomic factors. Focuses on solar performance, economic viability, battery optimization, investment decisions, and policy support to identify key drivers for better PV system design and sustainable energy planning.

Permutation
The goal of this analysis was to develop predictive models for key output variables related
to solar energy systems: Levelized Cost of Energy (LCOE), Net Present Value (NPV),
Energy Yield, and Payback Period. These models supported multiple objectives, including
comprehensive solar performance analysis, economic viability assessment, battery storage
optimization, investment decision-making, and potential policy support.
To interpret model predictions and assess feature importance in a model-agnostic manner,
Permutation Feature Importance (PFI) was implemented using Ridge regression as the base
model. Ridge regression was chosen for its effectiveness in handling multicollinearity, a
notable challenge in the dataset due to several highly correlated variables.
Feature importance was evaluated by measuring the decrease in model performance when
each input variable was permuted independently. This process was repeated for a range
of regularization strengths (alpha values) across models built for each of the four output
variables to identify optimal configurations.
The data analysis was performed in Python using key libraries such as Pandas for data ma-
nipulation, NumPy for numerical operations, Matplotlib and Seaborn for visualization,
and scikit-learn for modeling and evaluation. The dataset was split into training and
testing sets using a 70/30 ratio via train test split, ensuring a substantial portion of
data was preserved for final model evaluation. During model training, 4-fold cross-validation
was applied on the training set to improve robustness, reduce overfitting, and provide more
stable performance estimates
