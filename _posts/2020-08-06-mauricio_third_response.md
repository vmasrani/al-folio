---
layout: post
title: Maximum Expected Utility as a Normative Ideal
author: Mauricio Baker
date: 2020-08-05
description: The fifth in a series.
comments: true
---

_The fifth in a series with Mauricio Baker on critical rationalism and bayesian epistemology. See [one]({% post_url 2020-07-11-mauricio_first_response %}), [two]({% post_url 2020-07-13-vaden_first_response %}), [three]({% post_url 2020-07-17-mauricio_second_response %}), [four]({% post_url 2020-07-22-vaden_second_response %}), [five]({% post_url 2020-08-06-mauricio_third_response %}), [six]({% post_url 2020-08-06-vaden_final_response %}), and [seven]({% post_url 2020-08-06-mauricio_final_response %})._

---

Thanks for your thoughts! I think we agree on at least this:
- Collecting information, learning more, and engaging in argument (especially seeking serious criticisms of one’s own positions) is very important. Deference to others’ beliefs should not substitute this process.

And you’ve convinced me on at least two points:
- There are good ways of thinking about decision making other than thinking in terms of MEU
- CR is a great way of thinking about decision making
  - Often, at least, it’s better as an explicit approach than explicit MEU

Still, I want to insist on two claims over which we seem to have interesting disagreement:
- MEU is a normative ideal for decision making—choices (including choices made using CR) are good insofar as they are close to this ideal, and bad insofar as they deviate from it.
  - In practice, we will make better decisions if we keep MEU in mind as an ideal.
  - Ord’s claim is legitimate.
- Human decision making is in fact a rough approximation of ideal MEU

### MEU as Universally Ideal

> _Expected value calculus can be viewed as a critique, and as such, is entirely valid in some circumstances - namely when utilities, actions, and consequences are clearly defined, and we have the opportunity to repeat many trials._

We seem to agree that MEU is sometimes best. I’ll argue for a stronger claim: that it’s always best.

> _[...] consider the classic coin flip. In this instance, we have a clearly defined notion of objective probability - it's a property of the coin, and can be measured through experimental trials. It therefore makes sense to talk about aligning one's subjective probability with objective probabilities here, because there are in fact objective probabilities to align against._
>
> _But unless you want to invoke Everettian many worlds, we only have a single future. There either will, or will not be, a war between North and South Korea in the next ten years killing > 1000 people. The next ten years will only happen once. What is the objective probability of a single event? It's undefined. Why? Because there is nothing to measure [...]_
>
> _[...]_
>
> _What are we actually learning here? That when Scott says he's X% confident about something, he's right X% of the time (probably). Good. We can trust Scott when he says he's confident about something. But how is this evidence against the claim that there are no objective probabilities when dealing with the singular, unmeasurable future? The objective probabilities in this case just come from all the other times Scott has said he is X% confident about stuff, and don't refer to the future at all._

Good point—my wording was inaccurate, and war between the Koreas does not have an objective probability in the sense that a coin flip has an objective probability.

My revised claim is this: while credences don't correlate with straightforward objective probabilities for single events, they do generally correlate with [things in proportion to which one should weigh outcome values when aggregating them], which MEU does. This makes MEU an ideal in general, not just for decisions that seem to be clearly defined and have many trials.

There’s two lines of argument I want to make here. I’ll start with the one that’s less weird.

1. Even if there are no objective probabilities to which credences can correlate, there’s still something useful—whether something will or won’t happen (which we can quantify as 1 or 0)—that credences can correlate with. The low Brier scores of superforecasters indicate that their credences have this correlation, since these scores are calculated using the differences between probabilistic forecasts, and the 0s and 1s representing whether single events happened.
2. Why is it useful to weigh outcome values in proportion to credences that have this correlation? Because it's useful to more often bet on things that do happen, and not on things that don't happen (by "bet on x," I mean, roughly: acting in a way that will have a good outcome if x happens, and a bad outcome otherwise, at least relative to the outcome that some other action would have). Since good forecasters' credences correlate with whether some event happens, it's useful to more often bet on things that good forecasters assign high credences to. MEU lets us do this, making it valuable even when dealing with events that simply do or do not happen.
- a) An example of using this: I'm still waiting to hear back from school about whether students will be invited back to campus in the fall. Since I assign a not-very-low credence to either event, it makes sense to avoid actions that would be very costly if one outcome happens, and not very valuable otherwise, such as buying non-refundable plane tickets early.
- b) Even if only one outcome will happen, I will face many similar decisions in my life, and over a lifetime I will tend to make choices with worse outcomes if I don't follow the above approach.

I think this argument mostly works, but it’s not totally solid—the notion of “tend to” in (2b) alludes to some notion of probability. As you troublingly point out, this kind of thing is problematically circular—this argument was supposed to argue for something like probability for things that either will or won’t happen, but it relies on something like probability for whether my decisions over my lifetime go well—something that either will or won’t happen.

One potential response to the criticism of circularity is to revise my claim in (2b), to the following: Consider two groups of people: people whose willingness to make bets is strongly correlated with whether the bets pay off, and people for whom this correlation is weaker. As the number of choices made by people in each group increases, the average value of the outcomes of the choices made by people in the former group will approach a higher value than that of people in the latter group.

But what could I respond to someone who hears this argument, and doesn’t mind being in the latter group?

I’d have to go to the following, other argument. This is similar to invoking Everettian many worlds, except it’s less controversial as a claim about physics/astronomy, and it gives a role to more types of uncertainty than quantum uncertainty.

1. One should act in a way that accounts for how one’s action is correlated with others' actions. For example, If I know that I'm playing a prisoners' dilemma against a perfect simulation of myself, I will do better if I cooperate, even if I’m totally self-interested.
- I find two arguments for this compelling:
  - If one values how good the universe is, not just how good one personally makes it, then accounting for these correlated outcomes is accounting for things highly relevant to what one values.
  - When I’m making a decision, it’s intuitive to identify with myself—in a sense tied to some particular time and place—making the decision. But if I’m thinking of myself as a decision maker, it’s more relevant to think of myself as a decision-making algorithm, wherever this algorithm is implemented. [Brian Tomasik](https://reducing-suffering.org/anthropics-without-reference-classes/#Update_Feb_2015_You_are_all_your_copies) argues for this in a way I find compelling.
    - I think we agree that subjective experience is the implementation of some algorithms. This makes identifying as an algorithm more plausible.
2. Every decision we make is highly correlated with vast numbers of other decisions—perhaps infinitely many. Many of these other decisions are made in situations different enough that a decision algorithm’s outcomes in some implementations will be different than outcomes of some other implementations.
   - Our universe is spatially infinite[^1], or at least absurdly vast. As a result, when I make some decision, there are vast numbers of actors (perhaps infinite actors) in situations extremely similar to mine: they have just about the same information, values, and cognitive capacities as me—similar enough that we will make the same choice (that is, we’re all implementing the same decision-making algorithm. Alternatively, if I identify as a decision-making algorithm, then I’d describe this as: I am being implemented in all of these people).
   - We are also all ignorant of many things—it may be the case, for example, that half of us (measured by average density over space) are in situations where investing in Seoul will have great outcomes, and half of us are in situations where it will have bad outcomes, but the differences in our situations that will lead to these different outcomes have escaped our notice. Because of this, our decision-making algorithms remain highly correlated, while being instantiated in situations where identical choices will have different outcomes.
3. Whether our choices are highly correlated with infinitely many other choices or merely with a vast number of them, there are good reasons—if we accept (1)—for thinking that the best thing to do is always to maximize an average value of our choices: the sum of the values of different outcomes that a choice will have in different impelemtations, each weighted by the relative frequency of the outcome.
   - If our choices are highly correlated with an infinite number of choices, and we value the outcomes of choices that are highly correlated with our own, then any choice—if we consider its outcomes, aggregated over wherever the choice is made—results in infinite good outcomes and infinite bad outcomes. So the total value of any choice, traditionally conceived, is undefined[^2]. This problem does not seem unique to MEU. Under CR, if we seek arguments for _why each action will lead to desirable consequences_, these considerations imply that any action will lead to infinite desirable as well as infinite undesirable consequences. One way to get out of this is to change what one tries to maximize—maximize, not total value, but the average density of value over space and time[^3]. This approach has its issues, but other approaches to infinite ethics seem to have worse problems. For some decision-making algorithm to maximize value density according to its utility function[^4], it must make the choice that, over the infinite actors who implement the choice, has the highest average value. Anything else, over infinite trials, will lead to a lower overall value (a lower value density). The average value of a choice made in such a universe is the sum of the value of each outcome that it sometimes has, weighted by its relative frequency[^5].
   - Alternatively, suppose that, for whatever reason, you favor forgetting about infinity and the many headaches it can bring. Then my decision-making algorithm is merely being implemented by a vast number of actors. If we accept this, we can stick with a traditional notion of wanting to maximize total value. As the number of actors implementing our decision-making algorithm increases, it becomes arbitrarily close to certain that the choice with the highest total value will be the one that has the highest average value. Similarly to the previous case, average value is the sum of all of the values of a choice’s outcomes, weighted by their frequencies—choosing the highest average value is (nearly) equivalent to choosing the highest total value.
     - I find this pretty compelling, although you might reject the relevance to decision making of being “arbitrarily close to certain” that some decision is best, if this tracks no objective frequencies. In that case, my argument for MEU rests on (3a), above.

To summarize and extend these arguments:

Maximizing the average value of a choice over vast numbers of trials is nearly certain to maximize total value—or certain, if there are infinite trials and we replace total value with value density. Caring about correlated choices in a vast/infinite universe gives us many trials that we are concerned with. Different outcomes for different implementations of the same decision-making algorithm give a relevant meaning to the "average value of a choice." So, assuming that we want to maximize total value, in each world we must maximize the average value that our choice will have, when it is done by every actor who implements the same decision algorithm. To find this average value of a choice (assuming that we value outcomes), we must weigh [the value of each outcome that the choice will have in some situations] by the relative frequency of situations in which the choice will have that outcome. So there is an extremely decision-relevant sense in which we can—and, given my assumptions, should—talk about and account for the probabilities/weights of outcomes that, in each situation, either will or will not happen.

This means that, even for events that appear to be single events, there _is_ something to count, something to measure! We as decision-making algorithms can (more or less well) count the relative frequencies of outcomes in all the situations where we are implemented.

For example, suppose I am completely clueless about whether a choice will have some outcome or not. Using the broadest reference class—all outcomes—half of all outcomes happen, as for every possible outcome (“A”), there is an outcome that does not happen ("the absence of A"). So—to the best of my ability to count them[^6]—whenever I as a decision-making algorithm implement a decision amidst total cluelessness regarding some outcome, the outcome will occur half of the time. Since (if you accept my arguments), I want to pick the choice that will have the highest value on average, I should only pick the choice in question if its expected value—calculated by starting with the value of outcome A and the value of outcome not-A, weighing them equally, and then adding them—is higher than the expected value of other options. Over vast numbers of implementations of this decision algorithm, actors will take every bet that pays off, on average, if a desired outcome happens half of the time. They will also refuse every bet that is a loss, on average, if a desired outcome happens half of the time. Desired outcomes will happen half of the time, so this is the optimal outcome for total value—any deviation from this decision algorithm would lead to lower total value.

So this decision algorithm achieved ideal outcomes across the universe by acting consistently with MEU, and it would have done worse if it had chosen any other way. It successfully quantified the unknown and acted on it, and it was able to do this in part because its uncertainty measured something useful: the relative frequencies, across the universe, of outcomes over which it is clueless.

(Such clueless/indifferent priors seem useful for forecasting events that depend on future knowledge.)

A similar logic works for outcomes that occur with frequencies that are not necessarily 50%, such as the outcomes forecasted by a forecaster whose forecasts have been shown to correlate with frequencies. (By the way, Tetlock does emphasize the 2% of people who have especially strong correlations between forecasts and how often things happen, but he found that probabilistic forecasts generally tend to have some positive correlation. So it’s not the case that _this information is only accurate for a select “super” few of us anyway_. (And even if this was the case, we could just listen to these people for deciding important matters.))

This is an argument against the claim that, if good forecasters state their credences,

_We have learned nothing from this exchange, because arbitrary numbers representing beliefs - numbers uninformed by simulations or counts - have been offered in place of arguments._

On the contrary, the credences of good forecasters are informed by decision-relevant counts. We learn something from them. We can and should act on them: update our own credences and make later choices accordingly.

I want to emphasize that this process I argue for, of sharing and updating credences, should encapsulate—not replace—critical argument. In practice, the choice that maximizes expected utility choice is often learning more—making more observations, engaging in argument—because we can often unlock higher average values for some choice by putting it on hold and learning more about the particulars of our situations (e.g. “Am I in a situation where this argument for the choice that currently seems best holds up to scrutiny?”). In terms of my earlier argument, we can think of learning more as breaking up one group of highly correlated decision makers into multiple smaller groups, each of which can now make choices better tailored to their situations.

For example, suppose many actors, who are ignorant about whether some test will confirm that they have an illness, are implementing the same algorithm: deciding whether to self-quarantine. As they are implementing the same algorithm, there is no way—other than astronomical luck—for them to at this point choose whether or not to quarantine without leaving some actors significantly worse off. Suppose they choose neither of those options, and instead choose to learn more by getting tested. Then, we no longer have a single decision algorithm, but two: one with the input that its actors received a positive test result, and another with the input that its actors received a negative test result. Having been differentiated by the particulars of where they are implemented, these algorithms have new access to choices with higher average (and thus total) values. So learning more has an important place within MEU, even under my perhaps-odd arguments for it.

Looking back on this, these aren’t straightforwardly arguments for weighing outcome values by our subjective credences before adding them. More straightforwardly, they’re arguments that it’s optimal to weigh outcome values by _something_, even when we seem to be dealing with single events. This _something_ corresponds with things that Bayesian epistemologists pay attention to—indifferent priors amidst cluelessness, well-calibrated probability assignments—important things that CR applied with heavy skepticism toward Bayesian epistemology will overlook. Since these weights are actual counts, actual frequencies, it’s legitimate and useful to apply statistical methods like Bayes’ Theorem to them.

> _First, [CR] satisfies your request for a general approach to making decisions with these or similarly appealing qualities, because [CR] entirely subsumes [MEU]._
>
> _[...]_
>
> _Creating a set of sentences/actions and criticizing them by simulating possible counter arguments is what operations I'm consciously and constantly performing when deciding what to write. Not computing utilities multiplied by probabilities and then mentally summing them up._
>
> _[...]_
>
>_"getting closer to the truth by constantly updating in proportion to the weight of the evidence" actually just means "constantly correcting errors by criticizing your ideas about future events”_

I think we have a large amount of agreement on what decision making should look like in practice. This process of criticizing options through argument (broadly conceived) looks a lot like what I'd label heuristically calculating expected utilities.

I want to claim that MEU entirely encapsulates CR, because every action that CR might value—creatively generating options[^7], engaging in critical argument—is an option that may have high expected value. My words seem to echo your claim that CR subsumes MEU[^8]. I doubt there’s an interesting disagreement to be had over “which one really subsumes the other?” I’m happy to mostly accept CR as an explicit approach to decision making. Where I think we disagree is in my claim that, even if we use CR, making decisions in accordance with MEU is ideal, and this makes it useful to sometimes explicitly weigh outcome values by something like subjective credences, and to examine what values or credences our choices imply.

To elaborate on that last point:

As with any claim, we can usefully evaluate the claim that some choice is best by assuming that it's true, and then assessing how accurate its implications are. Since the best choices maximize EU, the claim that some choice is best implies that it maximizes EU, and this (given some utility function) implies credences / assignments of probability. In this sense, any choice implies credences. Alternatively, we can take our credences as givens and examine what our choice implies about our utility function / value assignments. In this sense, any choice implies assignments of value. Considering this can be useful because it can help one realize that some choice wouldn't actually maximize EU—assuming it's the best choice may imply weights or values that one doesn't endorse.

### Humans as MEU Approximators

> > _If these feelings aren't subjective credences that I usually track automatically (and consciously, when I put my slow, explicit thinking to the task), then what are they?_
>
> _Well they're just that, feelings. Who is to say they have numbers that sum to one attached to each? Dutch Book-style arguments about rational betting are no use here, because they always begin "If an agent is rational in a particular way, then ...". But we know humans aren't rational (cognitive biases, kahneman and tversky and all that), and therefore dutchbook arguments don’t apply to humans but to idealized rational agents who only exist in our imagination._

I’m not convinced by this. You raise the quote:

> _"During the course of a creative process, one is not struggling to distinguish between countless different explanations of nearly equal merit; typically, one is struggling to create even one good explanation."_

Well, we observe that these feelings of confidence about various things respond to evidence in the ways that we'd expect Bayesian credences to update (with additional baggage from evolution, e.g. heuristics that cut computation costs and biases that are advantageous in social interactions). In other words, we observe that these feelings look like a component of decision-making that we'd expect to find, if we evolved decision-making in a universe where approximating MEU with Bayesian belief updating works best.

With Bayesian epistemology, we have a good explanation for this observation: it's what it looks like—Bayesian belief formation, which evolved because that kind of belief formation is generally useful and therefore adaptive. For all organisms that make interesting choices, it’s adaptive to take bets that tend to pay off (in genetic terms). This seems even more plausible if we accept, as we do, that human brains are at least roughly Bayesian at the neuronal level. Do we have any other good explanation of why we have feelings that look Bayesian?

> _Who is to say they have numbers that sum to one attached to each? Dutch Book-style arguments about rational betting are no use here, because they always begin "If an agent is rational in a particular way, then ..."._

Feelings of confidence about claims, which are the feelings I have in mind when I talk about subjective credences, have no obvious numbers attached. But they do seem to clearly exist along a spectrum from "completely skeptical" to "completely confident." Not only are feelings of confidence ordered by differences in extent of confidence, these differences also seem to have magnitudes associated with them—upon reflection, I may feel a little more confident in claim A than in claim B, and much more confident in claim C than in claim A. This isn't quite a proof, but it seems highly suggestive that, implicitly, these feelings have numbers attached. And if you're using probabilities as MEU weights, they don't need to sum to 1—it's the ratios that matter (although a weight as a proportion of all weights must be greater than 0, because negative weights don't make sense, and it must be less than 1, because a part can't be bigger than the whole which contains it)

> _[...] dutchbook arguments don’t apply to humans but to idealized rational agents who only exist in our imagination._

Fair, but there are other reasons for thinking that approximations of these ideal agents exist outside our imagination. Approximations of these ideals may also exist as what evolution has selected for in brains, if actors that are these approximations tend to do better at maximizing evolutionary value. Evolution's optimizing pressure means that some actual things have been selected for closely approximating some ideals, so it's at least very plausible that idealized rational agents in our imagination are approximated by actual agents—ourselves.

> _The MEU approach to human decision making would suggest [...]_
> _Compute the expected utility for each action. I just want to highlight here that this is an incredibly non-trivial task in practice._

Is it much harder than other neat cognitive tricks that billions of years of evolution have pulled? I know very little about this.

### Loose Ends

> _Also I’m not sure what “frequentist data” is. [...] I suspect you’re using the term “frequentist data” to contrast it against other useful kinds of information about the world that aren’t derived from measurements_

Oops—yeah, I roughly meant that: the kind of data from which one could easily conclude the objective probability of something.

> _So I really want to pin you down here. When you say_
>
> _[...]_
>
> _I can't tell if you agree that this move is illegitimate or not._

My bad for not being very clear. As argued, I think your move would be legitimate, as is Ord's. The version of my quoted vague claim that I want to make now is "when a credence is formed with little information, it's best to only update a little on its basis, and—especially if the credence is highly relevant for an important decision—it's very valuable to look for more information."

> _So, uhhh, how did we get here again? [...] I ain't no frequentist!_

Ah, my bad.

> _Additionally, CR offers alternative suggestions when faced with a decision that MEU doesn't. [...] The MEU strategy [...] entirely neglects the most important aspect of decision making - namely the creation of new options._

MEU doesn’t need to neglect this. Under (approximations of) MEU, we can always have "creatively generate new options" as an option. You argue compellingly that this is high expected value, especially for important decisions before one has hit seriously diminishing returns to generating new options. I grant that explicit CR does better than explicit MEU at helping decision makers remember this option and its importance, but this does not mean that MEU is not an ideal for all decisions. Given experiences most people have had, it’s rational to assign a high expected value to generating new options, so failing to do this is failing to MEU. Because of this, when we argue that it’s bad to neglect the generation of new options, we’re arguing that people will make worse decisions if they fail to MEU—this is an argument for MEU being ideal, not against it.

> _And in any case, the frequency interpretation, whether with an infinite or a finite number of instances, logically doesn’t reproduce probabilities unless the instances are equally likely, which gives a circular definition of ‘likely’._

I claim to get out of this by using weights based on the proportion of actors implementing a decision algorithm for whom some outcome will happen. I do assume equal weights, but this comes from an egalitarian intuition—that I value people in different parts of the universe equally—not from a premise about probability. Circularity avoided!

> _I was hoping you might be able to hear just how weird it sounds to have a rationalist and presumed atheist argue so strongly in favour of belief._

Is it that weird? There seems to be an important difference between faith and belief: how hard one tries to form correct beliefs. And in my experience, people who buy Bayesian epistemology are big fans of becoming less wrong.

Even when we engage in critical argument, in some process of criticizing positions and arguments, at the end of the day we're still going with our feeling of confidence—with which position feels like it's most resilient to criticism. We don't have access to [knowledge of which arguments are most defensible] that's somehow independent from our feelings of confidence in various claims. CR doesn't emphasize this, but it doesn't get out of it either. Making decisions on the basis of critical arguments requires beliefs about the latter.

>_Everyone has different beliefs about which experts are reliable, and then tend to collect data to support these beliefs. This is the cause of the problem, not a solution to it._

I think we agree that people often make these choices arbitrarily and seek to confirm their beliefs. That doesn't mean these choices are necessarily arbitrary (e.g. I read that Tetlock article to learn about forecasting, not to get dirt on theologians). And this problem is hardly unique to valuing expert beliefs—for any kind of argument/evidence we might value, people will tend to seek ways of using it that confirm their pre-existing beliefs.

> _“Hence for the purposes of Arrow’s theorem each piece of evidence can be regarded as an ‘individual’ participating in the decision-making process, where the person as a whole would be the ‘group’._
>
> _Now, the process that adjudicates between the different explanations would have to satisfy certain constraints if it were to be rational. For instance, if, having decided that one option was the best, the person received further evidence that gave additional weight to that option, then the person’s overall preference would still have to be for that option – and so on. Arrow’s theorem says that those requirements are inconsistent with each other, and so seems to imply that all decision-making – all thinking – must be irrational. Unless, perhaps, one of the internal agents is a dictator, empowered to override the combined opinions of all the other agents. But this is an infinite regress: how does the ‘dictator’ itself choose between rival explanations about which other agents it would be best to override?”_

I’m not sure I understand how this is a new disproof of (approximate) MEU as human decision-making. This seems like a rehashing of the earlier infinite regress argument—if we assume that to make any decision, one must first make another, we get infinite regress. This seems to be a result of Deutsch’s assumption, not of mine. Don’t we agree that evolutionary arguments are a way out of the infinite regress problem?

I agree with many of the other points you make.

Oh, and I noticed that your list of book recommendations has a bunch I haven’t read from authors you’ve mentioned (Popper, Deutsch). Do you happen to have one or a few in particular that you’d recommend?

---

[^1]: Tegmark, [“Parallel Universes,”](https://space.mit.edu/home/tegmark/multiverse.pdf) pp. 1-4
[^2]: My ideas about this come mostly from Bostrom’s paper [“Infinite Ethics”](https://www.nickbostrom.com/ethics/infinite.pdf)
[^3]: This can be defined as follows: pick any point in space and space. Consider the value in a sphere of some radius centered around that point, divided by the volume of the sphere. Value density is the limit of this quantity as the radius, over space and time, increases to infinity. It’s normally good enough to just say “maximize total value,” because doing so over a limited, finite scale maximizes value density. One concern I have with this approach is that the resulting sphere may be dominated by the universe in heat death, which could imply that all universes have a value density of 0. One way to get out of that is to not count portions of the universe that are in states of heat death. Another way this problem could be avoided would be if it’s the case that, even considering heat death, the value density of the universe is not 0 (perhaps because entropy tends to increase, but not always, so if you give the universe enough time it’ll eventually re-organize into interesting things. Value density would not be 0 if the time that this takes does not increase between every ordered era of the universe.).
[^4]: It might seem circular to argue for MEU by assuming that we can judge actions by utility functions. Making this worse, two of the assumptions required for some actor to have a utility function rely on notions of probability. Still, I think the arguments I make here are salvageable. My arguments for the use of weights beyond objective probabilities require utility functions. Utility functions require actors to have certain kinds of preferences involving some type of probability. But utility functions don’t require assuming that actors maximize expected value, nor do they require the kinds of weights that I argue for. Circularity avoided!
[^5]: Similarly to computations of other values in an infinite universe, it seems best to compute these proportions by counting relative frequencies in an ever-expanding bubble—see footnote 3.
[^6]: One might be able to count in other ways and get different results, but they seem so contrived that I’m more reluctant to trust them.
[^7]: More on how MEU encapsulates this is in the “Loose Ends” section
[^8]: I think your move here was legit. Earlier, I thought you disagreed with my claim that MEU is optimal in at least some situations, so I was initially confused at seeing a proposed alternative that subsumes MEU for some situations.
