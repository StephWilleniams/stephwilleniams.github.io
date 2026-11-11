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

<div class="fig-row">
<figure>
  <img src="{{ '/images/research/internalCavity.jpg' | relative_url }}" alt="Top view of a bobtail squid with the mantle cavity outlined in red and blue arrows showing water flowing in at two inflows and out through the funnel" loading="lazy" onerror="this.closest('figure').remove()">
  <figcaption>Breathing flow: water enters the mantle cavity (outlined in red) at two inflows and leaves through the funnel (outflow).<span class="credit">Illustration: Stephen Williams</span></figcaption>
</figure>
<figure>
  <img src="{{ '/images/research/flowExample.jpg' | relative_url }}" alt="Simulated flow field with white streamlines bending around four circular obstacles, colored by speed" loading="lazy" onerror="this.closest('figure').remove()">
  <figcaption>A regularized-Stokeslet simulation. White lines are particle streamlines; color is flow speed.<span class="credit">Figure: Stephen Williams</span></figcaption>
</figure>
</div>

## What we found

Breathing strength, breathing rate and squid size dominate how long bacteria stay near the light organ. The shallow, rapid breathing of heat-stressed squid can halve the time bacteria spend in the regions that matter for colonization, a purely physical route by which warming could weaken the symbiosis.

## What's next

- Extending the model to a realistic, deforming mantle cavity.
- Adding swimming and chemotaxis, since *V. fischeri* are not passive tracers. Does active swimming buffer recruitment against weakened breathing, up to a threshold temperature?

Try a simplified version of the flow method in the [interactive Stokeslet demo]({{ '/#interactive' | relative_url }}).

## Outputs

- Williams, S., Ruiz, K. A., Heath-Heckman, E., Rutter, E. M., Khatri, S. Thermal stress disrupts symbiotic fluid dynamics in bobtail squid. *J. R. Soc. Interface* 23, 20251136 (2026). [Paper](https://doi.org/10.1098/rsif.2025.1136) · [Preprint](https://arxiv.org/abs/2511.00326) · [Code](https://github.com/StephWilleniams/SquidInternalFlows)
- [Poster: MDDLS 2025]({{ '/updates/mddls-2025/' | relative_url }}) · [Invited talk: AMS Western Sectional 2026]({{ '/updates/ams-western-sectional/' | relative_url }}) · [Talk: CassiopeaBase MATH-BIO 2026]({{ '/updates/cassiopeabase-math-bio-2026/' | relative_url }})
- Ongoing: Exploring the impacts of squid breathing dynamics on bacterial symbiont acquisition.
- [Interactive: Stokes flow from point forces]({{ '/interactive/#stokeslets' | relative_url }})

## References

<ol class="refs">
  <li>Nawroth, J. C. et al. Motile cilia create fluid-mechanical microhabitats for the active recruitment of the host microbiome. <em>PNAS</em> 114, 9510–9516 (2017). <a href="https://doi.org/10.1073/pnas.1706926114">doi:10.1073/pnas.1706926114</a></li>
  <li>Otjacques, E. et al. <em>Global Change Biology</em> (2025). <a href="https://doi.org/10.1111/gcb.70243">doi:10.1111/gcb.70243</a></li>
</ol>
