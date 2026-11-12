# REL301m RE

Nguồn: 50 ảnh trong bài đăng Facebook "REL301m RE" (Dơi FPT trùm sp, 09/11/2026). Ảnh không có số câu; thứ tự câu theo thứ tự ảnh trong album. Đáp án do Claude giải theo giáo trình Sutton & Barto / chuỗi khóa Coursera RL và đối chiếu với `SU26.md`, `REL301m - SU25 - RE.md`, bộ quiz Coursera; KHÔNG phải đáp án chính thức. Câu trùng đề cũ ghi rõ nguồn; còn lại gắn [Inference], câu khó/mơ hồ gắn "độ tin cậy thấp" kèm ghi chú. Nội dung câu hỏi giữ nguyên tiếng Anh như trong ảnh.

## Câu 1

What is the main advantage of using linear function approximation in reinforcement learning?

- A. It provides perfect accuracy
- B. It is computationally inexpensive and easy to implement
- C. It ensures convergence to the optimal policy
- D. It eliminates the need for exploration

**Đáp án đúng: B** [Inference]

## Câu 2

In Actor-Critic with Softmax Policies, how is the action chosen based on the softmax probabilities?

- A. The action with the highest probability is chosen
- B. The action is randomly sampled from the distribution
- C. The action with the lowest probability is chosen
- D. The action with the maximum advantage is chosen

**Đáp án đúng: B** [Inference]

## Câu 3

What is the difference between a policy and a value function in an MDP? (choose the best answer)

- A. A policy defines the reward for a state, while a value function defines the action to take.
- B. A policy is a long-term plan, while a value function is a short-term estimate.
- C. A policy defines the agent's behavior, while a value function estimates the desirability of a state or action.
- D. A policy is a mapping from states to actions, while a value function estimates the future rewards from a state.

**Đáp án đúng: D** [Inference – độ tin cậy thấp]

_Ghi chú: C cũng đúng; D là định nghĩa chuẩn hơn (policy: state→action, value: kỳ vọng return)._

## Câu 4

Which algorithm uses the state value function to iteratively improve the policy until it converges to the optimal policy?

- A. Monte Carlo methods
- B. Q-learning
- C. Policy iteration
- D. Temporal Difference learning

**Đáp án đúng: C** [Inference]

## Câu 5

In Q-learning, how is the action value updated for a given state-action pair?

- A. Using the expected return
- B. Using the maximum action value of the next state
- C. Using the discounted reward of the next state
- D. Using the average of all action values

**Đáp án đúng: B** [Inference]

## Câu 6

In reinforcement learning, what is a common downside of pure exploitation without exploration?

- A. Increased computational complexity.
- B. Missing out on potentially better actions that haven't been tried enough.
- C. High variance in reward estimation.
- D. Difficulty in policy convergence to get maximum the total rewards

**Đáp án đúng: B** (trùng đề SU26, cùng đáp án)

## Câu 7

Which of the following methods is NOT used for Policy Evaluation?

- A. Temporal Difference Learning
- B. Monte Carlo methods
- C. Dynamic Programming
- D. Deep Q-Networks

**Đáp án đúng: D** [Inference]

## Câu 8

How is the reward function related to the policy in reinforcement learning?

- A. The reward function determines the optimal policy.
- B. The reward function is irrelevant to the policy based on the value function.
- C. The policy is designed to maximize the cumulative reward based on the reward function.
- D. The policy defines the reward function.

**Đáp án đúng: C** [Inference]

## Câu 9

In the context of Markov Decision Processes (MDPs), what does the Bellman equation help to compute?

- A. The transition probabilities.
- B. The optimal policy.
- C. The reward function.
- D. The state space.

**Đáp án đúng: B** [Inference]

## Câu 10

What does the term "iterative" signify in Iterative Policy Evaluation?

- A. The process involves repeated computation until convergence
- B. It updates the policy in every iteration
- C. It requires iterating through all possible states
- D. It involves iterating through different reinforcement learning algorithms

**Đáp án đúng: A** [Inference]

## Câu 11

What is the purpose of the discount factor (gamma, γ) in reinforcement learning?

- A. To control the learning rate of the agent
- B. To prioritize recent rewards over distant future rewards
- C. To balance exploration and exploitation
- D. To determine the convergence rate of the algorithm

**Đáp án đúng: B** [Inference]

## Câu 12

Which method adjusts the exploration-exploitation balance by dynamically altering the reward estimates based on their uncertainty?

- A. Thompson Sampling
- B. Epsilon-Greedy
- C. Q-Learning
- D. Upper Confidence Bound (UCB)

**Đáp án đúng: D** [Inference]

## Câu 13

If you're preparing for an exam by studying a little bit each day, what type of task is this?

- A. Episodic task.
- B. Continuing task.
- C. Project-based task.
- D. Occasional task.

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Việc học mỗi ngày kéo dài liên tục → continuing; nếu xét có điểm kết thúc (ngày thi) thì A._

## Câu 14

Which algorithm commonly uses the Bellman equation to update the value function?

- A. K-means clustering
- B. Q-learning
- C. Principal Component Analysis (PCA)
- D. Gradient descent

**Đáp án đúng: B** [Inference]

## Câu 15

Which characteristic distinguishes Policy Iteration from other reinforcement learning methods?

- A. It focuses solely on immediate rewards
- B. It disregards the exploration phase
- C. It iteratively improves both policy and value function
- D. None of the above

**Đáp án đúng: C** [Inference]

## Câu 16

Which type of policy directly associates actions with states without using a value function?

- A. Value-based policy
- B. Model-based policy
- C. Policy-based policy
- D. Q-learning policy

**Đáp án đúng: C** [Inference]

## Câu 17

Which of the following is NOT a characteristic of the action-value function?

- A. It depends on both the state and the action.
- B. It can be used to derive the policy.
- C. It only considers the immediate reward.
- D. It is used to estimate the expected return.

**Đáp án đúng: C** [Inference]

## Câu 18

Which of the following statements is true about the SARSA algorithm?

- A. SARSA is an off-policy algorithm.
- B. SARSA always converges to the optimal policy.
- C. SARSA updates the Q-values using the action taken by the policy.
- D. SARSA requires a model of the environment.

**Đáp án đúng: C** [Inference]

## Câu 19

In off-policy Monte Carlo prediction, how is the return corrected?

- A. By averaging all returns without any adjustments
- B. By using the importance sampling ratio
- C. By discarding the returns from the behavior policy
- D. By applying a discount factor

**Đáp án đúng: B** [Inference]

## Câu 20

Which method is commonly used to improve the efficiency of learning in a sample model?

- A. Bootstrapping
- B. Experience replay
- C. Model-free updates
- D. Cross-entropy method

**Đáp án đúng: B** [Inference]

## Câu 21

What is the role of the model in the Dyna architecture?

- A. To replace the environment
- B. To generate random rewards
- C. To simulate transitions for planning
- D. To store past experiences

**Đáp án đúng: C** [Inference]

## Câu 22

Which statistical concept is importance sampling based on?

- A. Central Limit Theorem
- B. Law of Large Numbers
- C. Bayes' Theorem
- D. Markov Chain Monte Carlo

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Importance sampling là ước lượng Monte Carlo, dựa trên Law of Large Numbers._

## Câu 23

In one-step tabular Q-learning, how is the optimal action in a state determined during the learning phase?

- A. By selecting actions randomly
- B. By selecting the action with the highest Q-value
- C. By using a predefined action sequence
- D. By always choosing the first action

**Đáp án đúng: B** [Inference]

## Câu 24

In Q-learning, what does it mean when the Q-values have converged?

- A. The agent continues to explore all possible actions
- B. The Q-values no longer change significantly
- C. The agent stops learning and takes random actions
- D. The agent updates the Q-values for every action

**Đáp án đúng: B** [Inference]

## Câu 25

In which of the following scenarios would TD Prediction be most useful?

- A. When we need to find the optimal policy in a simple grid world.
- B. When we have a large state space and need to estimate the state values for a given policy.
- C. When we want to learn a model of the environment's transition dynamics.
- D. When we need to solve a multi-armed bandit problem.

**Đáp án đúng: B** [Inference]

## Câu 26

Which algorithm is an example of a planning method in reinforcement learning?

- A. Q-learning
- B. Deep Q-Networks (DQN)
- C. Monte Carlo Tree Search (MCTS)
- D. SARSA

**Đáp án đúng: C** [Inference]

## Câu 27

In the Windy Gridworld, what does the wind do to the agent's movement?

- A. It has no effect on the agent's movement.
- B. It pushes the agent downwards.
- C. It pushes the agent upwards as it moves through windy states.
- D. It randomly changes the agent's direction.

**Đáp án đúng: C** [Inference]

## Câu 28

Which of the following best describes an off-policy algorithm?

- A. It optimizes the policy based on past experiences only.
- B. It updates the policy based on the actions taken by the agent.
- C. It learns from actions that are not necessarily taken by the current policy.
- D. It only learns from the actions dictated by the current policy.

**Đáp án đúng: C** [Inference]

## Câu 29

What is the Bellman equation in the context of Q-learning?

- A. It provides the optimal policy directly.
- B. It updates the policy based on rewards received.
- C. It recursively updates the Q-values using the maximum future reward.
- D. It sets the learning rate for the agent.

**Đáp án đúng: C** [Inference]

## Câu 30

Why is it beneficial to update Q-values randomly in Random Tabular Q-planning?

- A. It ensures that all state-action pairs are updated equally.
- B. It helps in better exploration of the state-action space.
- C. It makes the algorithm simpler to implement.
- D. It guarantees convergence to the optimal policy.

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Lấy mẫu ngẫu nhiên cặp (s,a) giúp phủ đều không gian state-action khi planning._

## Câu 31

In importance sampling, what role do importance weights play?

- A. They determine the probability of each sample.
- B. They adjust the contribution of each sample to the estimate.
- C. They control the variance of the estimator.
- D. They are irrelevant in importance sampling.

**Đáp án đúng: B** [Inference]

## Câu 32

What does Temporal Difference offer that traditional learning environments often lack?

- A. Interactive simulations
- B. Passive learning experiences
- C. Inflexible scheduling
- D. Static course content

**Đáp án đúng: A** [Inference – độ tin cậy thấp]

_Ghi chú: Câu không thuộc giáo trình RL (nhiễu); chọn A theo ngữ nghĩa._

## Câu 33

What happens to SARSA's learning rate when the step size parameter (Alpha) is decreased?

- A. It learns faster.
- B. It learns more slowly but may find a better policy.
- C. It has no effect on learning.
- D. It learns the same rate as before.

**Đáp án đúng: B** [Inference]

## Câu 34

What is the main goal of Monte Carlo estimation?

- A. To minimize the number of actions taken
- B. To estimate the value of each state by computing a sample average over returns
- C. To maximize the rewards in a single episode
- D. To create a deterministic policy

**Đáp án đúng: B** [Inference]

## Câu 35

What does an Epsilon greedy policy primarily do?

- A. Always selects the greedy action.
- B. Randomly selects actions without any preference.
- C. Mostly selects the greedy action but occasionally explores randomly.
- D. Ignores the current action value estimates.

**Đáp án đúng: C** [Inference]

## Câu 36

What is the primary difference between Monte Carlo methods and dynamic programming?

- A. Monte Carlo methods require a model of the environment
- B. Dynamic programming learns directly from experience
- C. Monte Carlo methods estimate the value of individual states independently
- D. Dynamic programming does not use episodes

**Đáp án đúng: C** [Inference]

## Câu 37

Why might Expected Sarsa be preferred in an environment with high variance in rewards?

- A. Because it updates the Q-values less frequently.
- B. Because it uses the expected value which smooths out the updates.
- C. Because it disregards the rewards.
- D. Because it focuses only on the maximum reward.

**Đáp án đúng: B** [Inference]

## Câu 38

What is one approach to aggregating states in continuous state spaces?

- A. Using discrete state spaces only.
- B. Clustering states based on feature similarity.
- C. Ignoring state features altogether.
- D. Randomly grouping states.

**Đáp án đúng: B** [Inference]

## Câu 39

How can generalization be reduced in a learning environment?

- A. By reinforcing behaviors inconsistently.
- B. By using a variety of stimuli during training.
- C. By providing specific cues for different responses.
- D. By not reinforcing any behavior.

**Đáp án đúng: C** [Inference]

## Câu 40

Tile Coding is most commonly associated with which type of function approximation in reinforcement learning?

- A. Linear function approximation
- B. Non-linear function approximation
- C. Polynomial function approximation
- D. Radial basis function approximation

**Đáp án đúng: A** [Inference]

## Câu 41

What is the main objective of Actor-Critic algorithms?

- A. To solely maximize the critic's value function
- B. To learn both a policy (actor) and a value function (critic)
- C. To minimize the actor's policy gradient
- D. To eliminate the role of the critic in reinforcement learning

**Đáp án đúng: B** [Inference]

## Câu 42

In which field of study is the estimation of gradients using samples commonly applied?

- A. Quantum physics
- B. Computer graphics
- C. Sociology
- D. Linguistics

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Monte Carlo sampling dùng nhiều trong computer graphics (path tracing)._

## Câu 43

What does the average reward in reinforcement learning represent?

- A. The total reward accumulated during an episode
- B. The reward obtained at each time step
- C. The mean reward received over multiple episodes
- D. The maximum reward achievable in the environment

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Average reward r(π) = reward trung bình mỗi bước thời gian (continuing task)._

## Câu 44

In linear function approximation, the value function is typically represented as a linear combination of:

- A. Rewards
- B. Actions
- C. Features
- D. States

**Đáp án đúng: C** [Inference]

## Câu 45

How does the concept of average reward differ from the concept of cumulative reward?

- A. Average reward considers only the rewards obtained at specific time steps
- B. Cumulative reward is the sum of all rewards received, while average reward is the mean of those rewards
- C. Average reward measures the total reward over all episodes, while cumulative reward measures reward at each time step
- D. They are synonymous and can be used interchangeably

**Đáp án đúng: B** [Inference]

## Câu 46

How does context influence generalization in learning?

- A. Context always limits the ability to generalize.
- B. Similar contexts can enhance the transfer of learning.
- C. Different contexts prevent the application of learned knowledge.
- D. Context has no significant effect on learning outcomes.

**Đáp án đúng: B** [Inference]

## Câu 47

What is the main advantage of using a Gaussian policy in continuous action spaces?

- A. Simplicity of implementation
- B. Ability to handle discrete actions
- C. Smoothness and expressiveness
- D. Faster convergence rate

**Đáp án đúng: C** [Inference]

## Câu 48

Coarse coding can be seen as a form of which of the following in the context of state aggregation?

- A. Clustering
- B. Overfitting
- C. Exact encoding
- D. Model-free learning

**Đáp án đúng: A** [Inference]

## Câu 49

Which algorithm often employs Gaussian policies in reinforcement learning?

- A. Q-Learning
- B. Deep Q-Networks (DQN)
- C. Policy Gradient methods
- D. Temporal Difference Learning

**Đáp án đúng: C** [Inference]

## Câu 50

What is the advantage of using parameterized policies in reinforcement learning?

- A. They are simpler to implement
- B. They provide more flexibility in learning complex behaviors
- C. They converge faster to optimal solutions
- D. They require less computational resources

**Đáp án đúng: B** [Inference]
