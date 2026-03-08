# NEAT (Neuroevolution of Augmenting Topologies)

> A Python implementation of NEAT that runs in Google Colab, demonstrating evolution of neural network topologies from scratch.

---

## Overview

This is a Python implementation of NEAT that demonstrates neuroevolution by evolving both network weights and topology. The code outputs generation information and the structure of the best neural networks evolved at each improvement until reaching an optimal solution. Perfect for learning NEAT in an interactive environment.

---

## Features

- **Pure Python Implementation** — No external dependencies for core algorithm
- **Topology Evolution** — Dynamically add and remove network nodes
- **Weight Optimization** — Evolve connection strengths
- **Speciation** — Maintain population diversity through genetic distance
- **Colab-Ready** — Run directly in Google Colab without installation
- **Visualization** — Generation progress and network structure output

---

## How NEAT Works

1. **Start Simple** — Begin with minimal network structure
2. **Evaluate Fitness** — Test networks on a task
3. **Mutate** — Add/remove connections and nodes
4. **Speciate** — Group similar networks together
5. **Crossover** — Combine successful networks
6. **Repeat** — Evolve for multiple generations

The result is a population of increasingly sophisticated networks, discovering both optimal weights and structure.

---

## Getting Started

### Run in Google Colab

The code is designed to run directly in Google Colab without any setup:

1. Open [Google Colab](https://colab.research.google.com)
2. Copy and paste the code into a cell
3. Run and observe evolution progress with network topology changes
4. Monitor generation output showing best network improvements

### Run Locally

```bash
python neat_implementation.py
```

### Requirements

- Python 3.6+
- NumPy (for local execution)

---

## Output

The implementation displays:
- **Generation number** — Current evolution iteration
- **Best fitness** — Highest fitness achieved so far
- **Network topology** — Nodes and connections of best network
- **Progress metrics** — Population statistics

---

## Key Implementation Details

### Genome Representation
- **Connections** — Weighted edges between neurons
- **Nodes** — Neurons that process information
- **Innovation numbers** — Track mutations across generations

### Genetic Operators
- **Add connection** — Link two unconnected neurons
- **Add node** — Split existing connection with new neuron
- **Mutate weight** — Adjust connection strength
- **Remove nodes** — Prune ineffective neurons (optional)

### Speciation
- **Genetic distance** — Measure similarity between genomes
- **Species** — Groups of similar networks
- **Breed within species** — Reduce disruption from crossover

---

## Applications

- Game AI (bot behavior evolution)
- Robot control learning
- Function optimization
- Symbolic regression
- Multi-objective optimization

---

## References

- [Author's Medium Post](https://medium.com/@garybutler4/neat-implementing-my-first-research-paper-b0b0eba795b4) — Journey of implementing NEAT from scratch
- [Original NEAT Paper](http://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf) — Stanley & Miikkulainen
- [NEAT Python Libraries](https://neat-python.readthedocs.io/) — Production-ready NEAT

---

## License

Copyright © Walter Gordy
