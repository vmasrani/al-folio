---
layout: post
title: Human Decision Making
author: Mauricio Baker
date: 2020-07-17
description: The third in a series.
comments: true
---

_The third in a series with Mauricio Baker on critical rationalism and bayesian epistemology. See [one]({% post_url 2020-07-11-mauricio_first_response %}), [two]({% post_url 2020-07-13-vaden_first_response %}), [three]({% post_url 2020-07-17-mauricio_second_response %}), [four]({% post_url 2020-07-22-vaden_second_response %}), [five]({% post_url 2020-08-06-mauricio_third_response %}), [six]({% post_url 2020-08-06-vaden_final_response %}), and [seven]({% post_url 2020-08-06-mauricio_final_response %})._

---


---

One part of your response that I especially appreciated was your point about how Bayesians / EAs often rely heavily on probabilities with little backing (or none?) as if they were well supported. I'll argue that what EAs are doing that looks like this is often fine, but after reading your last response I expect to be paying more attention to how probability estimates were formed, and to what this implies for their value as information, and for the value of further information.
<!--more-->

There's a few points I want to skip over for now:

> _my main concerns don't really hinge this... I'd rather not argue about the meaning of 'existence' if we can avoid it 🙂_

Fair enough 🙂

As well as:

> _Without [probabilities based on measurements], we are claiming knowledge where we don't have it and this is dangerous._
>
> _...we don't have a total order across explanations, so can't coherently talk about "second best", "third best", etc_
>
> _If the [Future of Humanity Institute](https://www.fhi.ox.ac.uk/) dedicated itself to coming up with societal mechanisms to prevent conflicting ideas from becoming violent, I think it would go much further to achieve its goals_.
>
> _But there are no objective probabilities - no measurements from which to derive probabilities - when dealing with the unconditional future._

Our disagreements on these points seem downstream of another disagreement: do humans in fact make decisions using subjective credences, and should we? I agree that this is "an important disagreement worth spending time on."

To address that question, you write:

> _...What ideal rational agent would use a decision making process which starts with an infinite regress?_

> _Infinite regress isn't a problem when decision theory is used in machine learning, reinforcement learning, econometrics, etc, because the actual decisions are being made by human beings. The word "decision" in this case is just referring to a statistical procedure of learning from data, and is not the same as the (unknown) psychological/biological phenomenon called "decisions" in steps 1-5._

> _"Subjective credences" are often talked about as if they are just formed in your brain automatically and allow us to avoid having to make decisions (and thus avoiding the infinite regress problem). But this isn't true. Try it - try filling in a few entries of the conditional probability table in step 3 for example. What number are you going to write down for p(burns mouth \| drinks tea) = c ? Or p(has a productive day at work \| drinks coffee) = d? What are c and d? One could tally all the times one has burned their mouth drinking tea, but that is collecting measurements and switching back to objective probabilities, which we agree are legitimate._


I understood your argument here as being the following. Please let me know if I misunderstood or am interpreting uncharitably.

Humans do not (and should not) use expected-utility-maximization (of the sort in which consequences are weighted by subjective credences), because attempting to do so requires first making decisions about one's options, probabilistic predictions, and utility functions. This amounts to beginning with infinite regress, which is not a great way to make decisions. Computers that maximize expected value avoid this problem by having humans make these initial decisions, and then updating their probabilities by using data according to programmed rules. If humans worked like this, then we could follow decision theory without falling into infinite regress. However, humans don't work like this--our inability to introspect on precise, numerical subjective credences is strong evidence for the claim that we do not automatically calculate subjective credences. Even if we formed subjective credences by (consciously?) examining data, we would just be following frequentist statistics, and this would not support the claim that Bayesian statistics offer further value.

​My current impression is that humans do work roughly like the computers you mention, in that we are born with (or otherwise develop, without choosing) at least a few assignments of value, credences, and ways of updating our credences based on data.

Could you say more about why you think this is not the case? I know very little about the relevant psychology.

Some reasons why I think that it is the case:
 - Neurons seems roughly Bayesian:
   - Neurons' firing rates vary, depending on the firing rates of input neurons, and rates are on continuums. This looks like implicitly updating probabilistic credences in response to probabilistic evidence.
   - Neurons have varying responsiveness to other neurons. This looks like implicit beliefs about conditional probabilities--about the strength of evidence offered by different inputs.
   - Through Hebbian learning, neurons' responsiveness to other neurons changes. This looks like updating one's implicit beliefs about conditional probabilities. The conditions that cause changed responsiveness (one neuron's firing preceding that of another more or less frequently) correspond to conditions in which it is likely to be appropriate to update one's conditional probability (if it is frequently appropriate to fire a neuron A shortly before firing a neuron B, then neuron A is likely a good indicator of when it is appropriate to fire neuron B).
   - [Some studies](https://www.lesswrong.com/posts/hN2aRnu798yas5b2k/a-crash-course-in-the-neuroscience-of-human-motivation#Expected_Utility_in_Neurons) suggest that neurons encode, not just subjective credences, but expected utilities
 - Humans have rough access to probability assignments in the form of degrees of confidence:
   - e.g. When I think about the idea that "it is July," I feel very confident in it. When I think about the idea that "all cats are secretly hamsters," I feel very skeptical of it (and amused, but that's less relevant).
   - These feelings of confidence update in response to evidence, in roughly the ways that one would expect a Bayesian who relies heavily on heuristics to update their credences:
     - e.g. Back when a bunch of evidence suggested that it was June, I did not feel confident in the idea that "it is July"
     - Availability bias as an example of updating one's credences with heavy reliance on heuristics
    - If these feelings aren't subjective credences that I usually track automatically (and consciously, when I put my slow, explicit thinking to the task), then what are they?
  - You might ask: if this is the case, then why doesn't a precise number come to mind when I consider P(burns mouth \| drinks tea)? Because our [automatic, intuitive systems of thinking that often track and update credences] are much older, in evolutionary terms, than [our conscious, explicit systems of thinking that can handle abstract quantities]. And evolution is a tinkerer, so we did not develop slow, explicitly symbolic thinking by completely rewiring our automatic thinking into using explicitly symbolic terms.
    - While I lack a precise, introspectively available probability, I can still say something like "between 1/100 and 1/2." Such broad ranges are often enough to have clear implications, such as when the stakes of one possibility are very high.

Neuroscience and introspection, then, suggest that humans do automatically track probabilities with subjective credences. These processes mean that humans following decision theory would not begin with infinite regress--we already have some beliefs about actions we can take and their likely consequences (as well as some preferences over outcomes), and these offer a starting point for decision.

Given that decision theory does not lead to infinite regress, claiming that it only constrains preferences, given some other preferences, seems to sell it short. Given beliefs and preferences, decision theory constrains actions--given a mapping from actions to probabilistic outcomes, and a preference order over probabilistic outcomes, there is a rational preference order over actions. If I believe that it will probably rain, and I do not want to get drenched, then it is a good idea (by my own lights) to pack an umbrella.

I find "maximize expected value" appealing as a way of making decisions under uncertainty for at least three reasons:
1. It offers a way to account for things I care about: the desirability of consequences, and their likelihood if I take some action
2. It is demonstrably best in the situations where it is most feasible to judge which strategy is best: If our credences match objective probabilities exactly, then expected value equals average value over many trials. So anyone seeking to maximize total value over many trials would do best by maximizing expected value at each trial. This would still pretty much be the case if our credences closely approximated objective probabilities. As a result, any strategy that deviates from "maximize expected value" will do predictably worse than "maximize expected value," at least in these circumstances.
   -. This is, admittedly, limited to situations that involve many trials. But that seems fine--it seems unwise to accept a general strategy that does not work well if used many times.
   - I don't know how to judge which strategy is best in other circumstance: when my subjective credences deviate significantly from objective probabilities. That seems like asking "what would be the case if I'm just terrible at figuring out what is the case?" If I'm terrible at figuring out what is the case, then how would I know?
3. I know of no other general approach to making decisions with these or similarly appealing qualities

I've argued that humans have credences, that rationality constrains actions, and that maximizing expected value seems best. Next, I'll argue that the weights we should use when making decisions should draw on more than just frequentist analysis, because there are other useful measures of reality, and there is empirical support for the relative accuracy of Bayesian forecasting. After that, I'll address a few loose ends.

> _One could tally all the times one has burned their mouth drinking tea, but that is collecting measurements and switching back to objective probabilities, which we agree are legitimate. Calling them "subjective credences" doesn't actually help us to decide anything._

Drawing on credences can help us make better decisions, because credences can be usefully informed by more than just datasets:
- We can sometimes make useful predictions on the basis of an event's causal dynamics. For example, consider a symmetrical 60-sided die. I have no data on how often such dies roll the number 60. But my understanding of how it works allows me to predict that the objective probability is 1/60. This is (I think you'll agree) useful and accurate, and I could not make this prediction if I saw frequentist data as the only useful evidence for probabilistic prediction-making.
  - A lot of the research that organizations like FHI do seems to be this: efforts to understand the causal dynamics of [events about which we lack data] to inform probabilistic predictions
- We can make inferences from somewhat-relevant reference classes (maybe frequentist analysis is fine with this?)
  - For example, one's forecast of the likely impact of advanced AI can be informed by data about the previous impacts of new technologies, transformative technologies, and expansions in cognitive abilities. Insofar as these are similar, frequencies are likely correlated, so accounting for these will bring one's subjective credence closer to the objective probability.
- Bayesian updating allows for a holistic combination of multiple, different sources of evidence into a better-informed credence. I don't see how frequentist analysis does.
  - This also allows for accounting for relevant arguments.
- What if one doesn't remember "all the times one has burned their mouth drinking tea"? If this were the case, and if it were also the case that one's automatic credence-formation had tracked those now-consiously-forgotten burnings, then one's subjective credence would be informed by a potentially much larger dataset than a probability formed through deliberate frequentist analysis
- If some prior credences are heritable, then evolution would probably select for evolutionarily useful priors, which would often be useful for human goals (e.g. high credence in "spiders are dangerous!"). Bayesian updating from one's priors can make use of this useful information, which is not explicitly available in datasets. Another way of thinking about this might be that, because they were naturally selected for usefulness over many generations, some prior beliefs are in accord with large data sets (e.g. how often spiders are dangerous).

Carefully formed subjective credences have several advantages over probabilities informed only by frequentist statistics--they account for a wide range of predictively useful considerations: causal dynamics, arguments, and datasets that are not explicitly accessible.

Do our subjective credences track these measures of reality well enough to be useful? It seems that way (especially when people are careful to mitigate the inappropriate application of heuristics):

As [Scott Alexander's review](https://web.archive.org/web/20200406135830/http://slatestarcodex.com/2016/02/04/book-review-superforecasting/) of Superforecasters discusses, Philip Tetlock's team of "superforecasters" probabilistically predicted future events (the details of which were unprecedented) with greater accuracy (closeness to objective probabilities) than chance, and with greater accuracy than CIA forecasters working with classified information. (And they didn't just get lucky--the same people tended to be superforecasters over multiple rounds of testing.) [Tetlock writes](https://web.archive.org/web/20200426202327/http://slatestarcodex.com/2016/02/07/list-of-passages-i-highlighted-in-my-copy-of-superforecasting/):

> _The superforecasters are a numerate bunch: many know about Bayes’ theorem and could deploy it if they felt it was worth the trouble. But they rarely crunch the numbers so explicitly. What matters far more to the superforecasters than Bayes’ theorem is Bayes’ core insight of gradually getting closer to the truth by constantly updating in proportion to the weight of the evidence. That’s true of Tim Minto [the top superforecaster]. He knows Bayes’ theorem, but he didn’t use it even once to make his hundreds of updated forecasts. And yet Minto appreciates the Bayesian spirit. “I think it is likely that I have a better intuitive grasp of Bayes’ theorem than most people,” he said, “even though if you asked me to write it down from memory I’d probably fail.” Minto is a Bayesian who does not use Bayes’ theorem. That paradoxical description applies to most superforecasters._

Assuming that Tetlock's claim is supported by the thousands of data points he collected, frequentist analysis seems to provide support for the usefulness of Bayesian analysis. More generally, this is frequentist evidence for the capacity of people to make better-than-random forecasts of events without information about previous trials of the events.

Tetlock found that several other factors [were correlated](https://aiimpacts.org/evidence-on-good-forecasting-practices-from-the-good-judgment-project/) with accuracy, including well-informedness, intelligence, deliberation time, belief updating, training on forecasting skills, team-based forecasting, and questioning one's initial intuitions. This looks pretty good for Toby Ord, and for thinking that such forecasts are far from probabilities "made up out of thin air."

Note that the predictions that Tetlock's forecasters made were unconditional probabilistic predictions. And the vast majority of forecasters [did better than chance](https://aiimpacts.org/evidence-on-good-forecasting-practices-from-the-good-judgment-project-an-accompanying-blog-post/) (not just the superforecasters, although they did especially better than chance). This is (frequentist) evidence against the claim that

> _there are no objective probabilities - no measurements from which to derive probabilities - when dealing with the unconditional future._

Other implications for Bayesian analysis:

You write that:

> _The probability calculus is so powerful because it can be used to learn about the world by abstracting and aggregating information from complex phenomena which are often too difficult to analyze by other means. But this always requires there to be a dataset - measurements of reality - behind these calculations. Without this, we are claiming knowledge where we don't have it and this is dangerous._

I agree, and I think that this is an important point. I would add that, as I have argued, extensive datasets of highly relevant reference classes are not the only useful measures of reality--logical arguments, information about causal dynamics, somewhat-relevant reference classes, and datasets that can only be accessed by considering our subjective credences also measure reality, and our subjective credences (more or less) successfully account for these. Our subjective credences are erroneous enough that I'm happy to act in accordance with solid frequentist data when we have it. When we don't, our subjective credences still offer useful measures of reality. Without these, we are acting as if we have ignorance where we don't have it, and this, too, is dangerous.

> _...we don't have a total order across explanations, so can't coherently talk about "second best", "third best", etc_

If explanations are particular claims about what the world is like, and if, as I have argued, we have partial credences in such claims, then we can coherently talk about second best explanations, and thus make use of them.

To address a few other points:

>_ There is a result in epistemology which proves that certain events are not knowable in principle - namely those events which are causally dependent on future knowledge, which we by definition don't have_
> _\[...\]_
> _It's important to recognize that this result only applies to unconditional historical predictions ("X will happen".) but not conditional ones (i.e. "If X happens, then Y will happen").  Relevant to our discussion, it also applies to probabilistic unconditional predictions ("X has a Y% chance of happening"), for to assign probabilities would require us to put a distribution over a set of events we do not know._

I like this argument--very neat result. Your last step here, going from ruling out definite predictions to ruling out probabilistic forecasts, doesn't make sense to me. We cannot predict all (or much) of how things will go in the future, but we are not completely clueless either--we can still make useful probabilistic forecasts, on the basis of aspects of the future about which we are not clueless.

> _One could try to get out of this by switching to a subjectivistist view probability, and rely instead on the “credences of experts”. But this is arbitrary. How do we select which experts to listen to? How can we ignore experts in theology...?_

I agree that using expert credences requires us to make choices. Why would it follow that these choices must be arbitrary? A few ways in which the choice of which experts to listen to may be made non-arbitrarily:

- Use frequentist data about experts. Tetlock [also](https://web.archive.org/web/20200406135830/http://slatestarcodex.com/2016/02/04/book-review-superforecasting/) provides evidence for the claim that experts who consider many angles / perspectives do better than chance at forecasting, while experts who "know one big thing" tend to do worse than chance. My limited knowledge of (especially Abrahamic) theology suggests that "knowing one big thing" is a decently accurate characterization of much of it.
 - Theologians predicting the end of the world also have a pretty terrible track record
- Use your holistically informed, subjective credences about the reliability of various kinds of experts. My subjective credences say that intellectual traditions which valorize faith will tend to produce predictions less correlated with objective probabilities.
   - Yes, this argument for subjective credences is circular. This is fine, because here I'm arguing, not that Bayesianism has external justification, but that it's coherent.

> _All we can ever do is try to criticize the best explanation through arguments and experiments, and try to come up with better ones._

And then how do you make decisions? I'm still confused about what the decision-making alternative to [something that's roughly expected-value-maximization] is.

### Update
_(Added a few days later)_

I came across some material that surprised me, so I want to add a correction to my response:

Reading a little more Tetlock, it looks like he makes a major caveat that I hadn't been aware of: “there is no evidence that geopolitical or economic forecasters can predict anything ten years out beyond the excruciatingly obvious… These limits on predictability are the predictable results of the butterfly dynamics of nonlinear systems. In my EPJ research, the accuracy of expert predictions declined toward chance five years out.”

While this finding is not directly about technological forecasts, it's suggestive that my previous optimism about them doesn't hold up at all. I'm not sure what to make of this. Maybe:

Expected-value maximization still makes sense, although now the best way of going about it for long-term predictions involves overriding one's automatic/intuitive formation of credences, and giving all non-negligible possibilities equal weight, except when one has very strong reasons to move away from equal weights.

Starting with a prior probability of 50% makes sense if one is completely clueless. Using the broadest reference class--all possible predictions--half of all possible predictions are correct, as for every possible prediction that is correct ("A will happen"), there is a possible prediction that is incorrect ("A will not happen"). (This feels sketchy.)

Given quite strong evidence, one should adjust one's estimate significantly (since Tetlock does grant that people can predict "the excruciatingly obvious"):
- If some categories of things that may happen are broader than others (e.g. "human extinction" vs "human extinction through nuclear war"), one can (and mathematically should) give greater weight to broader categories.
- Looking back to Ord's estimates: frequentist evidence is strong evidence for adjusting estimate of non-anthropogenic risks way down, while climate models + ancient history arguably make it obvious that, while climate change and nuclear war pose enormous risks, they do not significantly threaten human extinction.
- So this line of reasoning seems to generally support Ord's low estimates, while suggesting that his higher estimates (e.g. risks from AI) should have stayed even closer to the clueless prior of 50%
