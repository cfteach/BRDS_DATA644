<center>

# MCMC Examples

(last update: Mar 19/2024)

</center>

The following examples are embedded from the MCMC simulations by [Chi Feng](https://chi-feng.github.io/mcmc-demo/).



<br>
<p style="margin-top:20px;"></p>

<b> Random Walk with Metropolis-Hastings (2D Gaussian example) </b>

The target distribution is a benign two-dimensional Gaussian—a nice Gaussian hill. You are looking down on it, with its peak in the center. The Markov chain wanders around this hill, making random proposals to move away from its current position. These proposals are represented by the arrows. We are implementing Metropolis-Hastings.

```{raw} html
<iframe src="https://elevanth.org/mcmcdemo2/applet.html#RandomWalkMH,standard" width="700" height="400"></iframe>
```



<br>
<p style="margin-top:20px;"></p>

<b> Random Walk with Metropolis-Hastings (donut example) </b>

Here’s another simulation, this time with a harder target: a donut. The donut target might look weird, but it represents a very common target, by analogy. In high dimensions—once there are many parameters—the target distribution occupies a narrow ring (in high-dimensional space). Most of the probability mass is not near the center. Now look what happens to honorable Metropolis-Hastings:

```{raw} html
<iframe src="https://elevanth.org/mcmcdemo2/applet.html#RandomWalkMH,donut" width="700" height="400"></iframe>
```



<br>
<p style="margin-top:20px;"></p>
<b> Hamiltonian Monte Carlo (2D Gaussian example) </b>

To make things a little crazier, suppose that this surface is frictionless. Now what we do is flick the particle in a random direction. It will frictionlessly flow across the bowl, eventually turning around. If we take samples of the particle’s position along its path, before flicking it off in another random trajectory, then we can learn about the shape of the surface.

This is the principle behind Hamiltonian Monte Carlo. It will be easier to see it in action. Here is another simulation, this time using Hamiltonian Monte Carlo, again on the two-dimensional Gaussian target. The paths are flicks of the particle, and the green arrows again represent accepted proposals.

```{raw} html
<iframe src="https://elevanth.org/mcmcdemo2/applet.html#HamiltonianMC,standard" width="700" height="400"></iframe>
```



<br>
<p style="margin-top:20px;"></p>

<b> Hamiltonian Monte Carlo (donut example) </b>

Now see on the donut example

```{raw} html
<iframe src="https://elevanth.org/mcmcdemo2/applet.html#HamiltonianMC,donut" width="700" height="400"></iframe>
```
