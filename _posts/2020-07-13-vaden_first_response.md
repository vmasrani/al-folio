---
layout: post
title: Probabilities Without Measurements
author: Vaden Masrani
date: 2020-07-13
description: The second in a series.
comments: true
---

_The second in a series with Mauricio Baker on critical rationalism and bayesian epistemology. See [one]({% post_url 2020-07-11-mauricio_first_response %}), [two]({% post_url 2020-07-13-vaden_first_response %}), [three]({% post_url 2020-07-17-mauricio_second_response %}), [four]({% post_url 2020-07-22-vaden_second_response %}), [five]({% post_url 2020-08-06-mauricio_third_response %}), [six]({% post_url 2020-08-06-vaden_final_response %}), and [seven]({% post_url 2020-08-06-mauricio_final_response %})._

---

So I thought a good place to start would be to quickly summarize my concerns with how Bayesianism is being used in the Effective Altruism community, before responding to your points in detail. I think the simplest way to express my concern would be the following: I am extremely worried about the widespread use (within the EA community, but more generally) of _probabilities without measurements_. This seems to be a temptation unique to the Bayesian, who always has an extra move available to them - they can replace datasets with "beliefs", swap objective probabilities for subjective ones, and carry on with their analysis.
<!--more-->

The probability calculus is so powerful because it can be used to learn about the world by abstracting and aggregating information from complex phenomena which are often too difficult to analyze by other means. But this always requires there to be a dataset - measurements of reality - behind these calculations. Without this, we are claiming knowledge where we don't have it and this is dangerous.

There is a result in epistemology which proves that certain events are not knowable in principle - namely those events which are causally dependent on future knowledge, which we by definition don't have. The argument is contained in [The Poverty of Historicism](https://en.wikipedia.org/wiki/The_Poverty_of_Historicism) (I've summarized, but included the [longer quote]({{ "assets/pdf/poverty_historicism_quote.pdf" | absolute_url }}) for reference):

>*1. The course of human history is strongly influenced by the growth of human knowledge.*\\
>*2. We cannot predict, by rational or scientific methods, the future growth of our scientific knowledge. If there is such a thing as growing human knowledge, then we cannot anticipate today what we shall know only tomorrow.*\\
>*3. We cannot, therefore, predict the future course of human history.*

It's important to recognize that this result only applies to unconditional historical predictions (_X will happen_.) but not conditional ones (i.e. _If Y happens, then X will happen_).  Relevant to our discussion, it also applies to probabilistic unconditional predictions (_X has a Y% chance of happening_), for to assign probabilities would require us to put a distribution over a set of events we do not know. I take this to be a disproof of the possibility of using probabilities to predict the future of humanity, to the extent that these predictions are unconditional (_Existential catastrophe via unaligned artificial intelligence: 10%_.).

One could try to get out of this by switching to a subjectivistist view probability, and rely instead on the “credences of experts”. But this is arbitrary. How do we select which experts to listen to? How can we ignore experts in theology who study eschatology and also warn of the end of humanity? Because the probabilities are not constrained by datasets, in practice this means they are often made up out of thin air, and then euphemistically referred to as "credences" or "priors" and in some cases hidden behind a smokescreen of mathematics.

So when you say “In practice, people who don’t approach ethics quantitatively seem to consistently overlook immense injustice and suffering" I entirely agree, but only when the quantitative method can be applied. If it can't, but one seeks to apply it anyway, I think one is equally liable to make mistakes on questions of injustice and suffering because one is, in effect, applying sophisticated quantitative methods to made up numbers - numbers not derived from measurements.

The EA community is at its very best when it recognizes when it recognizes how easily humans err in their intention to help, with [William MacAskill's](http://www.williammacaskill.com/) [playpump](https://en.wikipedia.org/wiki/Roundabout_PlayPump) story being the obvious example. But I think it has a huge blindspot here. This, in short, is my concern with how Bayesianism is being used in the EA community. Now to respond to your points.

> _Vaden’s skepticism toward longtermism (which seems to motivate his skepticism toward doing the best we can--somewhat-informed guesswork--to go about making decisions as longtermists) rests on various errors: he misinterprets the implications of the “repugnant” conclusion; he wrongly thinks that, under longtermism, far-future concerns always dominate near-future concerns; and wrongly believes that future people do not exist._

I love the phrase "somewhat-informed guesswork", and I agree with you entirely later on when you write "Somewhat-informed guesswork is the best we can do to learn about the long-term consequences of our actions". I would just add, "and this somewhat-informed guesswork can only be improved with quantitative methods when the numbers are derived from measurements, lest we deceive ourselves for reasons outlined above".

With your permission, I'd like to simply concede I misunderstood the implications of the repugnant conclusion, and grant there are arguments about the existence of people in the future, because my main concerns don't really hinge this. If these feels like a dodge though, I'm happy to respond to some of your points in detail (but I'd rather not argue about the meaning of 'existence' if we can avoid it 🙂)

> _I’m skeptical of the claim that we can do anything other than make decisions on the basis of our subjective credences. It seems useful, accurate, and representative of decision-making more broadly to say that my subjective credence in the claim [it will rain tomorrow] has a big influence, together with my desires and other beliefs, on whether I pack an umbrella tomorrow. And it seems like it should. If the probabilities that end up influencing our decisions are always our subjective credences, then it’s pointless to say that we should be using something else--the best we can do is calibrate these credences as well as possible (which we can do by e.g. drawing on frequentist data when possible). We use our subjective credences to make decisions, and standard decision theory endorses this, so it seems useful to devote a significant amount of effort to making these credences closer to what’s optimal._

> _Similarly, there’s good reasons to think that any decision we make is at least implicitly assigning relative quantitative values (which Vaden seems skeptical of). As with assigning credences--since we can’t do anything else, it seems useful to figure out how we can best go about assigning relative quantitative values._

I think this is an important disagreement worth spending time on. It's relatively easy actually to show that decision theory cannot be used to describe how humans make decisions, nor should it be used to model an ideal rational agent, (i.e to disprove both the normative and descriptive claim).

This can be seen with an example. Let's use the maximum expected utility principle to decide what to drink tomorrow morning with breakfast. The process would be something like:

1. Decide on a set of actions (_drink coffee_, _drink tea_,..., ).
2. Decide on a set of consequences for each action (_stay up late_, _burn mouth_, ...)
3. Decide on a value for each conditional probability p(consequence \| action) for all valid consequence, action tuples
4. Decide on a functional form for the utility function (discrete? continuous? piecewise? smooth? convex? ...)
5. Decide on a utility function U(c) mapping each consequence to a real number
6. Then, choose action which results in maximum expected utility.

Thus, some _other_ decision making process must be used in steps 1-5, on pain of infinite regress. The chosen outcome in 6 is a deterministic mapping from the results of the numbers decided in 3-5 to the actions decided in step 1, and therefore the returned action is not determined not by the MEU principle in step 6, but by the other decision making process in steps 1-5. What ideal rational agent would use a decision making process which starts with an infinite regress?

Infinite regress isn't a problem when decision theory is used in machine learning, reinforcement learning, econometrics, etc, because the actual decisions are being made by human beings. The word "decision" in this case is just referring to a statistical procedure of learning from data, and is not the same as the (unknown) psychological/biological phenomenon called "decisions" in steps 1-5.

"Subjective credences" are often talked about as if they are just formed in your brain automatically and allow us to avoid having to make decisions (and thus avoiding the infinite regress problem). But this isn't true. Try it - try filling in a few entries of the conditional probability table in step 3 for example. What number are you going to write down for p(_burns mouth_ \| _drinks tea_) = c ? Or p(_has a productive day at work_ \| _drinks coffee_) = d? What are c and d? One could tally all the times one has burned their mouth drinking tea, but that is collecting measurements and switching back to objective probabilities, which we agree are legitimate. Calling them "subjective credences" doesn't actually help us to decide anything.

On the relationship between decision theory and rationality, here is a quote I like from the physicist David Wallace in his introduction to decision theory ([longer quote]({{ "assets/pdf/wallace_quote.pdf" | absolute_url }}) for context):


> _That is, the Dutch book argument is a constraint on rational preferences: it says that agents with certain preferences are rationally committed to having other preferences. And this is the basic structure of decision theory. It is not in general concerned with the rationality or otherwise of any single decision by an agent: if someone wants to jump into an alligator pit, we might deem them irrational but decision theory will not. But someone who prefers jumping into alligator pits to lying on the beach, and prefers lying on the beach to jumping into snake pits, is constrained to prefer alligator pits to snake pits._
>
> \- _David Wallace, The Emergent Multiverse: Quantum Theory According to the Everett Interpretation_

So I return the charge of pointlessness - it’s pointless to say that we should be using decision theory when it cannot describe human decision making without collapsing to infinite regress, and only offers normative advice to a very narrow bandwidth of rationality anyway (i.e. constraining certain preferences given other preferences).

> _Rejecting probabilistic assessments of far future trajectories, Vaden argues that “the best explanation is all we have” (1:15:20). This is a big mistake. We also have the 2nd-best explanation, and the 3rd-best explanation, and so on. I’m not just saying this to nitpick. If the 2nd best explanation / set of arguments implies “we’re in significant danger, and we can do something about it,” ignoring it seems reckless. Expected value calculus based on subjective credences offer a way to account for things like 2nd-best explanations that would be important if true. I don’t see how Vaden’s proposed approach allows for such reasonable-seeming caution._

Explanations are discrete things - separated by bad explanations - and we don't get a better explanation by taking the weighted average across all explanations, as the expected value calculus would require. If we could, we would just average out quantum mechanics and general relativity, for example, and be done with it (And we don't have a total order across explanations, so can't coherently talk about "second best", "third best", etc.) All we can ever do is try to criticize the best explanation through arguments and experiments, and try to come up with better ones.

> _Vaden argues that ideas are the primary causes of existential risks. I’d be very curious to hear more about how ideas might pose x-risks, and how they might be positively shaped for the long-term future. But his claim that they’re primary causes seems unsubstantiated as a general claim and not very helpful in specific cases. For example, when it comes to risks of engineered pandemics--sure, these wouldn’t happen if no one thought that engineering a pandemic was a good idea, but restricting DNA synthesis might be a more tractable solution than reducing misanthropy._

Well I argued that, at least so far, the events in history which have brought us closest to extinction have been born through a conflict of differing ideas. And therefore it seems reasonable to assume the future will be the same. All I really meant by this is that while it's very important to catalog nuclear near-misses and bioweapon laboratory escapes for instance to reduce the possibilities of accidents in the future, the existential risks we will face in the future are ultimately unknowable, at least to the extent that predicting new ideas in the future is impossible.

I didn't make this claim with the intention of coming up with something helpful in the specific case, I think it does in fact contain some helpful suggestions. One would be that if we want to prevent extinction, we should focus on strengthening those institutions that allow for peaceful resolutions of conflicting ideals. I'm thinking here of (for instance) first past the post voting systems instead of proportional representation (counterintuitive yes, [here's](2018-11-14-prop_rep.md) an argument), improvements to social media platforms that  incentivize tribalism and division, protection of institutions which foster debate, and so on. If the [Future of Humanity Institute](https://www.fhi.ox.ac.uk/) dedicated itself to coming up with societal mechanisms to prevent conflicting ideas from becoming violent, I think it would go much further to achieve its goals.

> _Vaden also claims that measuring subjective credence doesn’t measure anything very important--that it’s detached from the objective probabilities that we actually want to know. If subjective credences are formed in such ways that they’re correlated with objective probabilities, then this claim is false._

Well, yes. But there are no objective probabilities - no measurements from which to derive probabilities - when dealing with the unconditional future. So what could they possibly be correlated with?
