---
layout: single
title:  "Quantum Transport Theory"
date:   2022-01-10 10:12:48 +0800
categories: Condensed-Matter-Physics
---
#### Preface

In a semi-classical model, namely the Boltzmann transport theory, we deal with probabilities and rates of electrons motion, instead of their quantum amplitudes. A direct result of this treat is Ohm's law, stating that the ability of a conductor to carry current is parameterized by a local quantity, namely, the conductivity. In this picture, the ability is decided by local properties. 

For example, when two conductors are connected in parallel as below.

![1641873501016](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\1641873501016.png)

The sum of the conductance has a equation as:
$$
G = G_1 + G_2
$$
But from a quantum view, things do not work like this. Electrons are waves, modulated by both conductors. In other words, a single electron can go both conductors. So:

1. We need to sum up the amplitudes of each electron passing through each individual conductor.
2. The motion of electrons are not decided by local properties any more, any change of non-local parameters may contribute to the interference of electrons, thus changing their motion significantly.

This post is to deal with transport from quantum views.

#### Landauer Formula and Conductance Quantization

Consider the configuration below.