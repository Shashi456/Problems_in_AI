# Unsolved/ Major Current Problems in Deep Learning and Artificial Intelligence. 
> Inspired by MIT Media labs Synthetic Neurobiology Labs, List of unsolved problems in Biology, I've decided to try and create a list for AI and DL. [CC: Thanks to Riva for this [tweet](https://twitter.com/rivatez/status/1121733391043502081)]


## Natural Language Processing

- Is perfect computational word-sense disambiguation attainable by using software? If yes, how and why? If no, why? (This presupposes the solution to the unsolved problems in the other areas of linguistics as a basis.)<sup>[[1]](https://en.wikipedia.org/wiki/Word-sense_disambiguation)</sup>
- Is there an objective gauge for the quality of translation?<sup>[[citation needed]]()</sup>
  - Although in the Machine Translation space, BLEU scores currently exist, it's primarily a score for evaluating against a reference, if we truly want to surpass a human level translation, a better objective is needed.
- Is there an objective gauge for the quality of a summary?<sup>[[citation needed]]()</sup>
  - As mentioned in the case of BLEU scores, Summarization has ROUGE scores.
- Natural Language Understanding 
  - Understanding Language is not just about assimilation but also about appreciating and extrapolating from it.
  - Current problems for NLI include SNLI and MNLI, but is predicting a result from a premise and hypothesis true NLI is something we should explore, maybe a reformalization of the task can also be looked at. 
- AI peer review<sup>[[3]](https://www.wired.com/2017/02/ai-can-solve-peer-review-ai-can-solve-anything/)</sup>
- Pure Abstractive summarization
  - I think what we currently are stuck at is solving the dataset, in this case the CNN-Daily Mail Dataset, which has its own flaws and is skewed towards extractive summarization. 




## AI systems 

- Exhibiting Common Sense<sup>[[citation needed]]()</sup>
  - Might sound farfetched but true AI systems have to exhibit common sense to some degree if not completely. I do not know anyone actively working in this area of research. 
- Dealing with Unexpected circumstances <sup>[[citation needed]]()</sup>
  - One of the pitfalls of AI systems, currently is assuming the existence of near perfect environments, We need to create environments which are probabilistic in the sense that they might throw something randomly into the environment. 
- Fair AI systems and an objective gauge of Fairness in Ai systems <sup>[[citation needed]]()</sup>
  - In the past year or so, we have seen how AI systems are unfair and that this is a function of the data they have been trained on because human curation has let the biases of humans seep into the data and that data inherently when rawly collected has biases imbued as well. 
  - To solve this problem, One of the primary things to do is what is the meaning of fairness and how do you objectively gauge it?
  
  


## AI Safety

[ The following problems were raised by the paper [here](https://arxiv.org/pdf/1606.06565.pdf)]

The following problems are problems of Accidental AI risks, where accidents are defined as uninted and harmful behavior that might emerge from Machine Learning systems.

- Avoiding Negative Side Effects
  - One thing we've found about RL agents is when they tend to optimize over an objective function it tends to explore the environment thoroughly(something which is desired), but within a multi-faceted environment, that might not be desired and can lead to very bad consequences.
  - So the problem here is to design objectives which optimize on X but avoiding side effects. 
  - The final outcome of these approaches need to limiting the effects of an ai agent on the environment.
  - Some approaches that can be explored here are : 
    - Define an Impact Regularizer 
    - Learn an Impact Regularizer
    - Penalize Influence
- Avoiding Reward Hacking
  - Rl agents often when trying to optimize on a reward function, sometimes find loopholes in the environment/system and basically exploit this to gain high rewards. Although smart, this is something that is not desired, this can be basically thought of as reward hacking. 
  - Some Approaches that can be looked at are as follows: 
    - Adversarial Reward Functions 
    - Reward Capping
    - Multiple Rewards [ Has an active area of research] 
- Scalable Oversight<sup>[[4]](https://ai-alignment.com/semi-supervised-reinforcement-learning-cf7d5375197f)</sup>
  - Designing Reward functions is a very difficult task, and even though we are successful at RL, it's somewhat limited by this designing because a complex reward function can't really have an objective gauge so we instead rely on cheap approximations which just work in a current problem.
  - Scalable oversight is about when humans are involved in the process, we have limited budget of how much we can help the system, so how do we design RL systems which can be independent yet perform well. One approach spoken about in the paper is Semi-supervised RL. 
  - A few approaches to look at are as follows : 
    - Hierarchichal Reinforcement Learning [Being worked upon currently, has an active area of research].
- Safe Exploration [ Has an Active area of Research ] 
  - Reinforcement Learning mostly depends on exploring environments, exploring an environment also entails the risks that the environment might present. Although it's inexpensive in simulations, since AI systems are becoming more autonomous and real world, we need some ways so that agents explore environments without causing insidious harm. 




TODO : 
  - [ ] Computer Vision 
  - [ ] Reinforcement Learning 
  - [ ] AI Policy
  - [ ] Adding more problems to other key areas.


