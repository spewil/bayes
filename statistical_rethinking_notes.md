# Statistical Rethinking 

## 1 

- causal inference is the prediction of intervention
- knowing cause = playing out counterfactuals (imputation)
- ? how do you identify causes that aren't measured but are important 
- DAGs are intuition pumps!!
- Rabbi Low constructed a Golem from clay (a robot!) -- golems are models
- statistical tests are very narrow-- useful for industrial process/quality control
- t-test -- Guinness Brewery science quality 
- null models aren't unique -- many processes produce similar distributions

- DAGs aren't generative models
- make a generative model
- synthesize data
- analyze data (e.g. with Bayesian data analysis)

- Recipe / Workflow:
	- Generative simulation of the sample (DAG is functional relationship, then model these functions)
	- Define estimand (thing to estimate)
	- Develop estimator
	- Validate estimator using generative model
	- Analyze real data, report findings

## 2

- Bayesian data:
	- For each possible explanation of the sample, count all the ways the sample could happen. Explanations with more possible ways to produce the sample are more plausible.
	- There are many processes that produce the data... lots of possible outcomes for the sample, and a likelihood of the current sample
- For each possible true worlds, count the number of outcomes seen in the sample for each possibly world where that sample is seen
- "Things that can happen more ways are more plausible"
- Special things about Bayesian inference
	- No minimum sample size
	- Shape of the posterior embodies sample and its size
	- No point estimates! The entire distribution
	- No one true interval
- posterior for one sample --> synthesize predictive distribution using samples from posterior --> posterior predictive distribution (repeats of the experiment)
- This is all optimal in the "world" of your model


## 3 

- gaussian = additive error -- how many sequences take you far from the center vs staying close
- summed fluctuations tend toward gaussian
- gaussian is a golem for estimating mean and variance (is maximum entropy distribution)

protocol:
- state a clear question
- sketch causal assumptions
- define a generative model
- use model to build an estimator

DAG:
H --> W means W = f(H)

- ** quadratic vs. laplace approximations of posteriors
- priors are there to constrain to expected reality! inputting scientific knowledge (softly)
- producing distributions of functions? the posterior is full of functions with different values (samples) of function parameters (models with different )
- 