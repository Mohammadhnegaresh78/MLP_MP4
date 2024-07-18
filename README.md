Machine Learning Course

Overview
Welcome to the Machine Learning Course offered by Dr. Aliyari at K. N. Toosi University of Technology! This course covers a wide range of topics in machine learning, providing you with the knowledge and skills necessary to understand and apply various machine learning algorithms.

📘 Course Overview
In this course, we will dive deep into the exciting field of machine learning. You'll learn the fundamentals of machine learning, explore various algorithms, and gain practical experience through hands-on assignments and projects.


📁 Mini Project 4

Mini Project 4: Deep Reinforcement Learning for Lunar Lander
Overview
This project aims to apply deep reinforcement learning techniques, specifically DQN and DDQN, to solve the Lunar Lander environment from OpenAI Gym. The project explores the effects of different batch sizes on agent performance and compares the efficiency of DQN and DDQN algorithms.



Table of Contents
Introduction
Project Structure
Environment Details
Methodology
Deep Q-Learning (DQN)
Double Deep Q-Learning (DDQN)
Results
Batch Size Comparison
DQN vs DDQN
Conclusion
References
Introduction
The Lunar Lander environment involves controlling a spacecraft to land safely on a designated landing pad. The agent must learn to navigate the lander using thrusters to control its horizontal and vertical velocities while considering the spacecraft's angle and leg contact with the ground.

Project Structure
Code: Implementation of the DQN and DDQN agents.
Reports: Detailed analysis and results of the experiments.
Notebooks: Jupyter notebooks containing code and explanations.
Videos: Recordings of the agent's performance during training.
Environment Details
State Space: 8-dimensional continuous space representing the lander's position, velocity, angle, and leg contact.
Action Space: 4 discrete actions:
Do nothing
Fire main engine
Fire left engine
Fire right engine
Reward System:
+100 to +140 points for landing
-100 points for crashing
+10 points for each leg contact
-0.03 points for firing the main engine
-0.1 points for each frame without termination
Methodology
Deep Q-Learning (DQN)
DQN uses a neural network to approximate the Q-value function, which represents the expected future rewards for each action given a state. The agent interacts with the environment and stores experiences in a replay buffer. The neural network is trained using mini-batches sampled from the replay buffer to break the correlation between consecutive experiences.

Double Deep Q-Learning (DDQN)
DDQN addresses the overestimation bias in Q-learning by using two networks: a value network and a target network. The value network is used to select actions, while the target network is used to evaluate them. This decoupling helps in providing more accurate value estimates.

Results
Batch Size Comparison
We experimented with three batch sizes: 32, 64, and 128. The results are as follows:

Batch Size 32: Shows significant initial volatility but stabilizes over time.
Batch Size 64: Provides a good balance between stability and learning speed.
Batch Size 128: Exhibits the highest stability and fastest convergence but may be slower in individual updates.
DQN vs DDQN
DQN: Prone to overestimation bias, which can lead to suboptimal policies.
DDQN: More stable and provides better performance by mitigating the overestimation bias.
Conclusion
Through this project, we demonstrated the application of DQN and DDQN algorithms in the Lunar Lander environment. DDQN outperforms DQN by providing more accurate value estimates, leading to better policy learning. The batch size significantly impacts the training stability and convergence speed, with larger batch sizes generally performing better.

References
OpenAI Gym
Stable Baselines3
Deep Q-Learning Paper
Double Q-Learning Paper
For detailed code implementation and analysis, please refer to the Jupyter notebooks and reports provided in this repository. The video recordings of the agent's performance are also available for a visual understanding of the training process.


🚩 Getting Started
To get started with the course, follow these steps:

Clone or fork this repository to your local machine.
Review the course materials in the respective directories.
Complete the assignments and projects as instructed.
Engage in discussions and ask questions in the course's Issues section.
Stay updated with course announcements and updates by watching this repository.
Setup Instructions
Clone the Repository
Clone the repository to your local machine using the following command:

git clone https://github.com/alirezarezaeei78/machine-learning-course.git
cd machine-learning-course
Install Required Packages
Install the required Python packages using pip:

pip install -r requirements.txt
Launch Jupyter Notebook
Start Jupyter Notebook to access the project's notebooks:

jupyter notebook
📜 Code of Conduct Please review and adhere to our Code of Conduct to create a respectful and inclusive learning environment for everyone.

📄 License This course repository is open-source and available under the MIT License. You are free to use, modify, and share the content, but please provide proper attribution.

📞 Contact If you have questions or need assistance, you can reach out to the course instructor:

Email: negaresh1378@gmail.com
