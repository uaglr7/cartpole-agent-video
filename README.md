# cartpole-agent-video
This repository documents the training of an **agent based on Deep Q-Learning (DQN)** in the classic `CartPole-v1` environment using Python, TensorFlow, and Gymnasium.  
The project demonstrates how an agent learns to balance a pole on a moving cart through trial and error.

---

## Objective
Train a Deep Q-Network agent capable of solving the **CartPole** task by:
- Interacting with the environment (`CartPole-v1`).
- Learning from experiences using replay memory.
- Gradually improving its performance until the pole remains balanced for 200+ steps.

The results are shown visually with videos **before**, **during**, and **after** training.

---

## Files Included in This Repository

| File | Description |
|------|--------------|
| `RLCartPole-Copy1.ipynb` | The Jupyter Notebook containing all the Python code used to create, train, and test the agent. |
| `HW1_CartPole_Evidence_2001442.pdf` | The report with screenshots of the training process, results, and links to the demonstration videos. |

> The notebook includes a full DQN implementation with Keras, memory replay, epsilon decay, and performance graphs.

---

## Videos of the Agent

The following videos show the **evolution of the agent**:

| Phase | Description |
|-------|--------------|------|
| **Before Training** | The agent moves randomly, and the pole falls quickly. | 
| **During Training** | Shows the neural network improving through multiple episodes. |
| **After Training** | The trained agent keeps the pole balanced successfully. |
| **Full Video** | A complete edited clip with all three stages. | 

---

## Technical Details

- **Environment:** `CartPole-v1` (Gymnasium)
- **Algorithm:** Deep Q-Network (DQN)
- **Libraries used:**
  - `TensorFlow / Keras`
  - `Gymnasium`
  - `NumPy`
  - `Matplotlib`
- **Key hyperparameters:**
  - Learning rate: `0.001`
  - Discount factor (gamma): `0.95`
  - Epsilon decay: `0.995`
  - Memory size: `2500`

The agent uses **experience replay** and an **epsilon-greedy policy** to explore and exploit efficiently.

---

## Results Summary

- The agent starts with random actions and low rewards.
- After several episodes, rewards increase steadily.
- Eventually, the pole stays balanced for ~200 time steps (the problem is considered *solved*).
- The reward curve and epsilon decay are plotted to visualize learning progression.

---

## Author

**Enrique Uriel Aguilar Flores**  
*4th Year Software Engineering Student at UANL*  
Monterrey, Nuevo León, México  
November 2025  

---

## Acknowledgements

The original CartPole DQN notebook and base code were created by **Professor Dr. José Arturo Berrones Santos** as part of the course materials.  
This repository contains my execution, modifications, analysis, and recordings demonstrating the agent’s performance.

## License

This repository is released for **educational purposes**.  
Feel free to fork, modify, and learn from it.  
All rights to the original dataset and environment belong to **OpenAI Gym / Gymnasium**.
