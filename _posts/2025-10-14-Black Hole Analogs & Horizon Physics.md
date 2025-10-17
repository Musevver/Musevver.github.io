---
layout: post
title: "Black Hole Analogs & Horizon Physics"
author: "Musevver Ugursal"
---


Black holes prove to be an increasingly fascinating rabbit hole for me. The idea that through Einstein's field equations you can have solutions that permit regions of space dominated by a *singularity* and shielded from view via the *event horizon* (the causal boundary of spacetime, once inside, nothing can escape) is an idea so absurd in principle that Einstein himself failed to consider its physicality. A lot of focus is given to the singularity and while it is an area of immense theoretical potential it is inaccessible by all modes of measure as it hides behind the event horizon, this proves frustrating as in physics there exists a contemporary tension between *Quantum Field Theory* & *General Relativity* as to what the fundamental nature of gravity is. 


They are both highly successful and celebrated theories and yet they give fundamentally incompatible answers to the question of "*how does gravity behave on the scale of quantum mechanics?*". This is where black holes shine, they act as stress tests for both the relativistic theory and the quantum theory simultaneously, however, given that the singularity is irrevocably hidden behind the horizon it might seem as though all progress in our understandings of black holes are hopelessly locked away but this isn't the case. I was reading a paper by Unruh & Wald in which they discuss what the vacuum would appear to be like for an accelerating observer far out in flat space, the conclusion is fascinating, an accelerated observer would measure the vacuum to have *thermality* and they would be able to physically justify this result both through relativity and quantum mechanics. Admittedly the math used in the paper got to be too much for me towards the end and I couldn't find any useful supplemental materials from either author as quite literally everything that Unruh and Wald have ever written are above anything I can currently follow through, however I was able to write code using these principles(more on that later).


Nevertheless I include a (crude) derivation:

$$ t = \xi \sinh\!\Bigl(\frac{a\tau}{c}\Bigr) \qquad x = \xi \cosh\!\Bigl(\frac{a\tau}{c}\Bigr) \qquad \xi > 0 $$

Above we have what a uniformly accelerated observer with hyperbolic acceleration would use where $$\xi$$ is the greek letter "*Xi*" representing how far the observer measures their own horizon to be, this then transforms their flat-space metric to become approximately(near the horizon):

$$ ds^2 = - (a\xi)^2 c^2\, d\tau^2 + d\xi^2 $$

We then use a "Wick rotation" which will transform our time to an imaginary time, this allows us to treat time as an extra spatial dimension, allowing for a vast simplification in the derivation. Note that it's analogous to the polar-coordinate form of the metric.

$$ ds^2 = (a\xi c)^2\ dt_E^2 + d\xi^2 $$

$$ ds^2 = r^2\ d\theta^2 + dr^2 $$

One consequence of turning our time into an imaginary spatial component is that we must now account for its periodicity $$\beta$$.

$$ \beta = \frac{2\pi c}{a} $$ 

Note that the $$2\pi$$ is a direct consequence of the polar-coordinate analog from earlier.


Next we use a known result from quantum mechanics, the correlation between imaginary-time periodicity and thermal states.

$$ T = \frac{1}{k_B \beta} $$

We then substitute the $$\beta$$ we obtained before to achieve the Unruh thermality:

$$ T_U = \frac{\hbar a}{2\pi c k_B} $$


Note the $$\hbar$$, this is a consequence of translating a time periodicity into an energy scale via the relation:

$$ e^{-i H t / \hbar} $$

A truly remarkable result, the Unruh effect challenges our idea of a vacuum and how a horizon gives rise to thermality, from it we gain some important insights about black holes. Notably, we no longer view the horizon as a dead-end, instead we now see it as a tool that allows us to develop new theories that will get us closer towards a theory of quantum gravity. The issue now is to build a model of an observer-*independent* black hole horizon from the observer-*dependent* Rindler horizon described by the Unruh effect, and I will lament that the Unruh effect derivation just about killed me trying to understand it and that generalizing it would be an even taller task. For this reason I am going to chicken out and instead I will do what any self-respecting physics student would do and attempt to "reason" the global solution from the Unruh effect, the general reasoning is sound although not rigorous in the slightest, it is as follows:

1. Consider the Unruh thermality derived earlier.
 
2. Now consider the equivalence principle which briefly states that "a gravitational field and an acceleration field are locally indistinguishable".
 
3. Therefore, what we previously assigned as *acceleration*-thermality is now indistinguishable from *gravitational*-thermality.

4. Reconcile then, that we can accurately model the black hole horizon locally using the Unruh effect.
  
5. Finally, a global solution is found once an outside observer is considered. This outside observer sees the radiation bleed from the black hole and redshift to infinity.

That final result is fascinating, the fact that through simple reasoning and logic(and a lot of math!) you now have this picture of a black hole that "bleeds". Your first instinct might be to think that this is some kind of relativistic "trick" but it is indeed real, the black hole radiates energy outward(very slowly!) and therefore loses mass in the process. What's really amazing to me actually is that timeline-wise, this global and more universal effect was formulated earlier than the Unruh effect by Stephen Hawking. This effect has since been named in honour of him, Hawking radiation.

Now all that remains is experimental evidence in favour of Hawking radiation and we have our first foothold towards finally understanding black holes, as Carl Sagan would say "*Extraordinary claims require extraordinary evidence*", but how do you even go about experimenting with a black hole? Unruh's formulation and Hawking's formulation have something in common, they are scale-*independent* and mass/gravity-*independent*, they are only dependent on two things:

1. A horizon.

2. A space-time.
   
and if you're thinking "*yeah but that's the hard part*" it turns out, in fact, to be the easiest part. Crucially, scale and mass independence mean that we don't need a giant undisturbed patch of spacetime with an event horizon, we need an object that behaves like a horizon and we need a medium that behaves like a space-time, let's refine what we're looking for:

1. A horizon *analog*.
 
2. A space-time *analog*.

The word analog means equivalent, reminiscent of the equivalence principle, the very fact that analogs are now in play means this problem has gone from a "thinking hard" problem to a "thinking different" problem. We first tackle the horizon analog, ultimately a horizon has two conditions, it must be:

1. A one-way information boundary.
 
2. Causally defined in an effective space-time.

The only way to manipulate light such that it satisfies the two conditions above is if we had an event horizon but since we're fresh out we need another kind of wave to manipulate, a natural progression is a sound wave as it's easily manipulable and observable. Therefore we will consider the "*Sonic horizon*" as a useful analog.

We now tackle the concept of a space-time analog, the two conditions for a space-time are that:

1. It must provide a metric.
 
2. It must appear continuous.

We have already selected a great analog for the horizon, this constrains what we can now select as a useful space-time analog, clearly it must be dense as we must propagate sound through it but it must also be easily manipulable, smooth on the scales of sound waves, cold so that noise doesn't overpower our sound waves. Cold, smooth, manipulable, that's a textbook description of a Bose-Einstein condensate and indeed it checks all the boxes that we require from it. And so now we have a useful space-time analog in the form of a Bose-Einstein condensate.

Using this setup scientists have been able to not only create very accurate horizons right here on earth but they've already been able to detect the hawking radiation in the phonons(sound waves) used in their setups. This is by no means confirmation that this will exactly work for real black holes but it's very hopeful, we have mathematical proof of hawking radiation and we now have simple analogs that produce what the theory predicts, this leaves scientists hopeful and means we've effectively established our first real foothold in understanding these "cosmic stress tests". Also I highly recommend reading about the "Anderson-Higgs mechanism" as it has some parallels with what we've discussed here *i.e.* theory --> model building --> experimental evidence.

And that's it! That's everything you need to conduct what I would call "*Horizon Physics*". It's a very young field and it doesn't necessarily exist to mature, it exists as an ephemeral tool to guide us towards a theory of quantum gravity. This idea of sonic black holes and horizons really fascinated me and the math was surprisingly "co-operative" in that it made symbolic manipulation fairly simple. For this reason i have coded a basic 1-D sonic horizon simulator in python, it is on my GitHub if you'd like to play around with it. In the future I might do one for an optical black hole as well or move onto another project, I had a lot of fun going down this rabbit hole and I hope it interested you as well!

<script>
window.MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']],
    tags: 'ams'
  },
  options: { skipHtmlTags: ['script','noscript','style','textarea','pre','code'] }
};
</script>
<script id="MathJax-script" async
        src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>
