# 🚂💨 The Numerical Train is Getting Heated Up
### Team Mirzakhani — MAT 433, Spring 2026
**Arav · Aziza · E · Essey · Monica · Ruben**

---

## Welcome Aboard!

Imagine you just stepped onto a train on a perfectly mild spring day. The weather outside
is totally fine — nothing extreme, nothing dramatic. But somehow, halfway through the ride,
you find yourself either sweating or reaching for your jacket.

This is actually a real engineering problem! Modern electric trains use automated
climate-control systems to keep passengers comfortable, but these systems are working in
a constantly changing environment. Doors open and close at every stop, passengers come and
go, and the outside temperature drifts throughout the journey. The system has to
*continuously predict* how the interior temperature is going to evolve and adjust
accordingly — and sometimes it does not get it quite right.

**So here is the question we are trying to answer:**

>  *Can noticeable temperature swings happen inside a train carriage even when the
> outside temperature seems perfectly mild and stable?*

To answer this, we are going to build mathematical models from scratch using the tools
we have developed in MAT 433 combined with our own research.

---

## What is in This Repo?

This Repo is the computational engine behind our paper.
Here is the roadmap:

| Section | What We Do |
|---|---|
| **Task 1** | Take 299 discrete outside temperature readings and build a smooth, continuous function $\theta(t)$ from them using interpolation |
| **Task 2** | Use $\theta(t)$ to model the interior temperature $T(t)$ with a first-order ODE, solved numerically using Forward Euler |
| **Task 3** | Upgrade the model with thermal inertia — a second-order ODE that makes the system respond more realistically |
| **Task 4** | Compute the thermal exposure $E = \int |T(t) - 72| \, dt$, a single number that captures how uncomfortable the ride was |

---

## A Few Things to Know Before You Run

- All three datasets are loaded at the top. Each one represents a different outside
  temperature scenario — one mild, one gradually cooling, one dropping dramatically.
- Our comfort temperature is $T_c = 72^\circ$F throughout.
- There are a ton of colors for graphs and such data.
- If you are running this for the first time, just hit **Runtime → Run All** and
  everything will generate automatically.

Let's go!

---
