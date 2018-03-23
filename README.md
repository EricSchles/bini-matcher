# bini-matcher

The goal of this project is to take all the models found in [scikit-learn](http://scikit-learn.org/stable/) 
and implement mini-batch versions of those models.  The final goal of this project is to be able to run cross-validated versions 
of each model as well as in ensemble for better accuracy and training of models. 

## Phases

This project will take place over several phases:

### Phase 1 - Research

In the first phase reasonable alternative implementations of scikit-learn models will be captured and stored here.

1. Random forest

Providence: https://stackoverflow.com/questions/41384604/updating-a-fitted-sklearn-random-forest-model

Implementation: https://github.com/balajiln/mondrianforest

### Phase 2 - Collection of disperate code bases

As you can see from above, most of these models are implemented seperately and will need to be brought together and
refactored into a set of consistence conventions and interfaces.

Sub steps here:

1. code refactor
2. API design (matching sklearn)
3. testing and evaluation

### Phase 3 - Merging with scikit-learn

Once this code base is complete, the intention is to get it merged with scikit-learn.  Maintaining this project over the
long term is probably going to be pretty hard.  But over the short term it should be easy to get things in working order.

Here this will be about openning PRs against each existing model to add a partial_fit method that calls these implementations of the models.

