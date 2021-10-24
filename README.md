# Neural_Network_Charity_Analysis

## Overview of the analysis: Explain the purpose of this analysis
Mock analysis of bids for charitable funds from mock charity.

## Results: Using bulleted lists and images to support your answers, address the following questions.
  ### Data Preprocessing
  #### What variable(s) are considered the target(s) for your model?
   The target is the IS_SUCCESSFUL variable.
  #### What variable(s) are considered to be the features for your model?
   APPLICATION_TYPE, 	AFFILIATION, 	CLASSIFICATION, 	USE_CASE, 	ORGANIZATION, 	STATUS, 	INCOME_AMT, 	ASK_AMT
  #### What variable(s) are neither targets nor features, and should be removed from the input data?
   EIN, NAME, SPECIAL_CONSIDERATIONS
    
  ### Compiling, Training, and Evaluating the Model
  #### How many neurons, layers, and activation functions did you select for your neural network model, and why?
  3 layers, all sigmoid. One additional layer of 10 neurons was added after the original 2. Of all testing scenarios, this produced the highest accuracy.
  #### Were you able to achieve the target model performance?
  No. Performance decreased with almost all adjustments. Minor adjustments added only two tenths of a percent of accuracy
  #### What steps did you take to try and increase model performance?
  Tried with each column dropped. - BEST: SPECIAL_CONSIDERATIONS
  Tried with both bigger, and smaller bins. - BEST: as is
  Tried with 4, 2 and 1 hidden layers. BEST: 3
  Tried with both more and less neurons on all hidden layers. BEST: as is, 10
  Tried with sigmoid and relu functions. BEST: all sigmoid
  Tried with 1000 epochs. BEST: as is

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
Any other model explored could work. I would have tried the random forest had I not been instructed to prepare a neural network. The image of legibility vs accuracy showed forests to be also of high accuracy.
