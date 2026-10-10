---
layout: organism
slug: euprymna-scolopes
title: Euprymna scolopes
summary: Modeling the breathing- and cilia-driven flows the Hawaiian bobtail squid uses to recruit its bacterial symbiont, and how heat stress disrupts them.
collaborators: Elizabeth Heath-Heckman (Michigan State), Kyra Ruiz, Erica Rutter, Shilpa Khatri
---

## The question

Within hours of hatching, the Hawaiian bobtail squid has to recruit the bioluminescent bacterium *Vibrio fischeri* from seawater. Bacteria are drawn into the squid's mantle cavity by breathing, then captured by flows from cilia on the light organ, where they settle in for the squid's lifetime [1]. Warming impairs this colonization [2], but where in the process the failure happens is not known.

## What I built

With the Heath-Heckman lab, I built a fluid-dynamics model of breathing-driven bacterial transport inside the squid, using the method of regularized Stokeslets. Varying breathing strength, breathing rate, ciliary beating and squid size across tens of thousands of simulations, I ran a Sobol sensitivity analysis to find which factors control how long bacteria spend near the light organ.

<figure>
  <img src="{{ '/images/research/internalCavity.png' | relative_url }}" alt="Diagram of breathing flow into the squid's mantle cavity and out through the funnel" loading="lazy" onerror="this.closest('figure').remove()">
  <figcaption>Breathing flow into the mantle cavity (red) and out through the funnel.<span class="credit">Figure: Stephen Williams</span></figcaption>
</figure>

<figure>
  <img src="{{ '/images/research/flowExample.png' | relative_url }}" alt="Simulated flow field inside the mantle cavity, with streamlines and speed shown in color" loading="lazy" onerror="this.closest('figure').remove()">
  <figcaption>Regularized-Stokeslet simulation of the mantle-cavity flow. White lines are particle streamlines; color is speed.<span class="credit">Figure: Stephen Williams, from <a href="https://doi.org/10.1098/rsif.2025.1136">Williams et al. (2026)</a></span></figcaption>
</figure>

## What we found

Breathing strength, breathing rate and squid size dominate how long bacteria stay near the light organ. The shallow, rapid breathing of heat-stressed squid can halve the time bacteria spend in the regions that matter for colonization, a purely physical route by which warming could weaken the symbiosis.

## What's next

- Extending the model to a realistic, deforming mantle cavity.
- Adding swimming and chemotaxis, since *V. fischeri* are not passive tracers. Does active swimming buffer recruitment against weakened breathing, up to a threshold temperature?

Try a simplified version of the flow method in the [interactive Stokeslet demo]({{ '/#interactive' | relative_url }}).

## Outputs

- Williams, S., Ruiz, K. A., Heath-Heckman, E., Rutter, E. M., Khatri, S. Thermal stress disrupts symbiotic fluid dynamics in bobtail squid. *J. R. Soc. Interface* 23, 20251136 (2026). [Paper](https://doi.org/10.1098/rsif.2025.1136) · [Code](https://github.com/StephWilleniams/SquidInternalFlows)
- [Poster: MDDLS 2025]({{ '/updates/mddls-2025/' | relative_url }}) · [Invited talk: AMS Western Sectional 2026]({{ '/updates/ams-western-sectional/' | relative_url }})

## References

<ol class="refs">
  <li>Nawroth, J. C. et al. Motile cilia create fluid-mechanical microhabitats for the active recruitment of the host microbiome. <em>PNAS</em> 114, 9510–9516 (2017). <a href="https://doi.org/10.1073/pnas.1706926114">doi:10.1073/pnas.1706926114</a></li>
  <li>Otjacques, E. et al. <em>Global Change Biology</em> (2025). <a href="https://doi.org/10.1111/gcb.70243">doi:10.1111/gcb.70243</a></li>
</ol>
