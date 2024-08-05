# Central Complex & Insect Navigation

## Sun et al. 2020
- [Link to paper](https://elifesciences.org/articles/73077)
- [Link to Git Repo](https://github.com/XuelongSun/insectNavigationCX)
---
- Applicability of previous computational models across sensory and task domains
- Visual Navigation > Olfactory Navigation
- Co-ordination with other guidance in flies and ants

## Central Complex
- Insect Midbrain
- Co-ordinate guidance strategies
- Markers
    + A head-direction system which tracks current heading relative to external or self motion cues
    + The innervation of the fan-shaped body (FB) region with sensory information relevant to different strategies
    + Well-preserved columnar structure that is well suited to computing desired headings for vector navigation tasks
    + A neural steering circuit in the FB capable of computing motor commands (reducing offset between current heading and desired heading)
- Computational models of this architecture have produced realistic path intergration (PI)
- To be considered a general navigation centre, it must be capable of:
    + Generating gradient ascent/descent behaviours, which rely on spatially varying <b>but </b> rotationally invariant. (e.g. odour gradients)
    + Co-ordinating competing guidance systems into a single meaningful motor command
    + General across sensory modalities and task spaces

## System

#### Overview
- Computational models have produced realistic path integration (PI) and trap-lining behaviours
- A biologically plausible neural copy-and-shift mechanism
- Ensures sensory information is presented in a format compatible with the steering circuit
- Source independancy (Perception, Chemotaxis & Anemotaxis)
- Allow transfer cues from unstable (egocentric) to stable (geocentric) frames of reference
    - Providing a mechanism for foraging insects to recover from environmental disturbances (blown off path)
    - Repurposed by different insect navigators to address their unique ecological needs

#### Neural ‘copy-and-shift’
- The steering circuit could be adapted to ascent gradients of visual familiarity when augmented by the mechanism
- Converts temporal changes in spatially sampled sensory information into an orientation signal.
- The agent will continue on its current heading until a undesired change in sensor valence, at which point the shift mechanism will create an offset between the current and desired headings, causing the steering circuit to initiate a change of direction.

---
    1. Copy the current heading from head-direection cells in the protocerebral bridge (PB). 
    2. At the same time, the signal undergoes a lateral shift in proportion to any undesired change in sensory valance, as measured by the mushroom body (MB) output neurons

- The architechture of the CX already possesses neural substrates ideally suited for both the copy-and-shift functions:
    + (COPY) Head-direction cells are known to transmit their output into the ring structures in the central body
    + (SHIFT) Neural mechanisms that laterally shify head-direction cells in response to sensory feedback (visual or self-motion cues)