# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

- The purpose was to see if a binary classifier could be created that could predict whether applicants would successful if funded by Alphabet Soup from a dataset.

## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?

- "Is_succcesful" was the target

#### What variable(s) are considered to be the features for your model?

- Affiliation, classification, use_case, organization, status, income_amt, special_considerations, ask_amt

#### What variable(s) are neither targets nor features, and should be removed from the input data?

- EIN and Name

### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

- 80 neurons in the first layer and 30 in the second. with one activation function for the input and a different one for the output. 

#### Were you able to achieve the target model performance?

- No

#### What steps did you take to try and increase model performance?

- Remove the "status" variable, increase the number of layers, increase the number of neurons, convert "ask_amt" to a binary variable (>5000 or not), tried different functions like gelu and leaky_relu.

### Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendatio

- Overall accuracy peaked at around 72% regardless of the steps I took to try and improve performance. 
- A random forest might be more effective. The deep learner was pretty slow when I increased the number of neurons and layers and I could see optimization of the deep learner taking a long time because of it. THe random forest method might be faster to optimize.