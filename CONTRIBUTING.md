# Contributing to Synapse

Synapse started as a solo learning journey, but understanding deepens when it's shared. If you're following along, working through the same ideas, or building intuition for the first time, you're welcome here.

## The spirit of this project

Before contributing, it helps to understand what this repo is *for*. It isn't trying to be the fastest, most production-ready, or most feature-complete implementation of anything. It's trying to be the clearest. A slower, more verbose, more heavily-commented piece of code that builds intuition is worth more here than a clever one-liner that hides what's happening. Keep that in mind for anything you propose.

## Ways to contribute

**Open a discussion.** If something in a notebook doesn't quite click, or you found a way of explaining a concept that helped it land for you, open a discussion. These are often the most valuable contributions — they shape how future sections get written.

**Report something that's broken or unclear.** If a notebook fails to run, a derivation has an error, or an explanation contradicts itself, open an issue. Include which notebook, which cell, and what you expected versus what happened.

**Suggest or add experiments.** Each notebook ends with prompts to break things on purpose. If you tried an experiment that revealed something interesting, write it up and open a pull request — these additions are genuinely welcome.

**Improve intuition sections.** Found a better analogy, a clearer diagram, or a way of framing a concept that made it click faster? These contributions are especially valued, since the whole point of this repo is building understanding, not just running code.

## Before you submit a pull request

A few things that keep this repo consistent:

Code should stay in the established style for its section — plain NumPy and Matplotlib for sections 01–04, with no shortcuts to PyTorch or TensorFlow before section 05. New code should follow the existing object-oriented structure (`Neuron`, `Layer`, `Network`) unless there's a good pedagogical reason to deviate.

Every new concept should follow the same shape as the existing material: intuition first, then math, then code, then experiments. If you're adding a notebook, try to keep that structure even if your section is shorter than the others.

Keep cells runnable on a laptop CPU. Nothing in sections 01–03 should require a GPU, and additions should respect that constraint unless there's a strong reason otherwise (and it should be clearly marked).

## Getting started

1. Fork the repo and clone your fork
2. Create a virtual environment and install dependencies (`pip install numpy matplotlib jupyter`)
3. Make your changes in a new branch
4. Run the notebook end-to-end to make sure it executes cleanly
5. Open a pull request describing what changed and why

## A note on tone

This project is meant to feel approachable, not intimidating. If you're contributing an explanation, write it the way you'd explain it to a friend who's smart but hasn't seen this before — not the way a textbook would. Questions, half-formed ideas, and "I'm not sure if this is right but..." pull requests are all welcome.

Thanks for being here.
