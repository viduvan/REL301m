# REL301M_SP26_FE

Nguồn: 50 ảnh trong bài đăng Facebook "REL301M_SP26_FE" (Dơi FPT trùm sp, 09/11/2026), số câu theo nhãn "Multiple Choice Question N" trên ảnh. Đáp án do Claude giải theo giáo trình Sutton & Barto / chuỗi khóa Coursera RL và đối chiếu với `SU26.md`, `REL301m - SU25 - RE.md`, bộ quiz Coursera; KHÔNG phải đáp án chính thức. Câu trùng đề cũ ghi rõ nguồn; còn lại gắn [Inference], câu khó/mơ hồ gắn "độ tin cậy thấp" kèm ghi chú. Nội dung câu hỏi giữ nguyên tiếng Anh như trong ảnh.

## Câu 1

What is the key objective of using a Temporal Difference (TD) learning algorithm? (choose the best answer/core idea of TD learning)

- A. To estimate the value of a state based on the complete return from a full episode.
- B. To update the value function by using the difference between successive state values.
- C. To learn the optimal value function without requiring a model of the environment's dynamics.
- D. To approximate the total return by bootstrapping from the immediate reward and the estimated value of the next state.

**Đáp án đúng: D** [Inference]

## Câu 2

Which of the following methods is associated with distribution models for handling uncertainty in state transitions?

- A. Markov Decision Processes (MDPs)
- B. Policy Gradient Methods
- C. Particle Filters
- D. Q-Learning

**Đáp án đúng: A** [Inference]

## Câu 3

Which of the following is a key benefit of using Dyna Architecture?

- A. Reduced computational resources
- B. Increased data redundancy
- C. Improved model scalability and adaptability
- D. Simplified system design

**Đáp án đúng: C** [Inference]

## Câu 4

What is the relationship between sample efficiency and sample-based models?

- A. Sample-based models are more sample-efficient than distribution models
- B. Sample-based models are generally less sample-efficient than distribution models
- C. Both types of models have the same sample efficiency
- D. Sample efficiency is not a concern in reinforcement learning

**Đáp án đúng: A** [Inference – độ tin cậy thấp]

_Ghi chú: Đề do AI sinh, đáp án chưa rõ; B (distribution model hiệu quả mẫu hơn) cũng có lý._

## Câu 5

What does the exploration in Gaussian policies rely on?

- A. Random noise added to the mean action
- B. Random sampling from a uniform distribution
- C. Fixed exploration rate
- D. Adaptive exploration based on reward feedback

**Đáp án đúng: A** [Inference]

## Câu 6

Which factor influences the stability of policy gradient algorithms during training?

- A. Learning rate
- B. Discount factor
- C. Exploration rate
- D. Entropy regularization

**Đáp án đúng: A** (trùng đề SU26, cùng đáp án)

## Câu 7

Which of the following algorithms is commonly used in reinforcement learning?

- A. k-Nearest Neighbors
- B. Q-Learning
- C. Principal Component Analysis
- D. Decision Trees

**Đáp án đúng: B** [Inference]

## Câu 8

What is a potential disadvantage of using Expected Sarsa over Sarsa?

- A. It tends to have higher variance in updates
- B. It requires knowledge of the policy's action probabilities
- C. It converges more slowly than Sarsa
- D. It cannot be used in online learning settings

**Đáp án đúng: B** [Inference]

## Câu 9

In the sample average method, what does the step size parameter determine?

- A. The total number of actions taken
- B. The influence of the most recent reward on the estimate
- C. The number of ads to display
- D. The initial value of Q

**Đáp án đúng: B** [Inference]

## Câu 10

Which technique is commonly used to reduce the variance of policy gradient estimates?

- A. Actor-Critic methods
- B. Temporal Difference learning
- C. Monte Carlo Tree Search
- D. Model-based reinforcement learning

**Đáp án đúng: A** [Inference]

## Câu 11

What is the primary purpose of the state value function in reinforcement learning?

- A. To determine the probability of taking a certain action
- B. To estimate the future rewards from a given state
- C. To record the history of visited states
- D. To minimize the error rate of predictions

**Đáp án đúng: B** [Inference]

## Câu 12

What is the main challenge associated with using parameterized policies in reinforcement learning?

- A. They are computationally expensive
- B. They often lead to overfitting
- C. They require a large amount of training data
- D. They can suffer from local optima

**Đáp án đúng: D** [Inference]

## Câu 13

What is the advantage of using a higher number of sample points in estimating the gradient?

- A. Increased accuracy
- B. Decreased computation time
- C. Reduced memory usage
- D. Smaller margin of error

**Đáp án đúng: A** [Inference]

## Câu 14

Which statement best describes Tabular Temporal Difference (TD) learning?

- A. It uses a table to store values for each state-action pair.
- B. It uses function approximation to estimate value functions.
- C. It updates values based on rewards and state transitions without using tables.
- D. It requires the exact model of the environment.

**Đáp án đúng: A** [Inference]

## Câu 15

What does the Q-Learning update do in the context of planning?

- A. It generates new states.
- B. It improves the policy based on updated action values.
- C. It eliminates the need for a model.
- D. It only focuses on real-world experiences.

**Đáp án đúng: B** [Inference]

## Câu 16

In expected Sarsa, the weights used in the expectation calculation are based on:

- A. The rewards received
- B. The probability of taking each action under the agent's policy
- C. The number of actions available
- D. The current state of the environment

**Đáp án đúng: B** [Inference]

## Câu 17

Which algorithm is commonly used to solve an MDP?

- A. K-means clustering
- B. Breadth-first search
- C. Value iteration
- D. Gradient descent

**Đáp án đúng: C** [Inference]

## Câu 18

What is a common approach to reduce the variance in Monte Carlo estimates?

- A. Using a discount factor.
- B. Using importance sampling.
- C. Using eligibility traces.
- D. Using linear function approximation.

**Đáp án đúng: C** [Inference – độ tin cậy thấp]

_Ghi chú: Eligibility traces/TD(λ) giảm phương sai so với MC thuần; importance sampling thường làm TĂNG phương sai._

## Câu 19

In contrast to Dynamic Programming and Monte Carlo methods, what aspect makes Temporal Difference(TD) methods more suitable for online learning?

- A. TD methods are slower to update values.
- B. TD methods require extensive computational resources.
- C. TD methods update values based on incomplete sequences.
- D. TD methods are less flexible in adapting to changing environments.

**Đáp án đúng: C** [Inference]

## Câu 20

What is the Bellman equation used for in the context of MDPs?

- A. To determine the optimal policy.
- B. To update the value function.
- C. To calculate the transition probabilities.
- D. To find the immediate reward.

**Đáp án đúng: B** [Inference – độ tin cậy thấp]

_Ghi chú: Bellman equation dùng để tính/cập nhật value function; A cũng có thể được chấp nhận._

## Câu 21

In the context of linear function approximation, what is the gradient of the value function approximation?

- A. The true value of the state
- B. The feature vector in that state
- C. The mean squared error
- D. The policy value

**Đáp án đúng: B** [Inference]

## Câu 22

Which phase of Policy Iteration involves updating the policy based on the current value function?

- A. Policy Evaluation
- B. Policy Improvement
- C. Policy Initialization
- D. Policy Iteration

**Đáp án đúng: B** [Inference]

## Câu 23

In the context of function approximation, what does Mu of S represent?

- A. The total number of states
- B. The probability distribution of state visits
- C. The error in value function approximation
- D. The learning rate of the algorithm

**Đáp án đúng: B** [Inference]

## Câu 24

What does the term "off-policy" refer to in the context of Expected Sarsa?

- A. Learning from actions that are not taken by the agent.
- B. Learning from actions that are taken by the agent.
- C. Learning without any prior knowledge of the environment.
- D. Learning that does not depend on the current policy.

**Đáp án đúng: A** [Inference – độ tin cậy thấp]

_Ghi chú: Expected Sarsa lấy kỳ vọng trên mọi action (kể cả action agent không chọn)._

## Câu 25

What is the Bellman equation used for in the context of MDPs?

- A. To calculate the shortest path between states.
- B. To update the policy in reinforcement learning.
- C. To express the relationship between the value of a state and the values of its successor states.
- D. To compute the transition probabilities between states to get maximum rewards

**Đáp án đúng: C** [Inference]

## Câu 26

What distinguishes Temporal Difference (TD) methods from Monte Carlo methods regarding the handling of incomplete episodes?

- A. TD methods require complete episodes for updating values.
- B. TD methods update values based on incomplete episodes.
- C. TD methods cannot handle incomplete episodes efficiently.
- D. TD methods do not rely on experiences for learning.

**Đáp án đúng: B** (trùng đề SU25 RE, cùng đáp án)

## Câu 27

Which problem arises due to the use of linear function approximation in reinforcement learning?

- A. Overfitting
- B. Curse of dimensionality
- C. Underfitting
- D. Vanishing gradients

**Đáp án đúng: C** [Inference – độ tin cậy thấp]

_Ghi chú: Linear FA có năng lực biểu diễn hạn chế → underfitting._

## Câu 28

In the context of Temporal Difference (TD), Which of the following is NOT a step in the TD(0) algorithm?

- A. Prediction
- B. Evaluation
- C. Backpropagation
- D. Bootstrapping

**Đáp án đúng: C** [Inference]

## Câu 29

What is the primary purpose of Dyna Architecture?

- A. To develop operating systems
- B. To design scalable web servers
- C. To model complex dynamic systems
- D. To manage database transactions

**Đáp án đúng: C** (trùng đề SU25 RE, cùng đáp án)

## Câu 30

Which of the following is a key component of Monte Carlo simulations?

- A. Deterministic algorithms
- B. Random sampling
- C. Fixed input values
- D. Analytical solutions

**Đáp án đúng: B** [Inference]

## Câu 31

In reinforcement learning, the state value function V(s) represents:

- A. The immediate reward received after taking an action in state s
- B. The total accumulated reward from state s
- C. The expected return starting from state s
- D. The likelihood of transitioning from state s to another state

**Đáp án đúng: C** [Inference]

## Câu 32

What is the main purpose of using optimistic initial values in function approximation?

- A. To ensure faster convergence
- B. To encourage exploration
- C. To minimize errors
- D. To guarantee optimal solutions

**Đáp án đúng: B** [Inference]

## Câu 33

In the Monte Carlo prediction method, what is the purpose of using the policy π?

- A. To determine the sequence of states
- B. To generate episodes
- C. To update the value function
- D. To ensure convergence of the algorithm

**Đáp án đúng: B** [Inference]

## Câu 34

What does the term "semi-gradient" refer to in the context of linear semi-gradient Temporal Difference learning?

- A. Using gradients to update the table values.
- B. Approximating gradients using a non-linear function.
- C. Using part of the gradient information to update parameters.
- D. Calculating exact gradients for function updates.

**Đáp án đúng: C** [Inference]

## Câu 35

In reinforcement learning, what does a stochastic policy do?

- A. Selects actions randomly with equal probability
- B. Selects the same action for a given state every time
- C. Selects actions based on a probability distribution
- D. Does not select any action

**Đáp án đúng: C** [Inference]

## Câu 36

What does the term "greedification" refer to in the context of policy improvement?

- A. Making a policy more random
- B. Selecting actions that maximize the value function
- C. Evaluating the performance of a policy
- D. Following the original policy without changes

**Đáp án đúng: B** [Inference]

## Câu 37

Which of the following is NOT a typical component of a reinforcement learning model?

- A. State transition probabilities
- B. Reward function
- C. Policy network
- D. Action space

**Đáp án đúng: C** [Inference]

## Câu 38

In an experiment, a pigeon is trained to peck a key when it sees a red light but not when it sees a green light. This is an example of:

- A. Generalization
- B. Spontaneous recovery
- C. Discrimination
- D. Habituation

**Đáp án đúng: C** [Inference]

## Câu 39

How many components does the feature vector have when there are four features and three actions in a stacked representation?

- A. 4
- B. 7
- C. 12
- D. 16

**Đáp án đúng: C** [Inference]

## Câu 40

In policy iteration, what is the role of the policy evaluation step?

- A. To improve the policy based on current estimates of the value function
- B. To randomly update the policy
- C. To compute the value function of the current policy
- D. To explore different policies without updating them

**Đáp án đúng: C** [Inference]

## Câu 41

Which of the following exploration strategies is commonly used with SARSA?

- A. Softmax action selection
- B. Upper Confidence Bound (UCB)
- C. Epsilon-greedy
- D. Boltzmann exploration

**Đáp án đúng: C** [Inference]

## Câu 42

What advantage does Tile Coding provide compared to a single large lookup table?

- A. Increased computational speed
- B. Reduced overfitting
- C. More memory efficiency
- D. Higher resolution of state representation

**Đáp án đúng: C** [Inference]

## Câu 43

Which type of reinforcement learning model typically uses Monte Carlo simulations to estimate values?

- A. Sample-based models
- B. Distribution models
- C. Both sample-based and distribution models
- D. Neither sample-based nor distribution models

**Đáp án đúng: A** [Inference]

## Câu 44

In Policy Iteration, which step involves evaluating the current policy's performance and updating the value function?

- A. Policy Evaluation
- B. Policy Improvement
- C. Policy Initialization
- D. Policy Iteration

**Đáp án đúng: A** [Inference]

## Câu 45

Which of the following is a primary characteristic of a distribution model in reinforcement learning?

- A. It directly samples actions based on a policy.
- B. It approximates the transition dynamics of the environment.
- C. It only updates after the entire episode ends.
- D. It requires a deterministic policy.

**Đáp án đúng: B** [Inference]

## Câu 46

Which term describes a methodical approach to handling episodic tasks?

- A. Ad hoc management
- B. Reactive management
- C. Proactive management
- D. Time-blocking

**Đáp án đúng: C** [Inference – độ tin cậy thấp]

_Ghi chú: Câu không thuộc giáo trình RL; chọn theo nghĩa "methodical/proactive"._

## Câu 47

Which term describes the probability distribution over next states given a current state and action in an MDP?

- A. Policy
- B. Reward function
- C. Transition model
- D. Value function

**Đáp án đúng: C** [Inference]

## Câu 48

What is the purpose of the accumulated product of important sampling ratios (W) in the off-policy Monte Carlo prediction algorithm?

- A. To store all past values of Rho
- B. To correct the returns generated by the behavior policy
- C. To calculate the average reward
- D. To simplify the algorithm

**Đáp án đúng: B** [Inference]

## Câu 49

What is the advantage of using policy gradient methods over value-based methods like Q-learning?

- A. Better convergence guarantees
- B. Simpler implementation
- C. More efficient memory usage
- D. Ability to handle continuous action spaces

**Đáp án đúng: D** [Inference]

## Câu 50

What differentiates off-policy Q-learning from on-policy methods like SARSA?

- A. Q-learning uses past experiences while SARSA uses future predictions.
- B. Q-learning updates using the highest Q-value of the next state, while SARSA updates using the action actually taken.
- C. Q-learning requires a model of the environment, while SARSA does not.
- D. Q-learning is based on deterministic policies, while SARSA is based on stochastic policies.

**Đáp án đúng: B** [Inference]
