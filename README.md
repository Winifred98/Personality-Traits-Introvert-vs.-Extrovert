Dataset Description: Personality Traits Dataset (Introvert vs. Extrovert)
This dataset consists of 2,512 unique observations collected from a personality test aimed at classifying individuals as either Introverts or Extroverts based on a combination of behavioral and social activity indicators.

Structure & Features
The dataset includes 8 variables, covering both numerical and categorical traits relevant to social behavior:
Time_spent_Alone (numeric) – Hours per day an individual prefers solitude.
Stage_fear (categorical: Yes/No) – Whether the individual experiences fear when speaking or performing in public.
Social_event_attendance (numeric) – Frequency of attending social events (scaled 0–10).
Going_outside (numeric) – Frequency of going outdoors per week.
Drained_after_socializing (categorical: Yes/No) – Whether the person feels emotionally exhausted after social interactions.
Friends_circle_size (numeric) – Number of people regularly considered friends.
Post_frequency (numeric) – Frequency of posting on social media (scaled 0–10).
Personality (categorical: Extrovert/Introvert) – Target variable representing classified personality type.

Data Cleaning & Preparation
Missing Values: Present in several numeric variables; imputed using median values.
Duplicates: 48 duplicate rows identified and removed.
Final Dataset Size: 2,512 unique records with no missing values post-cleaning.
Categorical Encoding: Converted relevant character fields into factors for modeling purposes.

Exploratory Summary
Roughly 56% of the individuals were classified as Extroverts, and 44% as Introverts.
Over 1,000 individuals reported experiencing stage fear and feeling drained after socializing — common indicators associated with introversion.

Median values:
Time spent alone: 3 hours/day
Friends circle size: 6 friends
Post frequency: 3 posts

Modeling & Insights
Two classification models were evaluated:
Logistic Regression
Accuracy: 91.8%

Key predictors: Stage_fear, Drained_after_socializing, Friends_circle_size
K-Nearest Neighbors (KNN) (best at k=6)
Accuracy: 94%

Outperformed logistic regression in correctly classifying both personality types.

Final Conclusion: KNN model offered the highest predictive performance for personality classification in this dataset.

