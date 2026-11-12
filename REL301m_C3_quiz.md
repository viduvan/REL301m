# REL301m – C3: Prediction and Control with Function Approximation – Quiz Coursera

Nguồn: trang "View feedback" của lượt nộp gần nhất trên Coursera (chỉ đọc, không nộp lượt mới). Câu hỏi/lựa chọn giữ nguyên tiếng Anh; công thức dạng LaTeX `$...$`. `[hình]` = câu có hình minh họa không trích được. Các câu ở lượt cuối bị chấm sai/chưa đủ đã được bổ sung đáp án từ feedback từng lựa chọn của Coursera và/hoặc tự giải; phần tự suy luận được gắn **[Inference]** và có giải thích trong _Ghi chú_.

## Câu 1

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following statements is true about function approximation in reinforcement learning? (Select all that apply)

- A. It allows faster training by generalizing between states.
- B. We only use function approximation because we have to for large or continuous state spaces. We would use tabular methods if we could, and learn an independent value per state.
- C. It can be more memory efficient.
- D. It can help the agent achieve good generalization with good discrimination, so that it learns faster and represent the values quite accurately.

**Đáp án đúng: A, C, D**

## Câu 2

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

We learned how value function estimation can be framed as supervised learning. But not all supervised learning methods are suitable. What are some characteristics of reinforcement learning that can make it harder to apply standard supervised learning methods?

- A. Data is available as a fixed batch.
- B. Data is temporally correlated in reinforcement learning.
- C. When using bootstrapping methods like TD, the target labels change.

**Đáp án đúng: B, C**

## Câu 3

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

Value Prediction (or Policy Evaluation) with Function Approximation can be viewed as supervised learning mainly because _________. [choose the most appropriate completion of the proceeding statement]

- A. Each state and its target (used in the Monte Carlo update, TD(0) update, and DP update) forms an input-output training example which we can use to train our approximation to the value function
- B. We use stochastic gradient descent to learn the value function.
- C. We can learn the value function by training with batches of data obtained from the agent’s interaction with the world.

**Đáp án đúng: A**

## Câu 4

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about using Mean Squared Value Error ( $\bar{VE} = \sum \mu(s) [v_\pi(s) - \hat{v}(s,w)]^2$ ) as the prediction objective? $\mu(s)$ represents the weighted distribution of visited states(Select all that apply)

- A. Even if the agent uses a linear representation that cannot represent the true values, the agent can still get zero MSVE.
- B. Gradient Monte Carlo with linear function approximation converges to the global optimum of this objective, if the step size is reduced over time.
- C. The agent can get zero MSVE when using a tabular representation that can represent the true values.
- D. This objective makes it explicit how we should trade-off accuracy of the value estimates across states, using the weighting $\mu$ .

**Đáp án đúng: B, C, D**

## Câu 5

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about $\mu(S)$ in Mean Squared Value Error? (Select all that apply)

- A. It serves as a weighting to minimize the error more in states that we care about.
- B. It is a probability distribution.
- C. If the policy is uniformly random, $\mu(S)$ would have the same value for all states.
- D. It has higher values for states that are visited more often.

**Đáp án đúng: A, B, D**

## Câu 6

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

The stochastic gradient descent update for the MSVE would be as follows.Fill in the blanks (A), (B), (C ) and (D) with correct terms. (Select all correct answers) $\mathbf{w_{t+1}} \doteq \mathbf{w_t} \hspace{0.25em} (A) \hspace{0.25em} \frac{1}{2}\alpha \nabla [\hspace{0.25em} (C) \hspace{0.25em} - \hspace{0.25em} (D)\hspace{0.25em} ]^2$ $\quad\quad = \mathbf{w_t} \hspace{0.25em} (B) \hspace{0.25em} \alpha [\hspace{0.25em} (C) \hspace{0.25em} - \hspace{0.25em} (D)\hspace{0.25em} ] \nabla \hat{v}(S_t,\mathbf{w_t})$ $(\alpha > 0)$

- A. $+, -, v_\pi(S_t), \hat{v}(S_t, \mathbf{w_t})$
- B. $-, -, \hat{v}(S_t, \mathbf{w_t}), v_\pi(S_t)$
- C. $-, +, v_\pi(S_t), \hat{v}(S_t, \mathbf{w_t})$
- D. $+, +, \hat{v}(S_t, \mathbf{w_t}), v_\pi(S_t)$

**Đáp án đúng: B, C** [Inference]

_Ghi chú: Coursera xác nhận D sai (feedback: update tỉ lệ với gradient âm của bình phương sai số). w − ½α∇[v_π − v̂]² = w + α[v_π − v̂]∇v̂ (C). Đảo thứ tự trong ngoặc vuông cũng cho kết quả tương đương: w − α[v̂ − v_π]∇v̂ (B)._

## Câu 7

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

In a Monte Carlo Update with function approximation, we do stochastic gradient descent using the following gradient: $\nabla[G_t - \hat{v}(s,\mathbf{w})]^2 = 2 [G_t - \hat{v}(s, \mathbf{w})]\nabla (-\hat{v}(S_t, \mathbf{w}_t))$ $\quad\quad\quad\qquad\quad= (-1)*2 [G_t - \hat{v}(s, \mathbf{w})]\nabla \hat{v}(S_t, \mathbf{w}_t)$ But the actual Monte Carlo Update rule is the following: $\mathbf{w_{t+1}} = \mathbf{w_t} + \hspace{0.25em} \alpha [G_t - \hat{v}(S_t, \mathbf{w}_t) ] \nabla \hat{v}(S_t, \mathbf{w}_t), \quad\quad (\alpha >0)$ Where did the constant -1 and 2 go when $\alpha$ is positive? (Choose all that apply)

- A. We assume that the 2 is included in $\nabla \hat{v}(S_t, \mathbf{w}_t)$ .
- B. We are performing gradient descent, so we subtract the gradient from the weights, negating -1.
- C. We are performing gradient ascent, so we subtract the gradient from the weights, negating -1.
- D. We assume that the 2 is included in the step-size.

**Đáp án đúng: B, D**

## Câu 8

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

When using stochastic gradient descent for learning the value function, why do we only make a small update towards minimizing the error instead of fully minimizing the error at each encountered state?

- A. Because we want to minimize approximation error for all states, proportionally to $\mu$ .
- B. Because small updates guarantee we can slowly reduce approximation error to zero for all states.
- C. Because the target value may not be accurate initially for both TD(0) and Monte Carlo method.

**Đáp án đúng: A**

## Câu 9

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

The general stochastic gradient descent update rule for state-value prediction is as follows: $\mathbf{w_{t+1}} \doteq \mathbf{w_t} + \alpha [U_t - \hat{v}(S_t, \mathbf{w_t})] \nabla \hat{v}(S_t,\mathbf{w_t})$ For what values of $U_t$ would this be a semi-gradient method?

- A. $v_\pi(S_t)$
- B. $R_{t+1} + \hat{v}(S_{t+1}, w_t)$
- C. $R_{t+1} + R_{t+2} + … + R_T$
- D. $G_t$

**Đáp án đúng: B**

## Câu 10

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following statements is true about state-value prediction using stochastic gradient descent? $\mathbf{w_{t+1}} \doteq \mathbf{w_t} + \alpha [U_t - \hat{v}(S_t, \mathbf{w_t})] \nabla \hat{v}(S_t,\mathbf{w_t})$ (Select all that apply)

- A. Using the Monte Carlo return as target, and under appropriate stochastic approximation conditions, the value function will converge to a local optimum of the Mean Squared Value Error.
- B. Using the Monte Carlo return or true value function as target results in an unbiased update.
- C. When using $U_t = R_{t+1} +\hat{v}(S_{t+1},\mathbf{w_t})$ , the weight update is not using the true gradient of the TD error.
- D. Stochastic gradient descent updates with Monte Carlo targets always reduce the Mean Squared Value Error at each step.
- E. Semi-gradient TD(0) methods typically learn faster than gradient Monte Carlo methods.

**Đáp án đúng: A, B, C, E**

_Ghi chú: Coursera xác nhận A, C, E đúng và báo còn thiếu đáp án. D sai vì SGD không "always" giảm MSVE ở mỗi bước, nên đáp án còn thiếu là B (MC return / true value là target không chệch) [Inference]._

## Câu 11

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about the TD fixed point? (Select all correct answers)

- A. Semi-gradient TD(0) with linear function approximation converges to the TD fixed point.
- B. The weight vector corresponding to the TD fixed point is a local minimum of the Mean Squared Value Error.
- C. The weight vector corresponding to the TD fixed point is the global minimum of the Mean Squared Value Error.
- D. At the TD fixed point, the mean squared value error is not larger than $\frac{1}{1-\gamma}$ times the minimal mean squared value error, assuming the same linear function approximation.

**Đáp án đúng: A, D**

## Câu 12

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about Linear Function Approximation, for estimating state-values? (Select all that apply)

- A. The size of the feature vector is not necessarily equal to the size of the weight vector.
- B. The gradient of the approximate value function $\hat{v}(s, \mathbf{w})$ with respect to $\mathbf{w}$ is just the feature vector.
- C. State aggregation is one way to generate features for linear function approximation.

**Đáp án đúng: B, C**

## Câu 13

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about coarse coding? (Select all that apply)

- A. In coarse coding, generalization occurs between states that have features with overlapping receptive fields.
- B. In coarse coding, generalization between states depend on the size and shape of the receptive fields.
- C. When using features with large receptive fields, the function approximator cannot make discriminations that are finer than the width of the receptive fields.
- D. When training at one state, the learned value function will be updated over all states within the intersection of the receptive fields.

**Đáp án đúng: A, B**

_Ghi chú: Coursera xác nhận A, B đúng; C, D "should not be selected". Độ phân giải tăng được khi thêm feature; khi train, value được cập nhật trên hợp (union) các receptive field, không phải giao (intersection)._

## Câu 14

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Consider a continuous two-dimensional state space. Assuming linear function approximation with the coarse-codings in either A, B or C, which of the following is TRUE? (Select all that apply) [hình]

- A. Generalization is broader in case A as compared to case B.
- B. In case B, when updating the state marked by an ‘x’ , the value function will be affected for a larger number of states as compared to case A.
- C. In case C, each update results in more generalization along the vertical dimension, as compared to horizontal dimension.
- D. In case C, each update results in more generalization along the horizontal dimension, as compared to vertical dimension.

**Đáp án đúng: B, C**

## Câu 15

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following affects generalization in tile coding? (Select all that apply)

- A. The number of tiles.
- B. The number of tilings.
- C. How the tilings are offset from each other.
- D. The shape of the tiles.

**Đáp án đúng: A, B, C, D**

_Ghi chú: Coursera xác nhận B, C, D đúng và báo còn thiếu, nên A cũng đúng._

## Câu 16

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

When tile coding is used for feature construction, the number of active or non-zero features

- A. is the number of tiles.
- B. is the number of tilings.
- C. is the number of tilings multiplied by the number of tiles.
- D. depends on the state.

**Đáp án đúng: B**

## Câu 17

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about neural networks (NNs) ? (Select all that apply)

- A. A NN is feedforward if there are no paths within the network by which a unit’s output can influence its input.
- B. Hidden layers are layers that are neither input nor output layers.
- C. The output of the units in NNs are typically a linear function of their input signals.
- D. NNs are parameterized functions that enable the agent to learn a nonlinear value function of state.
- E. The nonlinear functions applied to the weighted sum of the input signals are called the activation function.

**Đáp án đúng: A, B, D, E**

## Câu 18

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

Which of the following is the rectified linear activation function?

- A. $f(x) = \frac{1}{1 + e^{-x}}$
- B. $f(x) = 1$ if $x>0$ and $0$ otherwise
- C. $f(x) = max(0,x)$
- D. $f(x) = \frac{e ^{x} - e ^{-x}}{e ^{x} +e ^{-x}}$

**Đáp án đúng: C**

## Câu 19

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following are TRUE statements? (Select all that apply)

- A. A disadvantage of linear function approximation methods like tile coding is that they are linear in the input state.
- B. NNs are powerful function approximators and can learn accurate value functions, but typically require many samples to train.
- C. An advantage of linear methods is that they can be more data efficient than NNs, but they rely on an expert to design the features appropriately.
- D. An advantage of NNs is that learning can adapt the features, as compared to methods like tile coding.

**Đáp án đúng: B, C, D**

## Câu 20

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about backpropagation? (Select all that apply)

- A. Backpropagation corresponds to updating the parameters of a neural network using gradient descent.
- B. Backpropagation involves computing the partial derivatives of an objective function with respect to the weights of the network.
- C. The forward pass in backpropagation updates the weights of the network using the partial derivatives computed by the backward passes.
- D. Backpropagation computes partial derivatives starting from the last layer in the network, to save computation.

**Đáp án đúng: A, B, D**

_Ghi chú: Coursera xác nhận B, D đúng và báo còn thiếu. C sai vì forward pass không cập nhật trọng số, nên đáp án còn thiếu là A [Inference]._

## Câu 21

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Training neural networks (NNs) with backpropagation can be challenging because (Select all that apply)

- A. the loss surface might have flat regions, or poor local minima, meaning gradient descent gets stuck at poor solutions.
- B. the initialization can have a big impact on how much progress the gradient updates can make and on the quality of the final solution.
- C. neural networks cannot accurately represent most functions, so the loss stays large.
- D. learning can be slow due to the vanishing gradient problem, where if the partial derivatives for later nodes in the network are zero or near zero then this causes earlier nodes in the network to have small or near zero gradient updates.

**Đáp án đúng: A, B, D**

## Câu 22

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

Consider the following network: [hình] where for a given input $s$ , value of $s$ is computed by: $\psi = sW^{[0]} + b^{[0]}$ $x = \textit{max}(0, \psi)$ $v = xW^{[1]} + b^{[1]}$ What is the partial derivative of $v(s)$ with respect to $W^{[0]}_{ij}$ ?

- A. $s_i$
- B. $W^{[1]}_js_i$ if $x_j > 0$ and $0$ otherwise
- C. $x_j$
- D. $W^{[1]}_jx_j$ if $x_j > 0$ and $0$ otherwise

**Đáp án đúng: B**

## Câu 23

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE? (Select all that apply)

- A. When using stochastic gradient descent, we often completely eliminate the error for each example.
- B. The difference between stochastic gradient descent methods and batch gradient descent methods is that in the former the weights get updated using one random example whereas in the latter they get updated based on batches of data.
- C. Adagrad, Adam, and AMSGrad are stochastic gradient descent algorithms with adaptive step-sizes.
- D. Setting the step-size parameter for stochastic gradient descent can be challenging because a small step-size makes learning slow and a large step-size can result in divergence.

**Đáp án đúng: B, C, D**

## Câu 24

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about artificial neural networks (ANNs)? (Select all that apply)

- A. It is best to initialize the weights of a NN to large numbers so that the input signal does not get too small as it passes through the network.
- B. It is best to initialize the weights of a NN to small numbers so that the input signal does not grow rapidly as it passes through the network.
- C. If possible, it would be best to initialize the weights of an NN near the global optimum.
- D. A reasonable way to initialize the NN is with random weights, with each weight sampled from a normal distribution with the variance scaled by the number of inputs to the layer for that weight.

**Đáp án đúng: C, D**

_Ghi chú: Coursera xác nhận C, D đúng; B "should not be selected" (khởi tạo nhỏ làm tín hiệu teo lại, học chậm). A không chọn [Inference: khởi tạo quá lớn cũng không tốt]._

## Câu 25

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following are true? (Select all that apply)

- A. In the tabular case, updating the value of one state does not affect the values of other states.
- B. When using state aggregation or coarse coding, updating the value of one state does not affect the values of other states.
- C. When using state aggregation or coarse coding, there is generalization across states.
- D. In the tabular case, there is generalization across states, i.e., updates to the value function of one state influences the value function of other states.

**Đáp án đúng: A, C**

## Câu 26

_Nguồn: C3 – Control with Approximation (83.33%)_

To turn the update of Expected Sarsa algorithm to the update of Q-learning, one must:

- A. Use a neural network to approximate the action-value function.
- B. Expected Sarsa cannot be adapted to represent Q-learning.
- C. Use the maximum over all the actions instead of the expectation in the update function.
- D. Behave greedily with respect to the action-value function.

**Đáp án đúng: C**

## Câu 27

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following are true:

- A. Exploration is not a problem when using function approximation because learning generalizes across states and actions.
- B. When using function approximation, Q-learning will always result in better performance than Sarsa and Expected Sarsa.
- C. When using function approximation and with discrete actions, there is no straightforward way to turn Sarsa into Expected Sarsa.
- D. When learning value functions in the mountain car domain and using tiile coding, where all the rewards are -1 except when the terminal state is reached, initializing the weights of a linear function approximation to zero is an example of optimistic initialization.

**Đáp án đúng: D**

## Câu 28

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following statements about discounted return and differential return algorithms are true:

- A. There is a set of Bellman equations for the value function corresponding to the discounted return. However, there is no set of Bellman equations for differential value functions.
- B. The performance of discounted return algorithms can suffer because the optimal value of gamma is problem dependent.
- C. Algorithms that maximize the discounted return can suffer from an exponentially large variance when using a large discount factor.

**Đáp án đúng: B, C**

## Câu 29

_Nguồn: C3 – Control with Approximation (83.33%)_

Imagine we have 7 state features and 6 actions and we want to use linear function approximation to compute the action-value function. If we use feature stacking (as explained in Week 3), how many features would we need in total to approximate the action-value function of all the different actions?

- A. 67
- B. 13
- C. 42
- D. 76

**Đáp án đúng: C**

## Câu 30

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Imagine we are approximating the action-value function of three different actions (red, green, and blue) using three state features, resulting in the following weights and features: [hình] Which of these statements is true about our function approximation scheme?

- A. The green action will never be selected.
- B. The action-value of the green action will be exactly the same as the action-value of the red action for any state.
- C. There will not be any generalization across states.
- D. The action-value of the red action will be exactly the same as the action-value of the blue action.

**Đáp án đúng: B**

## Câu 31

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following feature and weight vectors corresponding to three state features and three actions (red, green, and blue): [hình] What is the approximate action-value for the blue action?

- A. 12
- B. 42
- C. 16
- D. 53

**Đáp án đúng: C**

## Câu 32

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following statements about epsilon-greedy policies and optimistic initialization are true:

- A. Implementing optimistic initialization is always straightforward and simple to implement regardless of the function approximation technique.
- B. Optimistic initialization results in a more systematic exploration in the tabular case because the agent takes actions it has not taken as often in a state.
- C. Optimistic initialization is always preferred over using an epsilon-greedy policy.
- D. Epsilon-greedy can be easily combined with any function approximation technique because it only needs to be able to query for the approximate action-values, without needing to know how they are initialized or computed.

**Đáp án đúng: B, D**

## Câu 33

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Consider the mountain car environment where all the rewards are -1 after every action until reaching the flag on top of the right hill: [hình] Which of the following are examples of optimistic initialization when using linear function approximation?

- A. Initialize all the weights at random using a uniform distribution between -5 and 5.
- B. Initialize all the weights so that the action-value function is -1 everywhere.
- C. Initialize all the weights so that the action-value function is zero everywhere.
- D. Initialize all the weights so that the action-value function is 10 everywhere.

**Đáp án đúng: C, D**

## Câu 34

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following MDP where the red action (L) at state S results in an immediate reward of +1 and 0 afterwards, and the blue action (R) results in 0 immediate reward, but a final reward of +2 when returning to state S. [hình] In this MDP, what is the optimal policy at state S when using discounted return with a value of gamma of 0.5? When using discounted return with a value of gamma of 0.9? When using average reward? (Hint: You can modify the equations used for the task from lesson 3 of this module to get the solution)

- A. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, red action; average reward, blue action.
- B. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, red action; average reward, red action.
- C. The optimal policy is: gamma = 0.5, red action; gamma = 0.9, blue action; average reward, blue action.
- D. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, blue action; average reward, red action.

**Đáp án đúng: C** [Inference]

_Ghi chú: Coursera xác nhận A sai. Mỗi vòng dài 4 bước. Red: G = 1/(1−γ⁴); Blue: G = 2γ³/(1−γ⁴). γ=0.5: 1 > 0.25 → red. γ=0.9: 1 < 1.458 → blue. Average reward: blue 2/4 > red 1/4 → blue._

## Câu 35

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following MDP with two states. State 1 has two actions: staying in the same state (blue) and switching to the other state (red). State 2 has a single (red) action leading to State 1. The rewards are listed next to each arrow/transition. [hình] If the agent is following a policy that takes the blue and red actions with equal probability, what is the average reward? (Hint: the state visitation probability is ⅔ for state 1 and ⅓ for state 2, the target policy probability \pi is the random policy, and all the transitions p are deterministic) Recall the formula is: [hình]

- A. Average reward = 3/4
- B. Average reward = 2
- C. Average reward = 1
- D. Average reward = 4/3

**Đáp án đúng: D** [Inference]

_Ghi chú: Coursera xác nhận A sai. Hình: blue (1→1) +1, red (1→2) +0, red (2→1) +3. r(π) = ⅔·(½·1 + ½·0) + ⅓·3 = ⅓ + 1 = 4/3._

## Câu 36

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

For which of the following tasks is the average reward setting preferable than the discounted return setting if we are interested in maximizing the total amount of reward?

- A. The nearsighted MDP from Week 3. The agent starts at an initial state S that splits into two paths, each leading to a ring that leads back to S after some time. If the agent chooses the left ring, it observes and immediate reward of +1 followed by 0 rewards, whereas choosing the right ring results on immediate reward of 0, but a final reward of +2 when returning to state S.
- B. An Atari 2600 game where the agent can keep playing until it loses all its lives, which are a finite amount.
- C. The job scheduling task from Section 10.3 of Sutton and Barto's RL textbook. The agent manages how jobs are scheduled into three different servers according to the priority of each job. When the agent accepts a job, the job runs in one of the servers and the agent gets a positive reward equal to the priority of the job, whereas when the agent rejects a job, the job returns to the queue and the agent receives a negative reward proportional to the priority of the job. The servers become available as they finish their jobs. Jobs are continually added to the queue and the agent accepts or rejects them.
- D. The episodic mountain car environment.

**Đáp án đúng: A, C**

## Câu 37

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is true about policy gradient methods? (Select all that apply)

- A. Policy gradient methods use generalized policy iteration to learn policies directly.
- B. Policy gradient methods do gradient ascent on the policy objective.
- C. If we have access to the true value function $v_\pi$ , we can perform unbiased stochastic gradient updates using the result from the Policy Gradient Theorem.
- D. The policy gradient theorem provides a form for the policy gradient that does not contain the gradient of the state distribution $\mu$ , which is hard to estimate.

**Đáp án đúng: B, C, D**

## Câu 38

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements about parameterized policies are true? (Select all that apply)

- A. The policy must be approximated using linear function approximation.
- B. The function used for representing the policy must be a softmax function.
- C. The probability of selecting any action must be greater than or equal to zero.
- D. For each state, the sum of all the action probabilities must equal to one.

**Đáp án đúng: C, D**

## Câu 39

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

Assume you’re given the following preferences $h_1 = 44$ , $h_2 = 42$ , and $h_3 = 38$ , corresponding to three different actions ( $a_1, a_2, a_3$ ), respectively. Under a softmax policy, what is the probability of choosing $a_2$ , rounded to three decimal numbers?

- A. 0.119
- B. 0.42
- C. 0.002
- D. 0.879

**Đáp án đúng: A**

## Câu 40

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is true about softmax policy? (Select all that apply)

- A. Similar to epsilon-greedy policy, softmax policy cannot approach a deterministic policy.
- B. It cannot represent an optimal policy that is stochastic, because it reaches a deterministic policy as one action preference dominates others.
- C. It is used to represent a policy in discrete action spaces.
- D. It can be parameterized by any function approximator as long as it can output scalar values for each available action, to form a softmax policy.

**Đáp án đúng: C, D**

## Câu 41

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

What are the differences between using softmax policy over action-values and using softmax policy over action-preferences? (Select all that apply)

- A. When using softmax policy over action-values, assuming a tabular representation, the policy will converge to the optimal policy regardless of whether the optimal policy is stochastic or deterministic.
- B. When using softmax policy over action-preferences, assuming a tabular representation, the policy will converge to the optimal policy regardless of whether the optimal policy is stochastic or deterministic.
- C. When using softmax policy over action-values, even if the optimal policy is deterministic, the policy may never approach a deterministic policy.

**Đáp án đúng: B, C**

## Câu 42

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

What is the following objective, and in which task formulation? $\Large r(\pi) = \Sigma_s \mu(s) \Sigma_a \pi(a|s, \mathbf{\theta}) \Sigma_{s’, r} p(s’, r | s, a) r$

- A. Average reward objective, episodic task
- B. Average reward objective, continuing task
- C. Discounted return objective, continuing task
- D. Undiscounted return objective, episodic task

**Đáp án đúng: B**

## Câu 43

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

The following equation is the outcome of the policy gradient theorem. Which of the following is true about the policy gradient theorem? (Select all that apply) $\Large \nabla r(\pi) = \Sigma_s \mu(s) \Sigma_a \nabla \pi(a|s, \mathbf{\theta}) q_{\pi} (s,a)$

- A. We do not need to compute the gradient of the state distribution $\mu$ .
- B. This expression can be converted into: $\large \mathbb{E}_\pi[\Sigma_a \nabla\pi(a|S, \mathbf{\theta})q_\pi(S,a)]$ In discrete action space, by approximating q_pi we could also use this gradient to update the policy.
- C. The true action value $q_\pi$ can be approximated in many ways, for example using TD algorithms.
- D. This expression can be converted into the following expectation over $\pi$ : $\large \mathbb{E}_\pi [\nabla \ln \pi (A|S, \theta) q_{\pi} (S,A)]$

**Đáp án đúng: A, B, C, D**

## Câu 44

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements is true? (Select all that apply)

- A. The Actor-Critic algorithm consists of two parts: a parameterized policy — the actor — and a value function — the critic.
- B. Subtracting a baseline in the policy gradient update tends to reduce the variance of the update, which results in faster learning.
- C. TD methods do not have a role when estimating the policy directly.
- D. To update the actor in Actor-Critic, we can use TD error in place of $q_\pi$ in the Policy Gradient Theorem.

**Đáp án đúng: A, B, D**

## Câu 45

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

To train the critic, we must use the average reward version of semi-gradient TD(0).

- A. True
- B. False

**Đáp án đúng: B**

## Câu 46

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

Consider the following state features and parameters $\theta$ for three different actions (red, green, and blue): [hình] Compute the action preferences for each of the three different actions using linear function approximation and stacked features for the action preferences.What is the action preference of $a_1$ (green)?

- A. 42
- B. 40
- C. 35
- D. 32

**Đáp án đúng: A**

## Câu 47

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements are true about the Actor-Critic algorithm with softmax policies? (Choose all that apply)

- A. The preferences must be approximated using linear function approximation.
- B. Since the policy is written as a function of the current state, it is like having a different softmax distribution for each state.
- C. The actor and the critic share the same set of parameters.
- D. The learning rate parameter of the actor and the critic can be different.

**Đáp án đúng: B, D**

## Câu 48

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is an advantage of Gaussian policy parameterization over discretizing the action space? (Select all that apply)

- A. Gaussian policies are differentiable, whereas policies over discretized actions are not.
- B. Continuous actions also allow learning to generalize over actions.
- C. Even if the true action set is discrete, but very large, it might be better to treat them as a continuous range.
- D. There might not be a straightforward way to choose a discrete set of actions.

**Đáp án đúng: B, C, D**

_Ghi chú: Coursera xác nhận B, C, D đúng; A "should not be selected" (softmax trên action rời rạc vẫn khả vi)._
