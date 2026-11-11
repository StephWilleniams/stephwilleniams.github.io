---
layout: organism
slug: chlamydomonas
title: Chlamydomonas reinhardtii
summary: How swimming microalgae drive passive particles under confinement, and how to use that to sort them.
collaborators: Marco Polin (IMEDEA), Raphaël Jeanneret, Idan Tuval, Shilpa Khatri
---

## The question

Many microbes live in mixtures: some swim, some don't. When the swimmers bump into passive particles, they push them around, and in a confined space, like a microfluidic channel or a host's tissues, those collisions can organize the whole suspension. How do swimmers redistribute the particles around them, and can we control it?

## What I found

In my PhD with Prof. Marco Polin at the University of Warwick, I combined swimming *Chlamydomonas reinhardtii* with passive colloids in microfluidic channels. Confinement alone produced a non-monotonic colloid distribution, with a pronounced peak at the boundary. I captured this with a stochastic, space-dependent jump-diffusion model driven by the algae's motion, and we used the effect to de-mix active–passive suspensions experimentally.

<figure>
  <img src="{{ '/images/research/channelFilling.png' | relative_url }}" alt="Simulation snapshots of swimmers driving passive particles into narrow side channels" loading="lazy" onerror="this.closest('figure').remove()">
  <figcaption>Active swimmers (red) drive passive colloids (blue) into side channels too narrow for the swimmers to enter: (A) weakly and (B) strongly scattering swimmers.<span class="credit">Figure: Stephen Williams</span></figcaption>
</figure>

## What's next

I am generalizing these results to a broader class of microswimmers, showing how scattering events near a boundary control where passive particles end up. My squid research extends the same problem to a much more complex case: a boundary that is alive.

## Outputs

- Williams, S., Jeanneret, R., Tuval, I., Polin, M. Confinement-induced accumulation and de-mixing of microscopic active–passive mixtures. *Nature Communications* 13, 4776 (2022). [Paper](https://doi.org/10.1038/s41467-022-32520-9) · [Preprint](https://arxiv.org/abs/2111.09763) · [Code](https://github.com/StephWilleniams/ActivePassiveConfinement)
- In preparation: Williams, S., Khatri, S., Polin, M. Controlling passive particle distributions in mixed systems through active scattering events.
- PhD thesis: *Mixed Active–Passive Systems in Confinement*, University of Warwick (2022).
