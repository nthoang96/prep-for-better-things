## Understanding and Managing Bias in AI Systems
### Bias
**Definition and Nature of Bias**
- Bias in AI often refers to biases in algorithms, which are procedures for solving problems through defined steps.
- Ethics and responsibility in algorithms emerge when applying them to real-world contexts, not just in mathematical operations.

**Simpson's Paradox and Gender Bias Example**
- The Simpson's paradox illustrates how aggregated data can show different trends than individual group data, complicating bias interpretation.
- In a case of gender bias in university admissions, both claims of discrimination and fairness can be true depending on data aggregation and context.

**Bias in Medical Outcomes**
- Studies show disparities in health conditions between racial groups, but removing bias in algorithms by equalizing health assumptions can lead to harmful outcomes.
- *Context matters*: removing bias in health risk algorithms may reduce necessary screenings for higher-risk groups, negatively impacting care

**Bias in Predictive Policing**
- Predictive policing algorithms can create feedback loops by focusing on areas with prior arrests, disproportionately affecting certain racial groups.
- This feedback loop can perpetuate racial disparities and raises ethical concerns about fairness and the role of policing.

**Heterogeneous Data and Bias**
- Differences in populations (genetic, dietary, community factors) lead to heterogeneous data, which complicates bias removal.
- Bias can exist in both homogeneous and heterogeneous data, requiring careful consideration of when and how to address it.

### What is Bias?
**Definitions and Types of Bias**
- Bias has two main definitions: an ethical/cultural one involving unfair prejudice, and a mathematical one involving systematic distortion in statistics.
- There are many cognitive biases in humans and various biases in AI and machine learning, such as sampling bias, reporting bias, and algorithmic bias.

![](biases.png)

**Legal Perspective on Bias**
- Protected classes (e.g., race, gender) are legally safeguarded against bias in many jurisdictions.
- Sensitive characteristics are variables that can introduce bias in algorithms but may be necessary for accurate modeling.
- Legal concepts include disparate treatment (intentional bias), disparate outcome (unequal results regardless of intent), equal opportunity, equal accuracy, calibration, and predictive parity.

**Data and Algorithmic Bias**
- Sampling bias occurs when data is not representative of the population.
- Reporting bias happens when only certain outcomes are recorded.
- Historical bias perpetuates past prejudices in current models.
- Algorithmic bias arises from the design or functioning of the algorithm itself.
- Survivorship bias focuses only on data from successful cases, ignoring failures.

**Mathematical and Practical Challenges in Fairness**
- AI models, such as loan approval systems, face trade-offs when applying fairness constraints across different groups with varying data distributions.
- Strategies like maximizing profit, group-unaware models, demographic parity, and equal opportunity each have limitations and can conflict.
- Achieving a universally fair AI system is challenging due to these inherent trade-offs and heterogeneous data.

### Managing AI Bias
**Understanding Bias in Decision-Making**
- Data alone may not clearly indicate the best decision due to contextual factors, as shown in the example comparing two candidates, Sam and Mo.
- Informal factors like networking opportunities and personal responsibilities can influence outcomes beyond measurable performance scores.

**The ADAPT Framework for Managing Bias**
- Awareness: Identify and measure different types of bias, especially in relation to protected classes or demographics.
- Diversity: Compare various metrics to detect anomalies or trends and involve diverse perspectives in decision-making.

**Analysis and Transparency**
- Analyze underlying causes of bias by investigating unmeasured variables and contextual factors.
- Publish bias data and results to promote transparency, encourage open dialogue, and foster fairness.

**Transformation and Continuous Improvement**
- Be ready to implement changes based on feedback and continuously improve AI models to reduce bias over time.

### Bias from a Data Perspective
**Bias in Data Collection**
- Sampling bias occurs when the sample data is not representative of the population, leading to poor model performance on underrepresented groups, as seen in facial recognition systems trained on celebrity images.
- Survivorship bias arises when only surviving or successful cases are analyzed, ignoring those that failed, exemplified by WWII aircraft armor placement decisions based on returning planes.

**Bias in Reporting**
- Reporting bias happens when only certain outcomes are reported, potentially skewing results.
- Social desirability bias occurs when respondents provide answers they think are socially acceptable rather than truthful, affecting survey data reliability.
- Publication bias refers to the tendency to publish only studies with significant or positive results, which can distort research findings.

**Systematic and Algorithmic Bias**
- Historical bias reflects past prejudices embedded in training data, such as hiring algorithms favoring historically preferred candidates.
- Algorithmic bias can result from uneven or missing data labels across groups, causing inaccurate predictions for underrepresented populations, as in medical risk prediction models.

**Bias in Homogeneous vs. Heterogeneous Data**
- Homogeneous data may cause overfitting and confirmation bias due to lack of representativeness.
- Heterogeneous data can introduce measurement bias, interaction effects, and confounding variables, complicating model interpretation.

**Mitigating Bias**
- Use random sampling, validated measurement tools, and train data collectors to reduce bias.
- Collect diverse data sources, maintain transparency, audit data for bias, and involve diverse perspectives in data analysis and model development.

## Addressing Human Bias through Agreement and Nudging Techniques
### Inter-Annotator Agreement

### Nudging Human Bias - USPTO
### Nudging Human Bias - Other Examples
### Amazon Scraps AI Recruiting Tool That Showed Bias Against Women
### Hotel Fires Robot Staff after Guest Complaints