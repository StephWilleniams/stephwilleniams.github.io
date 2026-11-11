---
layout: organism
slug: vibrio-fischeri
title: Vibrio fischeri
summary: Modeling how stress shapes biofilm formation in the squid's bacterial symbiont, and designing experiments that can measure it.
collaborators: Daravuth Cheam, Michele Nishiguchi, Suzanne Sindi, Shilpa Khatri, Erica Rutter
---

## The question

*Vibrio fischeri* (also classified as *Aliivibrio fischeri*) is the bioluminescent partner of the bobtail squid. Ocean flows carry the bacteria to the squid's light organ, where they gather in a symbiotic aggregate, a kind of biofilm, on its surface. They then disperse, swim to the light organ's pores, and are kept for the rest of the squid's life.

Outside the host, the same bacteria have to survive on their own. Under stress, from temperature, pH, oxygen, predators or crowding, *V. fischeri* shifts toward protective phenotypes, often at a cost: stronger biofilm formers tend to be weaker swimmers. That trade-off could change how well the next generation colonizes a squid.

## What I do

With Daravuth Cheam and Prof. Michele Nishiguchi at UC Merced, we expose free-living bacteria to stress over many generations, then test how well they colonize squid. My part is the statistical and mathematical modeling, and the design of the experiments themselves.

Before collecting data, it is worth asking which experiments could actually measure the model's parameters. I analyzed the identifiability of a trait-structured biofilm selection model under predation, and used a genetic algorithm to choose when to sample. Over a 24-hour experiment, 11 optimized time points estimated the biofilm-formation rate more accurately than 51 evenly spaced ones.

## What's next

- Fitting the model to lab-cultured *V. fischeri*, and testing its predictions on hatchlings from field-caught squid.
- Coupling biofilm and motility traits to test which shapes of trade-off can be told apart from evolution data, and what they predict under thermal stress.

## Outputs

- Williams, S., Cheam, D., Nishiguchi, M. K., Sindi, S. S., Khatri, S., Rutter, E. M. Identifiability, sensitivity, and genetic algorithms in bacterial biofilm selection models. *Bull. Math. Biol.* 88, 132 (2026). [Paper](https://doi.org/10.1007/s11538-026-01693-5) · [Code](https://github.com/StephWilleniams/BiofilmModelAnalysis) · [Update]({{ '/updates/identifiability-sensitivity-and-genetic-algorithms-in-bacterial-biofilm-s/' | relative_url }})
- [Interactive: one day of the biofilm selection model]({{ '/interactive/#biofilm-day' | relative_url }})
