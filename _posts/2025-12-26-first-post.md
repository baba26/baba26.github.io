---
title: "Fugacity"
---

Today I want to talk about "fugacity", in the context of grand canonical ensemble. This concept has confused me for a long time. But I think now I understand it enough to write this blog.

To setup the stage, we have a system that it is surrounded by a particle bath. So the system can gain or loose particles to environment. All this is to say that the number of particles in the system is not fixed. What's the partition function of such a system? This system is an example of what one abstractly calls as "grand canonical ensemble". In other words, if you consider this system at different times, and put all these snapshots of the system in a bag, you have constructed yourself a ensemble with varying number of particles. The partition for grad canonical ensemble is:
$$ Z_{GC} = \sum_{N=0}^{\infty} \int d(phase)\ e^{-\beta(H-\mu N)}   $$
Here N is the number of particles. d(phase) is the integration measure of phase space but its precise form doesn't matter for this discussion. [math]\mu[/math] is the chemical potential.
This can be rewritten as:
$$ Z_{GC} = \sum_{N} e^{\beta \mu N}\ Z_{canonical}^N $$
Here [math]Z_{canonical}^N[/math] is the canonical partition function for a system with N particles. Note that in canonical partition function the number of particles is fixed.

This expression is saying that a grad canonical partition function can be written as sum of canonical partition functions with different particle numbers, and each canonical partition function is weighted by a factor [math] e^{\beta \mu N} [/math]. Using the formal definition of fugacity ( denoted by z ), we can write:
$$ Z_{GC} = \sum_N z^N\ Z^{canonical}$$
Now we are ready to interpret the meaning of z. Let's first consider what happens if z is 1. Well, then all configurations ( irrespective of the particle number N ), are weighted equally. If z is smaller than 1, then configurations with smaller N weighted stronly over those with larger N. In all the averages ( hence all the observables ), smaller N configurations will contribute more. Conversely, if z is larger than 1, then large values of N will dominate all macroscopic observables. 

So we can say that fugacity parametrizes how many particles tend to be in the system. Sometimes people also say that fugacity is a control knob that allows us to regualate how many particles we want in the system.

If we had different kinds of particles, then we would have different fugacities for each of those particles.
