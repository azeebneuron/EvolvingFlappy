# EvolvingFlappy

EvolvingFlappy is an intriguing project that merges the classic Flappy Bird game with the innovative NEAT (NeuroEvolution of Augmenting Topologies) algorithm. Witness the autonomous evolution of birds as they learn to navigate through pipes, adapting and improving their strategies across generations.

## Introduction

EvolvingFlappy demonstrates the fascinating concept of evolving artificial intelligence through the NEAT algorithm. Birds in the game evolve their neural networks over generations to master the art of navigating through pipes, bringing a new dimension to the classic Flappy Bird experience.


## Installation

1. **Download:**
    - Download the project zip file or clone the repository:

    ```bash
    git clone https://github.com/Rahul-1337/EvolvingFlappy.git
    cd EvolvingFlappy
    ```

2. **Install Dependencies:**
    - Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage of NEAT in Flappy Bird NEAT

The Flappy Bird NEAT project utilizes the NEAT (NeuroEvolution of Augmenting Topologies) algorithm to autonomously evolve the behavior of birds in navigating through pipes. Here's an overview of how NEAT is used in this project:

1. **Initialization:**
   - NEAT starts with a population of birds, where each bird is represented by a neural network. These neural networks have randomly initialized structures.

2. **Evaluation:**
   - Each bird plays the Flappy Bird game, and its neural network receives inputs (e.g., bird's y-position, distance to pipes) and produces outputs (e.g., flap or not flap).
   - The fitness of each bird is determined based on its performance in the game, considering factors such as distance traveled, pipes passed, and survival time.

3. **Selection:**
   - Birds are selected for reproduction based on their fitness. Higher fitness birds have a higher chance of being selected.
   - NEAT uses "roulette wheel selection" to probabilistically choose individuals for reproduction.

4. **Crossover (Recombination):**
   - Selected birds are paired, and their neural network structures are combined through crossover to create new individuals.
   - Crossover involves exchanging parts of the neural network structures between two parents.

5. **Mutation:**
   - Random mutations are introduced to the offspring's neural network structures. Mutations can include adding or removing nodes and connections, tweaking weights, or other modifications.
   - Mutation helps explore a wider range of possibilities and prevents premature convergence.

6. **Next Generation:**
   - The new individuals (offspring) along with some of the best-performing individuals from the previous generation form the next generation.
   - The process of evaluation, selection, crossover, and mutation is repeated for each generation.

7. **Termination:**
   - The process continues for a specified number of generations or until a termination condition is met (e.g., achieving a certain level of performance).

8. **Best Individual:**
   - The best-performing individual (bird with the highest fitness) is saved for future use. This individual represents the neural network that performed the best in navigating the bird through the pipes.

In summary, NEAT evolves the neural networks controlling the birds, allowing them to learn and improve their ability to play the Flappy Bird game over successive generations.


## Game Features

- **NEAT Algorithm Integration:**
  - Birds use the NEAT algorithm to autonomously evolve over generations.
  - Neural networks guide bird behavior, learning to navigate through pipes.

- **Realistic Flappy Bird Gameplay:**
  - Birds exhibit flapping behavior, and their fitness is based on survival and passing through pipes.

## Customization

Feel free to experiment and customize the game:

- Adjust constants and game settings in `evolving_flappy.py`.
- Fine-tune NEAT parameters in `config.txt` for diverse evolutionary behaviors.



