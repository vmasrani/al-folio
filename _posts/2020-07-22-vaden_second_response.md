---
layout: post
title: Critical Rationalism and Bayesian Epistemology
author: Vaden Masrani
date: 2020-07-22
description: The fourth in a series.
comments: true
---

_The fourth in a series with Mauricio Baker on critical rationalism and bayesian epistemology. See [one]({% post_url 2020-07-11-mauricio_first_response %}), [two]({% post_url 2020-07-13-vaden_first_response %}), [three]({% post_url 2020-07-17-mauricio_second_response %}), [four]({% post_url 2020-07-22-vaden_second_response %}), [five]({% post_url 2020-08-06-mauricio_third_response %}), [six]({% post_url 2020-08-06-vaden_final_response %}), and [seven]({% post_url 2020-08-06-mauricio_final_response %})._

---

Really excellent stuff! I'll focus on what I read to be the major themes in your response and reply to those rather than going point-by-point. The themes I'll address are:

- Humans, computers, and infinite regress
- What other options to decision theory are there?
- The usefulness of bayesian analysis
- The Bayesian vs Frequentist dichotomy
- Superforecasters demonstrating subjective probabilities can track objective ones
- Loose end

### Humans and computers and infinite regress

> _I understood your argument here as being the following. Please let me know if I misunderstood or am interpreting uncharitably._
>
> _Humans do not (and should not) use expected-utility-maximization (of the sort in which consequences are weighted by subjective credences), because attempting to do so requires first making decisions about one's options, probabilistic predictions, and utility functions. This amounts to beginning with infinite regress, which is not a great way to make decisions. Computers that maximize expected value avoid this problem by having humans make these initial decisions, and then updating their probabilities by using data according to programmed rules. If humans worked like this, then we could follow decision theory without falling into infinite regress. However, humans don't work like this--our inability to introspect on precise, numerical subjective credences is strong evidence for the claim that we do not automatically calculate subjective credences. Even if we formed subjective credences by (consciously?) examining data, we would just be following frequentist statistics, and this would not support the claim that Bayesian statistics offer further value._
>
> _​My current impression is that humans do work roughly like the computers you mention, in that we are born with (or otherwise develop, without choosing) at least a few assignments of value, credences, and ways of updating our credences based on data._
>
> _Could you say more about why you think this is not the case?_

So first, great summary! To clarify a few points, yes, totally agree that humans work like computers - there is nothing supernatural about the brain, and anything that the brain can compute can also (in principle) be done by computers and vice versa. It's the hardware vs software distinction which is what is important here. Humans are born with innate software which we don't understand. I view understanding and reinstantiating this software on different hardware as the goal of artificial intelligence research.

So to say a little more about what I think isn't the case - the only thing I can say confidently is that the brain can't _only_ be running the MEU software to make decisions because of the infinite regress problem - there must be some additional decision-making software running.

You suggest evolution could be the thing that offers the starting point for decision making, by providing us at birth with certain inherited prior probability distributions (and presumably a finite repertoire of utility functions as well, plus software to rapidly calculate the high dimensional integrals required to compute posterior distributions and expectations). Reasonable enough hypothesis, and totally agree that if this is true it would stop the infinite regress.

But then it's not exactly accurate to say

> _Given that decision theory does not lead to infinite regress..._

but rather

> _Given that decision theory, plus additional auxiliary evolutionary hypotheses, which themselves imply additional software, does not lead to infinite regress...._

And while there are enough other problems with the philosophy of probability to make me skeptical that this is in fact true (to this subject I shall return), I don't hope to disprove the “MEU as an explanatory theory of human decision making” thesis here - although, *cough*, if you did want to find such a disproof using [Arrow's theorem](https://en.wikipedia.org/wiki/Arrow%27s_impossibility_theorem), I've attached a quote at the bottom[^1] (which you have no obligation to reply to, just including it because I found it interesting). So let's conclude the digression on infinite regress by us agreeing that evolutionary arguments are a way out of the infinite regress problem.

### What other options to decision theory are there?
... but only because I want to spend more time on your request for alternatives. The infinite regress problem with the "pure" MEU hypothesis should at the very least motivate an interest in exploring alternative approaches. After all, there is nothing in the laws of physics that says macroscopic decision-making agents must make decisions probabilistically. There are [all sorts](https://en.wikipedia.org/wiki/Action_selection) of alternatives to MEU, with a classic example being Deep Blue who beat Kasparov using an entirely deterministic decision making algorithm.

The one I have in mind comes from the philosophical school of [critical rationalism](https://en.wikipedia.org/wiki/Critical_rationalism) (hereafter referred to as CR). In short, it consists of making decisions by _creating new options and criticizing them_. I'll use Deutsch's terminology of _creativity_ here as a placeholder word for "whatever unknown software the brain is running to get out of the infinite regress problem."

The MEU approach to human decision making would suggest:

1. Creatively generate a set of actions, consequences, a utility function, and all requisite conditional probabilities.
2. Compute the expected utility for each action. I just want to highlight here that this is an _incredibly_ non-trivial task in practice. [This textbook](https://link.springer.com/book/10.1007/0-387-71599-1) is worth scanning to get a sense of the various difficulties associated with computing posterior distributions. My main area of research is in improving these methods as it happens, so I say this as someone who is actively working to make this process easier.
3. Choose the action with the maximum expected utility.

The CR approach to human decision making would instead suggest:

1. Creatively generate a set of actions. For each, creatively generate arguments as to why each action will lead to desirable consequences. Note this is analogous to the "mutation" stage in evolution, except applied to ideas instead of genes.
2. Subject each action to as much (creative) criticism as possible, both from yourself and others. There is no constraint on the particular form the criticism must take, provided it's derived by rational means (hence the term _critical rationalism_.) All criticism is it itself able to be criticized - reasonably and politely of course - hence creating an infinite regress of rational debate. Note this is analogous to the "selection" phase in evolution, with external criticism playing the role of the environment.
3. Repeat steps 1 and 2 in rough proportion to how important the decision is, trying all the while to creatively generate new ideas and subject them to the selection pressures of external critique.
4. Choose whichever action - whichever idea - best survives the critical process. If there is more than one, keep going until there isn't.

So when you say that you know of no other alternatives to the MEU approach, you seem to be echoing Scott Alexander (a writer I admire tremendously), when he [writes](https://slatestarcodex.com/2015/08/24/probabilities-without-models/):

---
> _A lot of responses to my Friday post on overconfidence centered around this idea that we shouldn’t, we can’t, use probability at all in the absence of a well-defined model. The best we can do is say that we don’t know and have no way to find out. I don’t buy this:_
>
> _“Mr. President, NASA has sent me to warn you that a saucer-shaped craft about twenty meters in diameter has just crossed the orbit of the moon. It’s expected to touch down in the western United States within twenty-four hours. What should we do?”_
>
> _“How should I know? I have no model of possible outcomes.”_
>
> _“Should we put the military on alert?”_
>
> _“Maybe. Maybe not. Putting the military on alert might help. Or it might hurt. We have literally no way of knowing.”_
>
> _“Maybe we should send a team of linguists and scientists to the presumptive landing site?”_
>
> _“What part of ‘no model’ do you not understand? Alien first contact is such an inherently unpredictable enterprise that even speculating about whether linguists should be present is pretending to a certainty which we do not and cannot possess.”_
>
> _“Mr. President, I’ve got our Israeli allies on the phone. They say they’re going to shoot a missile at the craft because ‘it freaks them out’. Should I tell them to hold off?”_
>
> _“No. We have no way of predicting whether firing a missile is a good or bad idea. We just don’t know.”_
>
> _In real life, the President would, despite the situation being totally novel and without any plausible statistical model, probably make some decision or another, like “yes, put the military on alert”. And this implies a probability judgment. The reason the President will put the military on alert, but not, say, put banana plantations on alert, is that in his opinion the aliens are more likely to attack than to ask for bananas._

---

It’s as if probabilities are the only way we can learn about the world! It’s simply not true that “The best we can do is say that we don’t know and have no way to find out” or that “[making some decision or another] implies a probability judgment.” No it doesn’t. We learn about the world by guessing and correcting our mistakes.

So at first I was a bit perplexed why most of our other disagreements were downstream of decision theory, but now I think I get it. Scott seems to be saying here that without bayesian decision theory, we will be utterly paralyzed and incapable of deciding anything, like the President dealing with his saucer-shaped craft.

So yes, it’s completely true to say that the President would make some decision, despite the situation being totally novel and without any plausible statistical model. But not because using  probabilities in the absence of a well-defined model is a totally a-okay thing to do, but because Scott is using the wrong model of human decision making.

In reality, the President would make a decision in this scenario the same way we all make decisions. By first creatively generating a few actions (_put the military on alert_, _put banana plantations on alert_, _call Israeli allies_), then internally criticizing them (_put banana plantations on alert? That won’t accomplish anything. I won’t even bother asking my advisors about this one_), then collecting more criticism by asking his advisors (_What are the consequences of putting the military on alert?_) and continuing to iterate in this manner until a decision is made (_We will put the military on alert and call Israeli allies only if the situation escalates_).

Stepping away from Scott’s example, note that both processes suffer from infinite regress and vague terminology, and are predicated on creative software we don’t understand. However, despite this, there are enough differences between the two to make the latter strictly preferable.

First, it satisfies your request for _a general approach to making decisions with these or similarly appealing qualities_, because the latter approach entirely subsumes the former. Expected value calculus can be viewed as a _critique_, and as such, is entirely valid in some circumstances - namely when utilities, actions, and consequences are clearly defined, and we have the opportunity to repeat many trials. This is why decision theory works so well in reinforcement learning on video games like Go or Starcraft, for example. Because in these settings, we have an infinite amount of trials available from repeated games, a clearly defined utility function (win or lose), and a clearly defined action space (move left, right, forward, etc).

But this view liberates us from viewing the expected value calculus as the _only_ critique, or the _only_ approach to decision making on offer. It's much more general. There is no requirement to try to quantify the unknowable, or to anchor decision making to a particular interpretation of the inescapably paradoxical probability calculus, or to a particular axiomatization of what rationality is, or to a limited set of symbols (numbers). All that matters is that we express our ideas as clearly as we can, using every communication tool at our disposal (numbers, characters, images, animations, code, ... ), in order to make it easy for others to spot and correct errors in our reasoning.

Second, it preserves everything the EA community cares about. I too care about the risks of unaligned AI and think we need to act. But that's because my first decision - to do nothing - was successfully criticized by Yudkowsky, Alexander, and others. _Dedicating time and resources to the problem is the most defensible decision_, that is, the decision most resilient to criticism.

Third, it's actually something you can do. As Less Wrong will [tell you](https://wiki.lesswrong.com/wiki/Decision_theory), MEU isn't very useful in practice. (“A core idea in decision theory is that of expected utility maximization, _usually intractable to directly calculate in practice_, but an invaluable theoretical concept." [italics mine])

The vast majority of decisions I have to make throughout my day aren't able to be neatly expressed in a decision matrix - for instance, in deciding what sentence to write next. Creating a set of sentences/actions and criticizing them by simulating possible counter arguments is what operations I'm consciously and constantly performing when deciding what to write. Not computing utilities multiplied by probabilities and then mentally summing them up.

Fourth, it offers counter-intuitive suggestions (or to be a bit more technical, “logical consequences”) which result in behavioral change. If the framework was "make decisions by communicating with people", the theory wouldn’t exactly be wrong, but it wouldn’t be terribly useful either.

CR is only valuable because criticism can be unpleasant, and people therefore usually avoid it. People don’t tend to reorganize their entire life in order to receive and give as much (friendly, constructive, polite, well-intentioned) criticism as they can. But they should, because this is the only way we currently know how to gain knowledge. (Perhaps at some point in the future we will have solved AI, and in the process discovered a more pleasant way to learn and to grow. But for now, it’s all we have).

And finally, CR offers alternative suggestions when faced with a decision that MEU doesn't. For instance, a friend of mine was trying to decide whether to quit his job and he asked for some advice. The MEU strategy would be to compute expected utility of each choice - quitting/not quitting - and choose the larger of the two.

Putting aside the fact that this is a pretty useless thing to say to a friend looking for advice, it entirely neglects the most important aspect of decision making - namely the creation of new options. People are not confined to a decision matrix.

So the advice I gave instead was to _consider new options_. Instead could he drop to part time? Take a leave of absence? Why did he want to quit in the first place? Was there something about his job he could change?

And then we reasoned through the problem together, by considering the consequences of each new possibility, generating new options all the while. Real life decision making is all about creatively generating new options, not mechanically weighing existing ones.

### The usefulness of bayesian analysis and the Bayesian vs Frequentist dichotomy

So, uhhh, how did we get here again? We may be running the risk of completely forgetting what the original disagreement was about, so this is probably a good place to start bringing the subject back to the use of probabilities within the EA community.

> _Next, I'll argue that the weights we should use when making decisions should draw on more than just frequentist analysis, because there are other useful measures of reality, and there is empirical support for the relative accuracy of Bayesian forecasting_

I should have mentioned this in my first response, but my main research focus is in bayesian inference in machine learning (specifically, the area of variational inference and deep generative modelling). I don't say this to argue from authority or anything, but only to say that you have a friend in me when you talk about how bayesian methods are superior to frequentist methods in many ways (make useful predictions on the basis of an event's causal dynamics, aggregating multiple sources of information, allowing the inclusion of information not present in datasets, etc.). Totally agree. I ain't no frequentist!

In fact, a good portion of my research activity is spent programming this exact thing. And when doing so, one quickly realizes that in order to actually implement these systems practice, there is no getting around the fact that you have to use either real or simulated data (or "sampled", to use some jargon). There is no alternative to "frequentist data” - all but the most trivial toy problems require counting _something_.

(Also I’m not sure what “frequentist data” is. “Frequentist” typically refers to a particular interpretation of the probability calculus, and not a kind of data. I suspect you’re using the term “frequentist data” to contrast it against other useful kinds of information about the world that aren’t derived from measurements  - information about causal dynamics, ideas about which reference classes are relevant, mathematical proofs, etc. Just so we’re mapping accurately between one another’s terminology, I refer to all of these kinds of statements as _arguments_ when used to criticize ideas in the service of being less wrong ).

So this is why I chose to focus in my opening salvo on another dichotomy; namely the use of (bayesian, frequentist, doesn't matter) probabilities with measurements vs probabilities without. This doesn't rule out bayesian statistics, but it does rule out moves like this:

> _In the case of artificial intelligence, everyone agrees the evidence and arguments are far from watertight, but the question is where does this leave us? Very roughly, my approach is to start with the overall view of the expert community that there is something like a one in two chance that AI agents capable of outperforming humans in almost every task will be developed in the coming century._
>
> \- _Toby Ord, The precipice, Chapter 6, page 165_

Imagine if I were to reply to Ord as follows:

> _Well I **am** an expert in the community, and after surveying the relevant literature, I believe the chance is only is 0.00001% that AI agents capable of outperforming humans in almost every task will be developed in the coming century!_

And someone from the audience yells:

> _Laughable! You are both fools! I too am an expert - more expert than either of you undoubtedly - and **my** survey of the most valuable and important literature has revealed that the chance is over three orders of magnitude greater than 1/2 that AI agents capable of outperforming humans in almost every task will be developed in the coming century!_

and so on. These arguments are _all invalid_. Even if we are all perfect bayesian decision makers, and even if we recognize that bayesian methods are superior to frequentist ones, this is still an invalid argument, for the simple reason that any number at all can be made up and defended in this manner.

We have learned nothing from this exchange, because arbitrary numbers representing beliefs - numbers uninformed by simulations or counts - have been offered in place of arguments. My rebuttal was vacuous for this reason - akin to saying “Because I believe it!”. Arguments we can learn from, _arguments we can do something with_.

This is the move I'm saying is illegitimate. Made up numbers, whether called “'rational beliefs” or "subjective probabilities" or "priors" or "credences" or "just orders of magnitude” or "uncertainty", must be somehow constrained by data (simulated or real) for them to be any more than just a measure of the speaker's subjective feeling of confidence. And as the superforecaster example shows, this information is only accurate for a select “super” few of us anyway. I'm all for bayesian statistics, but not bayesian epistemology and its cloud of euphemisms.

So I really want to pin you down here. When you say

> _One part of your response that I especially appreciated was your point about how Bayesians / EAs often rely heavily on probabilities with little backing (or none?) as if they were well supported. I'll argue that what EAs are doing that looks like this is often fine, but after reading your last response I expect to be paying more attention to how probability estimates were formed, and to what this implies for their value as information, and for the value of further information._

I can't tell if you agree that this move is illegitimate or not. If you agree my fake answer to Ord is a fallacious argument from authority from which we have learned nothing, then so is Ord’s, and we can all go home.

### Superforecasters demonstrating subjective probabilities can track objective ones

> _As Scott Alexander's review of Superforecasters discusses, Philip Tetlock's team of "superforecasters" probabilistically predicted future events (the details of which were unprecedented) with greater accuracy (closeness to objective probabilities) than chance, and with greater accuracy than CIA forecasters working with classified information. (And they didn't just get lucky--the same people tended to be superforecasters over multiple rounds of testing.) Tetlock writes:_

 > > _The superforecasters are a numerate bunch: many know about Bayes’ theorem and could deploy it if they felt it was worth the trouble. But they rarely crunch the numbers so explicitly. What matters far more to the superforecasters than Bayes’ theorem is Bayes’ core insight of gradually getting closer to the truth by constantly updating in proportion to the weight of the evidence. That’s true of Tim Minto [the top superforecaster]. He knows Bayes’ theorem, but he didn’t use it even once to make his hundreds of updated forecasts. And yet Minto appreciates the Bayesian spirit. “I think it is likely that I have a better intuitive grasp of Bayes’ theorem than most people,” he said, “even though if you asked me to write it down from memory I’d probably fail.” Minto is a Bayesian who does not use Bayes’ theorem. That paradoxical description applies to most superforecasters._

Well, it's not all that paradoxical when you realize that "getting closer to the truth by constantly updating in proportion to the weight of the evidence" actually just means "constantly correcting errors by criticizing your ideas about future events". As the superforecasters say, it's about the "Bayesian spirit" (i.e error correction), not taking literally some mathematical identity which allows you to switch the order of conditional probabilities. This is how we become less wrong. Paradox resolved.

(FWIW Scott says the same thing in the link you provided: "_[Superforecasters are] more likely to admit they might be wrong and correct themselves after an error is discovered. They’re more likely to debate with themselves, try to challenge their original perception, start asking “What could be wrong about this thing I believe?” rather than “How can I prove I’m right?”_)

> _Assuming that Tetlock's claim is supported by the thousands of data points he collected, frequentist analysis seems to provide support for the usefulness of Bayesian analysis._
> _This looks pretty good for Toby Ord, and for thinking that such forecasts are far from probabilities "made up out of thin air._

Completely agree that Bayesian analysis is useful (see above). But the existence of people who are better than average at error correcting, doesn't make my response to Ord any more legitimate. If you allow this kind of reasoning for Ord, you must allow it for me, and we’re back at square one, with the process of correcting one another’s errors ground to a halt.

> _Note that the predictions that Tetlock's forecasters made were unconditional probabilistic predictions. And the vast majority of forecasters did better than chance (not just the superforecasters, although they did especially better than chance). This is (frequentist) evidence against the claim that "there are no objective probabilities - no measurements from which to derive probabilities - when dealing with the unconditional future._

Well no, not really. One way to see this is to consider the classic coin flip. In this instance, we have a clearly defined notion of objective probability - it's a property of the coin, and can be measured through experimental trials. It therefore makes sense to talk about aligning one's subjective probability with objective probabilities here, because there are in fact objective probabilities to align against.

But unless you want to invoke Everettian many worlds, we only have a single future. There either will, or will not be, a war between North and South Korea in the next ten years killing > 1000 people. The next ten years will only happen once. What is the objective probability of a single event? It's undefined. Why? Because there is _nothing to measure_, unlike repeatedly flipping a coin and counting _heads_, or measuring the half life of carbon-14, or counting asteroids, or whatever. Nothing to measure, no objective probabilities.

If this all feels weird and circular and unsatisfying, well, welcome to the paradoxical nature of probability:

---

> You try to explain what a probability statement means — say, that heads will probably come up about half the time when you toss coins — and you find yourself reducing it to other probability statements — such as that if you bet on some other proportion you are ‘likely’ to lose. It seems that you can never reduce it to ‘so and so _will_ happen’. Consequently, people have been reduced to talking nonsense about this, such as the ‘frequency’ or ‘ensemble’ interpretations of probability. They say that something is ‘probable’ if it would happen in the majority of cases, if the experiment were repeated infinitely many times. But then they are not talking about reality, because real experiments aren’t performed infinitely many times. And even if they were, we want to know what to do on particular occasions. And in any case, the frequency interpretation, whether with an infinite or a finite number of instances, logically doesn’t reproduce probabilities unless the instances are equally likely, which gives a circular definition of ‘likely’.
>
> Other people have tried to say that probability is a measure of subjective belief. But then you have to explain why my subjective belief about the coin should be a property of the coin rather than just of me — and the answer has to be that it’s not any old belief, it’s the belief that I _should_ have, if I’m rational. But then, why should rational people have that subjective belief? Because if they were to adopt some other belief they would be likely to lose bets. There’s the circularity again.
>
> David Papineau once called this state of affairs at the foundations of probability theory a scandal.
>
> \- David Deutsch, In Many worlds?: Everett, Quantum Theory, and Reality

---

So superforecasters or not, the concept of objective probabilities of singularly occurring events still remains undefined. But this is only half the story, because I haven't explained what's going on in the superforecasters example. I'm going to take Scott's post [here](https://slatestarcodex.com/2020/04/08/2019-predictions-calibration-results/) as representative of the kinds of questions Tetlock used, just because the data and results were easier to find -  let me know if Tetlock's case differs in any significant way. Scott's scores for 2019:

> _Of 11 predictions at 50%, I got 4 wrong and 7 right, for an average of 64%_\\
> _Of 22 predictions at 60%, I got 7 wrong and 15 right, for an average of 68%_\\
> _Of 17 predictions at 70%, I got 5 wrong and 12 right, for an average of 71%_\\
> _Of 37 predictions at 80%, I got 6 wrong and 31 right, for an average of 83%_\\
> _Of 17 predictions at 90%, I got 1 wrong and 16 right, for an average of 94%_\\
> _Of 5 predictions at 95%, I got 0 wrong and 5 right, for an average of 100%_

What are we actually learning here? That _when Scott says he's X% confident about something, he's right X% of the time (probably)_. Good. We can trust Scott when he says he's confident about something. But how is this evidence against the claim that there are no objective probabilities when dealing with the singular, unmeasurable future? The objective probabilities in this case just come from all the other times Scott has said he is X% confident about stuff, and don't refer to the future at all.

To really hammer this point home, consider that we could have learned the exact same thing about Scott if we opened any pub quiz book and selected a few hundred questions at random about history, literature, geography, and mathematics (i.e. anything but the future). If he assigned confidence scores to each and we scored them using the answers at the back of the book, we would have learned what we learned in the forecasting case, except without having to wait a year.

The point is, we're learning about Scott here, and the accuracy of his subjective feeling of certainty - not some objective property of the future.  And the same goes with all of Tetlock's superforecasters.

### Summary

So there are a number of dangling arguments still left unaddressed, but wanted to give some closing thoughts and also give you an opportunity to let a few threads die off if they're no longer interesting.  I'll do my best to hit all the remaining direct questions in the "loose ends" section below.

It's always a great learning opportunity when two philosophies collide. In this case, it's between clashing epistemologies - Bayesian Rationality and its focus on _updating beliefs_ on the one hand, and Critical Rationalism and its focus on _critical arguments_ on the other. And while they have many similarities, it's the differences which are most relevant to us at present.

I would submit that bayesian rationality, with its emphasis on _evidence_, _beliefs_, and _uncertainty_ over _knowledge_, _arguments_, and _criticism_, is missing the forest for the trees. If updating beliefs is the central focus at the end of the day, and not producing, understanding, and criticizing one another’s arguments, then you may ask why we didn't just skip this whole ordeal by asking for one another’s belief scores. As this series of letters will show upon reexamination, it's because what we actually value is critical arguments. Not beliefs. This is a classic instance of struggling to see what is right in front of one’s nose.

### Loose Ends

> _Neurons seems roughly Bayesian_

I'm happy to accept that

> _If these feelings aren't subjective credences that I usually track automatically (and consciously, when I put my slow, explicit thinking to the task), then what are they?_

Well they're just that, feelings. Who is to say they have numbers that sum to one attached to each? Dutch Book-style arguments about rational betting are no use here, because they always begin "If an agent is rational in a particular way, then ...". But we know humans aren't rational (cognitive biases, kahneman and tversky and all that), and therefore dutchbook arguments don’t apply to humans but to idealized rational agents who only exist in our imagination.

> _I don't know how to judge which strategy is best in other circumstances: when my subjective credences deviate significantly from objective probabilities. That seems like asking "what would be the case if I'm just terrible at figuring out what is the case?" If I'm terrible at figuring out what is the case, then how would I know?_

Yes you do! Of course you do! You're selling yourself short :) See alternative above and discussion on subjective credences tracking objective probabilities.

> _Your last step here, going from ruling out definite predictions to ruling out probabilistic forecasts, doesn't make sense to me. We cannot predict all (or much) of how things will go in the future, but we are not completely clueless either--we can still make useful probabilistic forecasts, on the basis of aspects of the future about which we are not clueless._

Whoops yeah my bad, poorly explained. This is actually explained more clearly by Ord in one of his footnotes.

> _For instance, we shall sometimes have to say that something used to be a risk (given our past knowledge), but is no longer one. One example would be the possibility that nuclear weapons would ignite the atmosphere (see p. 90). But note that this comes up for all kinds of risk, such as thinking last week that there was a risk of the elevator falling due to a frayed cable, but having this risk drop to zero given our current knowledge (we inspected the cable and found it to be fine)._
>
> \- _Toby Ord, The Precipice, Footnote 9, Chapter 2_

So Ord and Popper and I agree that all risk assessments can change entirely (drop to zero, etc) given new knowledge. So that last step - ruling out probabilistic forecasts - only applies when the forecast in question is causally dependent on future knowledge - i.e Malthus predicting mass starvation, superintelligent AI - but not things like Halley's comet or volcanic eruptions, which presumably will happen whether or not we learn more about them.

> _I agree that using expert beliefs requires us to make choices. Why would it follow that these choices must be arbitrary? A few ways in which the choice of which experts to listen to may be made non-arbitrarily:_
> - _Use frequentist data about experts. Tetlock also provides evidence for the claim that experts who consider many angles / perspectives do better than chance at forecasting, while experts who "know one big thing" tend to do worse than chance. My limited knowledge of (especially Abrahamic) theology suggests that "knowing one big thing" is a decently accurate characterization of much of it._
>   - _Theologians predicting the end of the world also have a pretty terrible track record_
> - _Use your beliefs about the reliability of various kinds of experts. My beliefs say that intellectual traditions which valorize faith will tend to produce predictions less correlated with objective probabilities._
>   - _Yes, this argument for beliefs is circular. This is fine, because here I'm arguing, not that Bayesianism has external justification, but that it's coherent._

“Arbitrary” in the sense that half the US considers Tucker Carlson to be an expert, and the other half Rachel Maddow, and which you believe tends to depend mainly on geography. Everyone has different beliefs about which experts are reliable, and then tend to collect data to support these beliefs. This is the cause of the problem, not a solution to it.

And yeah, okay, it was a little unfair of me to replace "credence" or "subjective credence", or “holistically informed, subjective credences” with the word "belief" in the above near-quote. But I was hoping you might be able to hear just how weird it sounds to have a rationalist and presumed atheist argue so strongly in favour of belief.

---

[^1]:Arrow’s theorem applies not only to collective decision-making but also to individuals, as follows. Consider a single, rational person faced with a choice between several options. If the decision requires thought, then each option must be associated with an explanation – at least a tentative one – for why it might be the best. To choose an option is to choose its explanation. So how does one decide which explanation to adopt? Common sense says that one ‘weighs’ them – or weighs the evidence that their arguments present. This is an ancient metaphor. Statues of Justice have carried scales since antiquity. More recently, inductivism has cast scientific thinking in the same mould, saying that scientific theories are chosen, justified and believed – and somehow even formed in the first place – according to the ‘weight of evidence’ in their favour. <br /> <br />  Consider that supposed weighing process. Each piece of evidence, including each feeling, prejudice, value, axiom, argument and so on, depending on what ‘weight’ it had in that person’s mind, would contribute that amount to that person’s ‘preferences’ between various explanations. Hence for the purposes of Arrow’s theorem each piece of evidence can be regarded as an ‘individual’ participating in the decision-making process, where the person as a whole would be the ‘group’.  <br /> <br />   Now, the process that adjudicates between the different explanations would have to satisfy certain constraints if it were to be rational. For instance, if, having decided that one option was the best, the person received further evidence that gave additional weight to that option, then the person’s overall preference would still have to be for that option – and so on. Arrow’s theorem says that those requirements are inconsistent with each other, and so seems to imply that all decision-making – all thinking – must be irrational. Unless, perhaps, one of the internal agents is a dictator, empowered to override the combined opinions of all the other agents. But this is an infinite regress: how does the ‘dictator’ itself choose between rival explanations about which other agents it would be best to override?  <br />  <br /> There is something very wrong with that entire conventional model of decision-making, both within single minds and for groups as assumed in social-choice theory. It conceives of decision-making as a process of selecting from existing options according to a fixed formula (such as an apportionment rule or electoral system). But in fact that is what happens only at the _end_ of decision-making – the phase that does not require creative thought. In terms of Edison’s metaphor, the model refers only to the perspiration phase, without realizing that decision-making is problem-solving, and that without the inspiration phase nothing is ever solved and there is nothing to choose between. At the heart of decision-making is the creation of new options and the abandonment or modification of existing ones.   <br />  <br /> To choose an option, rationally, is to choose the associated explanation. Therefore, rational decision- making consists not of weighing evidence but of explaining it, in the course of explaining the world. One judges arguments as explanations, not justifications, and one does this creatively, using conjecture, tempered by every kind of criticism. It is in the nature of good explanations – being hard to vary – that there is only one of them. Having created it, one is no longer tempted by the alternatives. They have been not outweighed, but out-argued, refuted and abandoned. During the course of a creative process, one is not struggling to distinguish between countless different explanations of nearly equal merit; typically, one is struggling to create even one good explanation, and, having succeeded, one is glad to be rid of the rest.<br /> <br /> - Beginning of Infinity, page 236
