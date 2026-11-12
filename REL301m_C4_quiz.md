# REL301m – C4: A Complete Reinforcement Learning System (Capstone) – Quiz Coursera

Nguồn: trang "View feedback" của lượt nộp gần nhất trên Coursera (chỉ đọc, không nộp lượt mới). Câu hỏi/lựa chọn giữ nguyên tiếng Anh; công thức dạng LaTeX `$...$`. `[hình]` = câu có hình minh họa không trích được. Các câu ở lượt cuối bị chấm sai/chưa đủ đã được bổ sung đáp án từ feedback từng lựa chọn của Coursera và/hoặc tự giải; phần tự suy luận được gắn **[Inference]** và có giải thích trong _Ghi chú_.

## Câu 1

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a control setting in which updates will be made at every time step? [Select all that apply]

- A. Expected SARSA
- B. SARSA
- C. Q-learning

**Đáp án đúng: A, B, C**

## Câu 2

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a prediction setting in which updates will be made at the end of each episode? [Select all that apply]

- A. Monte-Carlo Prediction
- B. Exploring Starts Monte-Carlo
- C. Off-Policy Monte-Carlo

**Đáp án đúng: A, C**

## Câu 3

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a tabular setting in which we will be learning a model and using it for planning? [Select all that apply]

- A. Expected SARSA
- B. Dyna-Q
- C. Dyna-Q+

**Đáp án đúng: B, C**

## Câu 4

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a control setting in which we are given access to a model? [Select all that apply]

- A. Iterative Policy Evaluation
- B. Policy Iteration
- C. Value Iteration
- D. Dyna-Q

**Đáp án đúng: B, C, D**

## Câu 5

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a continuing control setting with a discrete action space and function approximation? [Select all that apply]

- A. Gaussian Actor-Critic
- B. Differential Softmax Actor-Critic
- C. Differential Semi-Gradient SARSA

**Đáp án đúng: B, C**

## Câu 6

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in an online prediction setting with linear function approximation? [Select all that apply]

- A. Semi-Gradient TD
- B. Gradient Monte Carlo
- C. SARSA

**Đáp án đúng: A**

## Câu 7

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

In the continuing acrobot system (shown below), a double pendulum is fixed to the red square. The goal is to swing the double pendulum such that the height of the mass on the end of the lower pendulum exceeds the height of the black line. When the goal is reached, a reward of one is given and the double pendulum transitions to a vertical position. Otherwise, the reward is zero. Which of the following algorithms are appropriate for control in this context? [Select all that apply] [hình]

- A. Expected SARSA
- B. Q-learning
- C. Average Reward Actor-Critic

**Đáp án đúng: C**

## Câu 8

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate for control in the lunar lander MDP, as it is described in the lecture “Initial Project Meeting with Martha: Formalizing the Problem”? [Select all that apply]

- A. Expected SARSA
- B. Q-learning
- C. Average Reward Actor-Critic

**Đáp án đúng: A, B**

## Câu 9

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following meta-parameters can be tuned to improve performance of the agent? Performance refers to the cumulative reward the agent would receive in expectation across different runs. (Select all that apply)

- A. Random seed (for the random number generator)
- B. Exploration parameter (e.g., epsilon in e-greedy or the temperature tau in the softmax policy)
- C. The step size in the update rule of the learning algorithm (e.g., alpha in Q-learning)
- D. Number of hidden-layer units in a neural network approximating the value function

**Đáp án đúng: B, C, D**

## Câu 10

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

Suppose a problem that you have formulated as an MDP has k continuous input dimensions. You are considering using tile coding as a function approximator. With T tilings and t tiles per dimension in each tiling, which of the following represent the resultant number of features? (Assume each tiling covers all k dimensions.)

- A. T∙t^k
- B. k∙T^t
- C. T ∙ t / k
- D. T ∙ t ∙ k

**Đáp án đúng: A**

## Câu 11

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements regarding feature-construction methods are TRUE? (Select all that apply)

- A. A simple implementation of tile coding leads to memory requirements that might be exponential in the number of features.
- B. The feature representation obtained using neural networks changes with time.
- C. The feature representation obtained using tile coding changes with time.
- D. In low-dimensional problems, tile coding is computationally efficient and provides good generalization and discrimination.

**Đáp án đúng: A, B, D**

## Câu 12

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Adding more hidden layers (of a fixed finite width) increases the representation capacity of neural network. For example, if you have a single-hidden layer neural network with 16 units and nonlinear activations, then adding another layer of 16 units to get a neural network with two hidden layers can represent more functions.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 13

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Adding more hidden layers to a neural network increases the number of parameters needed to be learned.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 14

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements regarding the exploration approach are TRUE? (Select all that apply)

- A. A softmax policy is a limited strategy for exploration because it can only be used with action preferences and policy-gradient methods.
- B. Optimistic initial values are difficult to maintain when using neural networks as a function approximator.
- C. Epsilon-greedy exploration is difficult to combine with neural networks.
- D. Both optimistic initial values and epsilon-greedy exploration can be easily used with neural networks, because they are simple exploration strategies.

**Đáp án đúng: B**

## Câu 15

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following are TRUE about the softmax temperature parameter tau?

- A. Tau does not affect the exploration at all.
- B. For very small tau, the agent mostly selects the greedy action.
- C. For very large tau, the agent’s policy is nearly a uniformly-random policy.
- D. If tau is large, the agent’s policy is more stochastic.

**Đáp án đúng: B, C, D**

## Câu 16

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements are true about activation functions? (Select all that apply)

- A. The gradient of flat regions in the range of an activation function w.r.t. the input is zero.
- B. Linear activation functions (such as f(x)=x) have derivatives close to zero for inputs of large magnitude.
- C. Rectified Linear Units (ReLUs) are linear activation functions.
- D. For inputs of large magnitude, the derivative of the sigmoid and tanh functions are close to zero.

**Đáp án đúng: A, D**

## Câu 17

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

Consider you are using a neural network to approximate the action-value function of a reinforcement learning agent. You decide to use a neural network with two hidden layers. Now you want to choose the activation function for the hidden layers and the output layer. One option is to use a neural network with tanh activation functions in both hidden layers, and a linear activation in the output layer. Another option is to use a neural network with linear activations in both the hidden layers and the output layer. True or False: In both cases (option one and option two), the neural network can represent the same class of action-value functions.

- A. True
- B. False

**Đáp án đúng: B**

## Câu 18

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements are TRUE regarding methods for selecting a stepsize for the learning update?

- A. A stepsize that reduces over time (such as 1/N, where N is the number of agent-environment interactions) is necessary when the environment changes over time.
- B. An adaptive stepsize selection method like RMSProp uses a heuristic to change the stepsize during learning.
- C. The heuristic to change the stepsize can be learned from the data collected from the agent-environment interactions.

**Đáp án đúng: B, C**

## Câu 19

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Suppose we want to find the optimal policy that obtains the maximum undiscounted return per episode in some task. We are using Expected Sarsa. With the rest of the meta-parameters fixed, we want to find the best setting of the stepsize that results in the best performance in this setting. In the following graph, the blue line represents how the performance measure varies with stepsize. Obviously, we do not have this information beforehand, and we are selecting a range of stepsizes to try out with our agent. Which of the following graphs best represent the range of stepsizes that should be tried out for a given experiment? (the orange points represent the selected stepsizes)

- A. [hình]
- B. [hình]
- C. [hình]

**Đáp án đúng: B**

## Câu 20

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Epsilon-greedy exploration uses information from all the action values of a particular state when choosing a non-greedy action in that state.

- A. False
- B. True

**Đáp án đúng: A**
