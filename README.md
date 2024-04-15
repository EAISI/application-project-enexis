# Enexis - Energy Transition - Data Science case study

## Introduction

Enexis Netbeheer is a regional energy network operator, managing the network in the North, East and South of the Netherlands. They do not sell gas or electricity, though they ensure that energy finds its way safely from the energy suppliers to people’s homes or premises, connecting to approximately 2.6 million households, businesses, and official agencies. They are constantly working on creating a better, smarter, and more efficient grid which is ready for the future.

On June 28 2019, the Dutch cabinet published the [Climate Agreement](https://www.rijksoverheid.nl/actueel/nieuws/2019/06/28/klimaatakkoord-maakt-halvering-co2-uitstoot-haalbaar-en-betaalbaar): the Dutch elaboration of the international climate agreements in Paris (2015). The aim is to significantly reduce CO2 emissions: by half by 2030 compared to 1990. One of the agreements is that 30 energy regions in the Netherlands will investigate where and how best to generate sustainable electricity on land (wind and sun). But also which heat sources can be used so that districts and buildings can get rid of natural gas. Where is space and how much? Are the places socially acceptable and financially feasible? In a Regional Energy Strategy (RES), each energy region describes its own choices. The [National Program RES](https://www.regionale-energiestrategie.nl/default.aspx) supports the regions in making the RES.

## Assignment

We invite you to shed some light on the Enexis case, with CRISP-DM as a guideline.

### Business understanding

Any good project starts with a deep understanding of the customer’s needs. The Business Understanding phase focuses on understanding the objectives and requirements of the project:

**Determine business objectives**: From a business perspective, what does Enexis Netbeheer really want to accomplish and then define business success criteria. For example, why is it important for Enexis to be at the forefront of the energy transition?

**Assess situation**: Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis. How can the business context of the case be used in the analysis of the data?

**Determine data mining goals**: In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective. What insights can be gained from the energy consumption and production data? What can we learn from smartmeter penetration?

**Produce project plan**: Select technologies and tools and define detailed plans for each project phase.

While many teams hurry through this phase, establishing a strong business understanding is like building the foundation of a house – absolutely essential.

### Data understanding

The data is provided in the `data` folder. Consider how this data can help you in solving this challenge:

**Collect initial data**: Acquire the necessary data and (if necessary) load it into your analysis tool. How complete is the data?

**Describe data**: Examine the data and document its surface properties like data format, number of records, or field identities.

**Verify data quality**: How clean/dirty is the data? Document any quality issues.

**Explore data**: Dig deeper into the data. Query it, visualize it, and identify relationships among the data. What kind of business dynamics do you recognize in the data? Which patterns do you see in the historical energy consumption and production (trends, conversion, etc.)? What are your hypothesis on the underlying causes for the patterns that you find?

Based on your initial insights, what would be your advise to Enexis. Use the data to support your advice and present your insights in a compelling story during the interview. We are keen to see not only your results, but also what approach you’ve taken. Use your creativity to find insights that will raise Enexis' interest and shows them the value of their data.

### Data preparation 

This phase, which is often referred to as “data munging”, prepares the final data set(s) for modeling. It has five tasks:

**Select data**: Determine which data sets will be used and document reasons for inclusion/exclusion.

**Clean data**: Often this is the lengthiest task. Without it, you’ll likely fall victim to garbage-in, garbage-out. A common practice during this task is to correct, impute, or remove erroneous values.

**Construct data**: Derive new attributes that will be helpful. For example, convert the day, month, and year features to a single date feature.

**Integrate data**: Create new data sets by combining data from multiple sources.

**Format data**: Re-format data as necessary. For example, you might convert string values that store numbers to numeric values so that you can perform mathematical operations. Additionally, downcasting data can reduce the number of megabytes used by the data.

### Modeling

Here you’ll likely build and assess various models based on several different modeling techniques. Although a predictive model is not the primary aim of this case, energy consumption and production could possibly be modelled using open source metadata that can be linked to postal codes and CBS buurten. This by itself could provide additional insights. This phase has four tasks:

**Select modeling techniques**: Determine which algorithms to try (e.g. regression, neural net).

**Generate test design**: Pending your modeling approach, you might need to split the data into training, test, and validation sets.

**Build model**: As glamorous as this might sound, this might just be executing a few lines of code like “reg = LinearRegression().fit(X, y)”.

**Assess model**: Generally, multiple models are competing against each other, and the data scientist needs to interpret the model results based on domain knowledge, the pre-defined success criteria, and the test design.

Although the CRISP-DM guide suggests to “iterate model building and assessment until you strongly believe that you have found the best model(s)”, in practice you should continue iterating until you find a “good enough” model, proceed through the CRISP-DM lifecycle, then further improve the model in future iterations. 

### Evaluation

Whereas the Assess Model task of the Modeling phase focuses on technical model assessment, the Evaluation phase looks more broadly at which model best meets the business and what to do next. This phase has three tasks:

**Evaluate results**: Do the models and insights meet the business success criteria? Which one(s) should we approve for the business?

**Review process**: Review the work accomplished. Was anything overlooked? Were all steps properly executed? Summarize findings and correct anything if needed.

**Determine next steps**: Based on the previous three tasks, determine whether to proceed to deployment, iterate further, or initiate new projects.

### Deployment

“Depending on the requirements, the deployment phase can be as simple as generating a report or as complex as implementing a repeatable data mining process across the enterprise.” – [CRISP-DM Guide](https://github.com/jads-nl/execute-nhs-proms/blob/master/references/crisp_visualguide.png)

A model is not particularly useful unless the customer can access its results. The complexity of this phase varies widely. This final phase has four tasks:

**Plan deployment**: Develop and document a plan for deploying the model.

**Plan monitoring and maintenance**: Develop a thorough monitoring and maintenance plan to avoid issues during the operational phase (or post-project phase) of a model.

**Produce final report**: The project team documents a summary of the project which might include a final presentation of data mining results.

**Review project**: Conduct a project retrospective about what went well, what could have been better, and how to improve in the future.

## Attribution

This case study, including the data, was generously provided by [Enexis Netwerkbeheer](https://www.enexis.nl/) for teaching purposes. 
