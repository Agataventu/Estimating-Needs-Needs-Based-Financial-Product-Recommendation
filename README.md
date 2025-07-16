# Estimating-Needs-Needs-Based-Financial-Product-Recommendation
Leveraging supervised machine learning to estimate user financial needs and recommend appropriate products in line with regulatory requirements and client life stages.
(Developed as a project in the Fintech course at Polimi )

## Summary
The dataset (Dataset_Needs.xls) contains detailed client-level financial and demographic data collected via standardized MIFID/IDD questionnaires, which are mandatory in European financial regulation. These questionnaires capture both objective and subjective characteristics that influence an individual's financial profile and potential investment needs. 
At a high level, the goal of the project is to estimate a client's **investment needs** and the **next best action (NBA)** using client data and machine learning. Our work aligns with MIFID/IDD requirements, focusing on matching client profiles with financial products through **personalized**, **data-driven** approaches. 
In other words, we want to: 

1. Estimate the presence of one or more investment needs (e.g., retirement, inheritance planning, income generation) for each client based on their profile.
2. Recommend the most suitable financial product(s) aligned with those needs.
3. Leverage supervised machine learning to build classifiers that detect specific needs, even when those needs are not directly stated but can be inferred.

Inspired by real-world business use cases, we explored **explicit** and **implicit** need labels, building recommendation models that could assist financial advisors in scalable, ethical, and accurate personalization.

## Project Structure
├── Dataset_Needs.xls     # Main input dataset

├── EstimatingNeeds.ipynb # Feature engineering and base models + voting ensemble models
├── README.md # You are here

### Data Exploration
Power transformations to improve feature distributions.
Outlier removal for inconsistent age–education correlations.

### Feature Engineering
Engineered variables related to income, accumulation goals, and financial education.

### Modeling
- Multi-Layer Perceptron (MLP)
- Voting Classifier (Standard and Stacked)
- One-vs-All classification for need-specific predictions
- Evaluation via ROC curves, feature importance, and recall metrics

### Recommendation Logic
- Client–Product matching using explicit/implicit needs
- Consideration of regulatory constraints (MIFID/IDD)

**Team Members**: Brignoli Ettore Davide, Capoferri Luca, Untila Denis, Venturi Agata  

