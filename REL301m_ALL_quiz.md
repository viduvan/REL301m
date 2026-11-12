# REL301m – Tổng hợp quiz Coursera (C1–C4, đã khử trùng lặp)

Gộp 4 khóa, bỏ câu trùng (cùng đề + cùng bộ lựa chọn, kể cả khác thứ tự). Quy ước giống các file từng khóa.

## Câu 1

_Nguồn: C1 – Sequential Decision-Making (100%)_

What is the incremental rule (sample average) for action values?

- A. $Q_{n+1}= Q_n + \frac{1}{n} [R_n + Q_n]$
- B. $Q_{n+1}= Q_n + \frac{1}{n} [R_n - Q_n]$
- C. $Q_{n+1}= Q_n + \frac{1}{n} [Q_n]$
- D. $Q_{n+1}= Q_n - \frac{1}{n} [R_n - Q_n]$

**Đáp án đúng: B**

## Câu 2

_Nguồn: C1 – Sequential Decision-Making (100%)_

Equation 2.5 (from the SB textbook, 2nd edition) is a key update rule we will use throughout the Specialization. We discussed this equation extensively in video. This exercise will give you a better hands-on feel for how it works. The blue line is the target that we might estimate with equation 2.5. The red line is our estimate plotted over time. $q_{n+1}=q_n+\alpha_n[R_n -q_n]$ Given the estimate update in red, what do you think was the value of the step size parameter we used to update the estimate on each time step? [hình: estimate cập nhật khoảng một nửa sai số]

- A. 1.0
- B. 1/2
- C. 1/8
- D. 1 / (t - 1)

**Đáp án đúng: B**

## Câu 3

_Nguồn: C1 – Sequential Decision-Making (100%)_

(Cùng đề Equation 2.5 như trên) Given the estimate update in red, what do you think was the value of the step size parameter we used to update the estimate on each time step? [hình: estimate cập nhật khoảng 1/8 sai số]

- A. 1.0
- B. 1/8
- C. 1 / (t - 1)
- D. 1/2

**Đáp án đúng: B**

## Câu 4

_Nguồn: C1 – Sequential Decision-Making (100%)_

(Cùng đề Equation 2.5 như trên) Given the estimate update in red, what do you think was the value of the step size parameter we used to update the estimate on each time step? [hình: estimate nhảy bằng target trước đó]

- A. 1/2
- B. 1/8
- C. 1.0
- D. 1 / (t - 1)

**Đáp án đúng: C**

## Câu 5

_Nguồn: C1 – Sequential Decision-Making (100%)_

(Cùng đề Equation 2.5 như trên) Given the estimate update in red, what do you think was the value of the step size parameter we used to update the estimate on each time step? [hình: ban đầu cập nhật hết, sau giảm dần]

- A. 1.0
- B. 1/2
- C. 1/8
- D. 1 / (t - 1)

**Đáp án đúng: D**

## Câu 6

_Nguồn: C1 – Sequential Decision-Making (100%)_

What is the exploration/exploitation tradeoff?

- A. The agent wants to explore the environment to learn as much about it as possible about the various actions. That way once it knows every arm’s true value it can choose the best one for the rest of the time.
- B. The agent wants to explore to get more accurate estimates of its values. The agent also wants to exploit to get more reward. The agent cannot, however, choose to do both simultaneously.
- C. The agent wants to maximize the amount of reward it receives over its lifetime. To do so it needs to avoid the action it believes is worst to exploit what it knows about the environment. However to discover which arm is truly worst it needs to explore different actions which potentially will lead it to take the worst action at times.

**Đáp án đúng: B**

## Câu 7

_Nguồn: C1 – Sequential Decision-Making (100%)_

Why did epsilon of 0.1 perform better over 1000 steps than epsilon of 0.01? [hình]

- A. Epsilon of 0.1 is the optimal value for epsilon in general.
- B. The 0.01 agent explored too much causing the arm to choose a bad action too often.
- C. The 0.01 agent did not explore enough. Thus it ended up selecting a suboptimal arm for longer.

**Đáp án đúng: C**

## Câu 8

_Nguồn: C1 – Sequential Decision-Making (100%)_

If exploration is so great why did epsilon of 0.0 (a greedy agent) perform better than epsilon of 0.4? [hình]

- A. Epsilon of 0.0 is greedy, thus it will always choose the optimal arm.
- B. Epsilon of 0.4 explores too often that it takes many sub-optimal actions causing it to do worse over the long term.
- C. Epsilon of 0.4 doesn’t explore often enough to find the optimal action.

**Đáp án đúng: B**

## Câu 9

_Nguồn: C1 – MDPs (100%)_

The learner and decision maker is the _______.

- A. Reward
- B. Agent
- C. Environment
- D. State

**Đáp án đúng: B**

## Câu 10

_Nguồn: C1 – MDPs (100%)_

At each time step the agent takes an _______.

- A. Environment
- B. State
- C. Reward
- D. Action

**Đáp án đúng: D**

## Câu 11

_Nguồn: C1 – MDPs (100%)_

Imagine the agent is learning in an episodic problem. Which of the following is true?

- A. The number of steps in an episode is always the same.
- B. The number of steps in an episode is stochastic: each episode can have a different number of steps.
- C. The agent takes the same action at each step during an episode.

**Đáp án đúng: B**

## Câu 12

_Nguồn: C1 – MDPs (100%)_

If the reward is always +1 what is the sum of the discounted infinite return when $\gamma < 1$ $G_t=\sum_{k=0}^{\infty} \gamma^{k}R_{t+k+1}$

- A. $G_t=\frac{1}{1-\gamma}$
- B. Infinity.
- C. $G_t=\frac{\gamma}{1-\gamma}$
- D. $G_t=1*\gamma^k$

**Đáp án đúng: A**

## Câu 13

_Nguồn: C1 – MDPs (100%)_

How does the magnitude of the discount factor (gamma/ $\gamma$ ) affect learning?

- A. The magnitude of the discount factor has no effect on the agent.
- B. With a larger discount factor the agent is more far-sighted and considers rewards farther into the future.
- C. With a smaller discount factor the agent is more far-sighted and considers rewards farther into the future.

**Đáp án đúng: B**

## Câu 14

_Nguồn: C1 – MDPs (100%)_

Suppose $\gamma=0.8$ and we observe the following sequence of rewards: $R_1 = -3$ , $R_2 = 5$ , $R_3=2$ , $R_4 = 7$ , and $R_5 = 1$ , with $T=5$ . What is $G_0$ ? Hint: Work Backwards and recall that $G_t = R_{t+1} + \gamma G_{t+1}$ .

- A. 11.592
- B. 6.2736
- C. 12
- D. -3
- E. 8.24

**Đáp án đúng: B**

## Câu 15

_Nguồn: C1 – MDPs (100%)_

What does MDP stand for?

- A. Markov Decision Protocol
- B. Markov Deterministic Policy
- C. Markov Decision Process
- D. Meaningful Decision Process

**Đáp án đúng: C**

## Câu 16

_Nguồn: C1 – MDPs (100%)_

Consider using reinforcement learning to control the motion of a robot arm to pick up objects and place them into new positions. The actions in this case might be the voltages applied to each motor at each joint, and the states might be the latest readings of joint angles and velocities. The reward might be +1 for each object successfully picked up and placed. To encourage smooth movements, on each time step a small, negative reward can be given as a function of the moment-to-moment “jerkiness” of the motion. Is this a valid MDP?

- A. Yes
- B. No

**Đáp án đúng: A**

## Câu 17

_Nguồn: C1 – MDPs (100%)_

Case 1: Imagine that you are a vision system. When you are first turned on for the day, an image floods into your camera. You can see lots of things, but not all things. You can't see objects that are occluded, and of course you can't see objects that are behind you. After seeing that first scene, do you have access to the Markov state of the environment? Case 2: Imagine that the vision system never worked properly: it always returned the same static imagine, forever. Would you have access to the Markov state then? (Hint: Reason about $P(S_{t+1} | S_t, ..., S_0)$ , where $S_t$ = AllWhitePixels)

- A. You have access to the Markov state in both Case 1 and 2.
- B. You have access to the Markov state in Case 1, but you don’t have access to the Markov state in Case 2.
- C. You don’t have access to the Markov state in Case 1, but you do have access to the Markov state in Case 2.
- D. You don’t have access to the Markov state in both Case 1 and 2.

**Đáp án đúng: A**

## Câu 18

_Nguồn: C1 – MDPs (100%)_

What is the reward hypothesis?

- A. Ignore rewards and find other signals.
- B. That all of what we mean by goals and purposes can be well thought of as the maximization of the expected value of the cumulative sum of a received scalar signal (called reward)
- C. That all of what we mean by goals and purposes can be well thought of as the minimization of the expected value of the cumulative sum of a received scalar signal (called reward)
- D. Always take the action that gives you the best reward at that point.

**Đáp án đúng: B**

## Câu 19

_Nguồn: C1 – MDPs (100%)_ · _chọn nhiều đáp án_

Imagine, an agent is in a maze-like gridworld. You would like the agent to find the goal, as quickly as possible. You give the agent a reward of +1 when it reaches the goal and the discount rate is 1.0, because this is an episodic task. When you run the agent its finds the goal, but does not seem to care how long it takes to complete each episode. How could you fix this? (Select all that apply)

- A. Give the agent -1 at each time step.
- B. Give the agent a reward of +1 at every time step.
- C. Set a discount rate less than 1 and greater than 0, like 0.9.
- D. Give the agent a reward of 0 at every time step so it wants to leave.

**Đáp án đúng: A, C**

## Câu 20

_Nguồn: C1 – MDPs (100%)_

When may you want to formulate a problem as continuing?

- A. When the agent-environment interaction does not naturally break into sequences. Each new episode begins independently of how the previous episode ended.
- B. When the agent-environment interaction naturally breaks into sequences and each sequence begins independently of how the previous sequence ended.

**Đáp án đúng: A**

## Câu 21

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

A policy is a function which maps ____ to ____.

- A. States to values.
- B. Actions to probability distributions over values.
- C. States to probability distributions over actions.
- D. Actions to probabilities.
- E. States to actions.

**Đáp án đúng: C**

## Câu 22

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

The term “backup” most closely resembles the term ___ in meaning.

- A. Value
- B. Update
- C. Diagram

**Đáp án đúng: B**

## Câu 23

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

At least one deterministic optimal policy exists in every Markov decision process.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 24

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

The optimal state-value function:

- A. Is not guaranteed to be unique, even in finite Markov decision processes.
- B. Is unique in every finite Markov decision process.

**Đáp án đúng: B**

## Câu 25

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Does adding a constant to all rewards change the set of optimal policies in episodic tasks?

- A. Yes, adding a constant to all rewards changes the set of optimal policies.
- B. No, as long as the relative differences between rewards remain the same, the set of optimal policies is the same.

**Đáp án đúng: A**

## Câu 26

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Does adding a constant to all rewards change the set of optimal policies in continuing tasks?

- A. No, as long as the relative differences between rewards remain the same, the set of optimal policies is the same.
- B. Yes, adding a constant to all rewards changes the set of optimal policies.

**Đáp án đúng: A**

## Câu 27

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Select the equation that correctly relates $v_{\ast}$ to $q_{\ast}$ . Assume $\pi$ is the uniform random policy.

- A. $v_{\ast}(s) = \sum_{a, r, s’} \pi(a | s) p(s’, r | s, a) [r + q_{\ast}(s’)]$
- B. $v_{\ast}(s) = \sum_{a, r, s’} \pi(a | s)p(s’, r | s, a) q_{\ast}(s’)$
- C. $v_{\ast}(s) = max_a q_{\ast}(s, a)$
- D. $v_{\ast}(s) = \sum_{a, r, s’} \pi(a | s) p(s’, r | s, a) [r + \gamma q_{\ast}(s’)]$

**Đáp án đúng: C**

## Câu 28

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Select the equation that correctly relates $q_{\ast}$ to $v_{\ast}$ using four-argument function $p$ .

- A. $q_{\ast}(s, a) = \sum_{s’, r} p(s’, r | a, s) [r + v_{\ast}(s')]$
- B. $q_{\ast}(s, a) = \sum_{s’, r} p(s’, r | a, s) \gamma [r + v_{\ast}(s’)]$
- C. $q_{\ast}(s, a) = \sum_{s’, r} p(s’, r | a, s) [r + \gamma v_{\ast}(s’)]$

**Đáp án đúng: C**

## Câu 29

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Write a policy $\pi_{\ast}$ in terms of $q_{\ast}$ .

- A. $\pi_{\ast}(a|s) = q_{\ast}(s, a)$
- B. $\pi_{\ast}(a|s) = \max_{a’} q_{\ast}(s, a’)$
- C. π∗(a|s)=1 if a=argmaxa′q∗(s,a′), else 0\pi_{\ast}(a|s) = 1 \mbox{ if } a = \mbox{argmax}_{a'} q_{\ast}(s, a'), \mbox{ else } 0

**Đáp án đúng: C**

## Câu 30

_Nguồn: C1 – [Practice] Value Functions and Bellman Equations (90%)_

Give an equation for some $\pi_{\ast}$ in terms of $v_{\ast}$ and the four-argument $p$ .

- A. $\pi_{\ast}(a|s) = 1 \text{ if } v_{\ast}(s) = \max_{a’} \sum_{s’, r} p(s’, r | s, a’) [ r + \gamma v_{\ast}(s’)], \text{ else } 0$
- B. $\pi_{\ast}(a|s) = 1 \text{ if } v_{\ast}(s) = \sum_{s’, r} p(s’, r | s, a) [ r + \gamma v_{\ast}(s’)], \text{ else } 0$
- C. $\pi_{\ast}(a|s) = \sum_{s’, r} p(s’, r | s, a) [ r + \gamma v_{\ast}(s’)]$
- D. $\pi_{\ast}(a|s) = \max_{a’} \sum_{s’, r} p(s’, r | s, a’) [ r + \gamma v_{\ast}(s’)]$

**Đáp án đúng: A** [Inference]

_Ghi chú: Coursera xác nhận D sai. π\* chỉ đặt xác suất 1 cho action đạt max trong phương trình Bellman tối ưu, nên chọn A._

## Câu 31

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

A function which maps ___ to ___ is a value function. [Select all that apply]

- A. State-action pairs to expected returns.
- B. States to expected returns.
- C. Values to actions.
- D. Values to states.

**Đáp án đúng: A, B**

## Câu 32

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

Consider the continuing Markov decision process shown below. The only decision to be made is in the top state, where two actions are available, left and right. The numbers show the rewards that are received deterministically after each action. There are exactly two deterministic policies, $\pi_{\text{left}}$ and $\pi_{\text{right}}$ . Indicate the optimal policies if $\gamma = 0$ ? If $\gamma = 0.9$ ? If $\gamma = 0.5$ ? [Select all that apply] [hình]

- A. For $\gamma = 0.5, \pi_{\text{left}}$
- B. For $\gamma = 0.9, \pi_{\text{left}}$
- C. For $\gamma = 0, \pi_{\text{left}}$
- D. For $\gamma = 0, \pi_{\text{right}}$
- E. For $\gamma = 0.5, \pi_{\text{right}}$
- F. For $\gamma = 0.9, \pi_{\text{right}}$

**Đáp án đúng: A, C, E, F**

_Ghi chú: Coursera xác nhận C, E đúng và B sai. Feedback của E ghi: với γ=0.5, tổng reward 2 bước của left = right = 1, nên cả hai policy đều tối ưu (vì vậy A đúng). Với γ=0.9, right tốt hơn (F) [Inference]._

## Câu 33

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

Every finite Markov decision process has __. [Select all that apply]

- A. A unique optimal value function
- B. A stochastic optimal policy
- C. A deterministic optimal policy
- D. A unique optimal policy

**Đáp án đúng: A, C**

## Câu 34

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_

The ___ of the reward for each state-action pair, the dynamics function $p$ , and the policy $\pi$ is _____ to characterize the value function $v_{\pi}$ . (Remember that the value of a policy $\pi$ at state $s$ is $v_{\pi}(s) = \sum_a \pi(a | s) \sum_{s',r} p(s', r | s, a) [ r + \gamma v_{\pi}(s') ]$ .)

- A. Mean; sufficient
- B. Distribution; necessary

**Đáp án đúng: A**

## Câu 35

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

The Bellman equation for a given a policy $\pi$ : [Select all that apply]

- A. Holds only when the policy is greedy with respect to the value function.
- B. Expresses state values $v(s)$ in terms of state values of successor states.
- C. Expresses the improved policy in terms of the existing policy.

**Đáp án đúng: B**

## Câu 36

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_

An optimal policy:

- A. Is not guaranteed to be unique, even in finite Markov decision processes.
- B. Is unique in every finite Markov decision process.
- C. Is unique in every Markov decision process.

**Đáp án đúng: A**

## Câu 37

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

The Bellman optimality equation for $v_{\ast}$ : [Select all that apply]

- A. Expresses the improved policy in terms of the existing policy.
- B. Holds for the optimal state value function.
- C. Holds when the policy is greedy with respect to the value function.
- D. Expresses state values $v_{\ast}(s)$ in terms of state values of successor states.
- E. Holds for $v_{\pi}$ , the value function of an arbitrary policy $\pi$ .

**Đáp án đúng: B, D**

## Câu 38

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_

Give an equation for $v_{\pi}$ in terms of $q_{\pi}$ and $\pi$ .

- A. $v_{\pi}(s) = \max_{a} \gamma \pi(a | s) q_{\pi}(s, a)$
- B. $v_{\pi}(s) = \max_{a} \pi(a | s) q_{\pi}(s, a)$
- C. $v_{\pi}(s) = \sum_{a} \pi(a | s) q_{\pi}(s, a)$
- D. $v_{\pi}(s) = \sum_{a} \gamma \pi(a | s) q_{\pi}(s, a)$

**Đáp án đúng: C**

## Câu 39

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_

Give an equation for $q_{\pi}$ in terms of $v_{\pi}$ and the four-argument $p$ .

- A. $q_{\pi}(s, a) = \sum_{s’} \sum_{r} p(s’, r | s, a)[r + \gamma v_{\pi}(s’)]$
- B. $q_{\pi}(s, a) = \max_{s’, r} p(s’, r | s, a) [r + v_{\pi}(s’)]$
- C. $q_{\pi}(s, a) = \max_{s’, r} p(s’, r | s, a)[r + \gamma v_{\pi}(s’)]$
- D. $q_{\pi}(s, a) = \max_{s’, r} p(s’, r | s, a) \gamma[r + v_{\pi}(s’)]$
- E. $q_{\pi}(s, a) = \sum_{s’} \sum_{r} p(s’, r | s, a) \gamma[r + v_{\pi}(s’)]$
- F. $q_{\pi}(s, a) = \sum_{s’} \sum_{r} p(s’, r | s, a) [r + v_{\pi}(s’)]$

**Đáp án đúng: A**

## Câu 40

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_ · _chọn nhiều đáp án_

Let $r(s,a)$ be the expected reward for taking action $a$ in state $s$ , as defined in equation 3.5 of the textbook. Which of the following are valid ways to re-express the Bellman equations, using this expected reward function? [Select all that apply]

- A. $q_{\ast}(s, a) = r(s, a) + \gamma \sum_{s’} p(s’ | s, a) \max_{a’} q_{\ast}(s’, a’)$
- B. $v_{\pi}(s) = \sum_a \pi(a | s) [r(s, a) + \gamma \sum_{s’} p(s’ | s, a) v_{\pi}(s’)]$
- C. $q_{\pi}(s, a) = r(s, a) + \gamma \sum_{s’} \sum_{a’} p(s’ | s, a) \pi(a’ | s’)q_{\pi}(s’, a’)$
- D. $v_{\ast}(s) = \max_a [r(s, a) + \gamma \sum_{s’} p(s’ | s, a) v_{\ast}(s’)]$

**Đáp án đúng: A, B, C, D**

## Câu 41

_Nguồn: C1 – [Graded] Value Functions and Bellman Equations (90.90%)_

Consider an episodic MDP with one state and two actions (left and right). The left action has stochastic reward $1$ with probability $p$ and $3$ with probability $1-p$ . The right action has stochastic reward $0$ with probability $q$ and $10$ with probability $1-q$ . What relationship between $p$ and $q$ makes the actions equally optimal?

- A. $7 + 3p = -10q$
- B. $13 + 3p = -10q$
- C. $13 + 2p = 10q$
- D. $7 + 2p = -10q$
- E. $13 + 3p = 10q$
- F. $7 + 3p = 10q$
- G. $13 + 2p = -10q$
- H. $7 + 2p = 10q$

**Đáp án đúng: H**

## Câu 42

_Nguồn: C1 – Dynamic Programming (100%)_ · _chọn nhiều đáp án_

The value of any state under an optimal policy is ___ the value of that state under a non-optimal policy. [Select all that apply]

- A. Strictly greater than
- B. Greater than or equal to
- C. Strictly less than
- D. Less than or equal to

**Đáp án đúng: B**

## Câu 43

_Nguồn: C1 – Dynamic Programming (100%)_

If a policy $\pi$ is greedy with respect to its own value function $v_{\pi}$ , then it is an optimal policy.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 44

_Nguồn: C1 – Dynamic Programming (100%)_

Let $v_{\pi}$ be the state-value function for the policy $\pi$ . Let $\pi'$ be greedy with respect to $v_{\pi}$ . Then $v_{\pi'} \geq v_{\pi}$ .

- A. True
- B. False

**Đáp án đúng: A**

## Câu 45

_Nguồn: C1 – Dynamic Programming (100%)_ · _chọn nhiều đáp án_

What is the relationship between value iteration and policy iteration? [Select all that apply]

- A. Value iteration and policy iteration are both special cases of generalized policy iteration.
- B. Policy iteration is a special case of value iteration.
- C. Value iteration is a special case of policy iteration.

**Đáp án đúng: A**

## Câu 46

_Nguồn: C1 – Dynamic Programming (100%)_ · _chọn nhiều đáp án_

The word synchronous means "at the same time". The word asynchronous means "not at the same time". A dynamic programming algorithm is: [Select all that apply]

- A. Asynchronous, if it does not update all states at each iteration.
- B. Synchronous, if it systematically sweeps the entire state space at each iteration.
- C. Asynchronous, if it updates some states more than others.

**Đáp án đúng: A, B, C**

## Câu 47

_Nguồn: C1 – Dynamic Programming (100%)_

All Generalized Policy Iteration algorithms are synchronous.

- A. True
- B. False

**Đáp án đúng: B**

## Câu 48

_Nguồn: C1 – Dynamic Programming (100%)_

Which of the following is true?

- A. Asynchronous methods generally scale to large state spaces better than synchronous methods.
- B. Synchronous methods generally scale to large state spaces better than asynchronous methods.

**Đáp án đúng: A**

## Câu 49

_Nguồn: C1 – Dynamic Programming (100%)_ · _chọn nhiều đáp án_

Why are dynamic programming algorithms considered planning methods? [Select all that apply]

- A. They learn from trial and error interaction.
- B. They use a model to improve the policy.
- C. They compute optimal value functions.

**Đáp án đúng: B**

## Câu 50

_Nguồn: C1 – Dynamic Programming (100%)_

Consider the undiscounted, episodic MDP below. There are four actions possible in each state, A = {up, down, right, left}, which deterministically cause the corresponding state transitions, except that actions that would take the agent off the grid in fact leave the state unchanged. The right half of the figure shows the value of each state under the equiprobable random policy. If $\pi$ is the equiprobable random policy, what is q(7,down)q(7, \mbox{down})? [hình]

- A. q(7,down)=−14q(7, \mbox{down}) = -14
- B. q(7,down)=−20q(7, \mbox{down}) = -20
- C. q(7,down)=−21q(7, \mbox{down}) = -21
- D. q(7,down)=−15q(7, \mbox{down}) = -15

**Đáp án đúng: D**

## Câu 51

_Nguồn: C1 – Dynamic Programming (100%)_

Consider the undiscounted, episodic MDP below. There are four actions possible in each state, A = {up, down, right, left}, which deterministically cause the corresponding state transitions, except that actions that would take the agent off the grid in fact leave the state unchanged. The right half of the figure shows the value of each state under the equiprobable random policy. If $\pi$ is the equiprobable random policy, what is $v(15)$ ? Hint: Recall the Bellman equation $v(s) = \sum_a \pi(a | s) \sum_{s’, r} p(s’, r | s, a) [r + \gamma v(s’)]$ . [hình]

- A. $v(15) = -23$
- B. $v(15) = -21$
- C. $v(15) = -24$
- D. $v(15) = -25$
- E. $v(15) = -22$

**Đáp án đúng: C**

## Câu 52

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_ · _chọn nhiều đáp án_

Which approach ensures continual (never-ending) exploration? (Select all that apply)

- A. Exploring starts
- B. On-policy learning with a deterministic policy
- C. On-policy learning with an $\epsilon$ -soft policy
- D. Off-Policy learning with an $\epsilon$ -soft behavior policy and a deterministic target policy
- E. Off-Policy learning with an $\epsilon$ -soft target policy and a deterministic behavior policy

**Đáp án đúng: A, C, D**

## Câu 53

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_ · _chọn nhiều đáp án_

When can Monte Carlo methods, as defined in the course, be applied? (Select all that apply)

- A. When the problem is continuing and given a batch of data containing sequences of states, actions, and rewards
- B. When the problem is continuing and there is a model that produces samples of the next state and reward
- C. When the problem is episodic and given a batch of data containing sample episodes (sequences of states, actions, and rewards)
- D. When the problem is episodic and there is a model that produces samples of the next state and reward

**Đáp án đúng: C, D**

## Câu 54

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_ · _chọn nhiều đáp án_

Which of the following learning settings are examples of off-policy learning? (Select all that apply)

- A. Learning the optimal policy while continuing to explore
- B. Learning from data generated by a human expert

**Đáp án đúng: A, B**

## Câu 55

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

Which of the following is a requirement on the behaviour policy $b$ for using off-policy Monte Carlo policy evaluation? This is called the assumption of coverage.

- A. For each state $s$ and action $a$ , if $\pi(a\mid s)>0$ then $b(a\mid s)>0$
- B. For each state $s$ and action $a$ , if $b(a\mid s)>0$ then $\pi(a\mid s)>0$
- C. All actions have non-zero probabilities under $\pi$

**Đáp án đúng: A**

## Câu 56

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_ · _chọn nhiều đáp án_

When is it possible to determine a policy that is greedy with respect to the value functions $v_{\pi}, q_{\pi}$ for the policy $\pi$ ? (Select all that apply)

- A. When state values $v_{\pi}$ and a model are available
- B. When state values $v_{\pi}$ are available but no model is available.
- C. When action values $q_{\pi}$ and a model are available
- D. When action values $q_{\pi}$ are available but no model is available.

**Đáp án đúng: A, C, D**

## Câu 57

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

Monte Carlo methods in Reinforcement Learning work by...Hint: recall we used the term sweep in dynamic programming to discuss updating all the states systematically. This is not the same as visiting a state.

- A. Averaging sample returns
- B. Averaging sample rewards
- C. Planning with a model of the environment
- D. Performing sweeps through the state set

**Đáp án đúng: A**

## Câu 58

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

Suppose the state $s$ has been visited three times, with corresponding returns $8$ , $4$ , and $3$ . What is the current Monte Carlo estimate for the value of $s$ ?

- A. $3$
- B. $15$
- C. $5$
- D. $3.5$

**Đáp án đúng: C**

## Câu 59

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

When does Monte Carlo prediction perform its first update?

- A. After the first time step
- B. After every state is visited at least once
- C. At the end of the first episode

**Đáp án đúng: C**

## Câu 60

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

For Monte Carlo Prediction of state-values, the number of updates at the end of an episode depends onHint: look at the innermost loop of the algorithm

- A. The length of the episode
- B. The number of states
- C. The number of possible actions in each state

**Đáp án đúng: A**

## Câu 61

_Nguồn: C2 – Graded Quiz (IsmE3) (100%)_

In an $\epsilon$ -greedy policy over $\mathcal{A}$ actions, what is the probability of the highest valued action if there are no other actions with the same value?

- A. $1-\epsilon$
- B. $\epsilon$
- C. $1-\epsilon+\frac{\epsilon}{\mathcal{A}}$
- D. $\frac{\epsilon}{\mathcal{A}}$

**Đáp án đúng: C**

## Câu 62

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

TD(0) is a solution method for:

- A. Control
- B. Prediction

**Đáp án đúng: B**

## Câu 63

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_ · _chọn nhiều đáp án_

Which of the following methods use bootstrapping? (Select all that apply)

- A. Dynamic Programming
- B. Monte Carlo
- C. TD(0)

**Đáp án đúng: A, C**

## Câu 64

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

Which of the following is the correct characterization of Dynamic Programming (DP) and Temporal Difference (TD) methods?

- A. Both TD and DP methods use expected updates.
- B. Both TD and DP methods use sample updates.
- C. TD methods use expected updates, DP methods use sample updates.
- D. TD methods uses sample updates, DP methods use expected updates.

**Đáp án đúng: D**

## Câu 65

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_ · _chọn nhiều đáp án_

Match the algorithm name to its correct update (select all that apply)

- A. TD(0): $V(S_t) \leftarrow V(S_t) + \alpha [G_t - V(S_t)]$
- B. Monte Carlo: $V(S_t) \leftarrow V(S_t) + \alpha [R_{t + 1} + \gamma V(S_{t + 1}) - V(S_t)]$
- C. Monte Carlo: $V(S_t) \leftarrow V(S_t) + \alpha [G_t - V(S_t)]$
- D. TD(0): $V(S_t) \leftarrow V(S_t) + \alpha [R_{t + 1} + \gamma V(S_{t + 1}) - V(S_t)]$

**Đáp án đúng: C, D**

## Câu 66

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_ · _chọn nhiều đáp án_

Which of the following well-describe Temporal Difference (TD) and Monte-Carlo (MC) methods?

- A. TD methods can be used in continuing tasks.
- B. MC methods can be used in continuing tasks.
- C. TD methods can be used in episodic tasks.
- D. MC methods can be used in episodic tasks.

**Đáp án đúng: A, C, D**

## Câu 67

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_ · _chọn nhiều đáp án_

In an episodic setting, we might have different updates depending on whether the next state is terminal or non-terminal. Which of the following TD error calculations are correct?

- A. $S_{t + 1}$ is non-terminal: $\delta_t = R_{t + 1} + \gamma V(S_{t + 1}) - V(S_t)$
- B. $S_{t + 1}$ is non-terminal: $\delta_t = R_{t + 1} - V(S_t)$
- C. $S_{t + 1}$ is terminal: $\delta_t = R_{t + 1} + \gamma V(S_{t + 1}) - V(S_t)$ with $V(S_{t + 1}) = 0$
- D. $S_{t + 1}$ is terminal: $\delta_t = R_{t + 1} - V(S_t)$

**Đáp án đúng: A, C, D**

## Câu 68

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

Suppose we have current estimates for the value of two states: V(A) = 1.0, V(B) = 1.0 in an episodic setting. We observe the following trajectory: A, 0, B, 1, B, 0, T where T is a terminal state. Apply TD(0) with step-size, $\alpha = 1$ , and discount factor, $\gamma = 0.5$ . What are the value estimates for state A and state B at the end of the episode?

- A. (1.0, 1.0)
- B. (0.5, 0)
- C. (0, 1.5)
- D. (1, 0)
- E. (0, 0)

**Đáp án đúng: B**

## Câu 69

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

Which of the following pairs is the correct characterization of the targets used in TD(0) and Monte Carlo?

- A. TD(0): High Variance Target, Monte Carlo: High Variance Target
- B. TD(0): High Variance Target, Monte Carlo: Low Variance Target
- C. TD(0): Low Variance Target, Monte Carlo: High Variance Target
- D. TD(0): Low Variance Target, Monte Carlo: Low Variance Target

**Đáp án đúng: C**

## Câu 70

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

Suppose you observe the following episodes of the form (State, Reward, ...) from a Markov Decision Process with states A and B:EpisodesA, 0, B, 0B, 1B, 1B, 1B, 0B, 0B, 1B, 0What would batch Monte Carlo methods give for the estimates V(A) and V(B)? What would batch TD(0) give for the estimates V(A) and V(B)? Use a discount factor, $\gamma$ , of 1.For Batch MC: compute the average returns observed from each state. For Batch TD: You can start with state B. What is its expected return? Then figure out V(A) using the temporal difference equation: $V(S_t) = E [R_{t+1} + \gamma V(S_{t+1})]$ .Answers are provided in the following format: $V^\text{batch-MC}(A)$ is the value for state $A$ under Monte Carlo learning $V^\text{batch-MC}(B)$ is the value of state $B$ under Monte Carlo learning $V^\text{batch-TD}(A)$ is the value of state $A$ under TD learning $V^\text{batch-TD}(B)$ is the value of state $B$ under TD learningHint: review example 6.3 in Sutton and Barto; this question is the same, just with different numbers.

- A. $V^\text{batch-MC}(A)=0$ $V^\text{batch-MC}(B)=0.5$ $V^\text{batch-TD}(A)=0.5$ $V^\text{batch-TD}(B)=0.5$
- B. $V^\text{batch-MC}(A)=0$ $V^\text{batch-MC}(B)=0.5$ $V^\text{batch-TD}(A)=0$ $V^\text{batch-TD}(B)=0.5$
- C. $V^\text{batch-MC}(A)=0$ $V^\text{batch-MC}(B)=0.5$ $V^\text{batch-TD}(A)=0$ $V^\text{batch-TD}(B)=0$
- D. $V^\text{batch-MC}(A)=0$ $V^\text{batch-MC}(B)=0.5$ $V^\text{batch-TD}(A)=1.5$ $V^\text{batch-TD}(B)=0.5$
- E. $V^\text{batch-MC}(A)=0.5$ $V^\text{batch-MC}(B)=0.5$ $V^\text{batch-TD}(A)=0.5$ $V^\text{batch-TD}(B)=0.5$

**Đáp án đúng: A** [Inference]

_Ghi chú: Coursera xác nhận B sai. Tự tính: V(B) = 4/8 = 0.5 (có 8 lần gặp B, 4 lần reward 1). MC: V(A) = 0 (return duy nhất của A là 0). TD: V(A) = 0 + V(B) = 0.5._

## Câu 71

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

True or False: "Both TD(0) and Monte-Carlo (MC) methods converge to the true value function asymptotically, given that the environment is Markovian."

- A. True
- B. False

**Đáp án đúng: A**

## Câu 72

_Nguồn: C2 – Practice Quiz (afTG5) (90.90%)_

Which of the following pairs is the correct characterization of the TD(0) and Monte-Carlo (MC) methods?

- A. Both TD(0) and MC are offline methods.
- B. Both TD(0) and MC are online methods.
- C. TD(0) is an online method while MC is an offline method.
- D. MC is an online method while TD(0) is an offline method.

**Đáp án đúng: C**

## Câu 73

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

What is the target policy in Q-learning?

- A. $\epsilon$ -greedy with respect to the current action-value estimates
- B. Greedy with respect to the current action-value estimates

**Đáp án đúng: B**

## Câu 74

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Which Bellman equation is the basis for the Q-learning update?

- A. Bellman equation for state values
- B. Bellman equation for action values
- C. Bellman optimality equation for state values
- D. Bellman optimality equation for action values

**Đáp án đúng: D**

## Câu 75

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Which Bellman equation is the basis for the Sarsa update?

- A. Bellman equation for state values
- B. Bellman equation for action values
- C. Bellman optimality equation for state values
- D. Bellman optimality equation for action values

**Đáp án đúng: B**

## Câu 76

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Which Bellman equation is the basis for the Expected Sarsa update?

- A. Bellman equation for state values
- B. Bellman equation for action values
- C. Bellman optimality equation for state values
- D. Bellman optimality equation for action values

**Đáp án đúng: B**

## Câu 77

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Which algorithm’s update requires more computation per step?

- A. Expected Sarsa
- B. Sarsa

**Đáp án đúng: A**

## Câu 78

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Which algorithm has a higher variance target?

- A. Expected Sarsa
- B. Sarsa

**Đáp án đúng: B**

## Câu 79

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Q-learning does not learn about the outcomes of exploratory actions.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 80

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Sarsa, Q-learning, and Expected Sarsa have similar targets on a transition to a terminal state.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 81

_Nguồn: C2 – Practice Quiz (8ukkF) (100%)_

Sarsa needs to wait until the end of an episode before performing its update.

- A. True
- B. False

**Đáp án đúng: B**

## Câu 82

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

Which of the following are the most accurate characterizations of sample models and distribution models? (Select all that apply)

- A. A sample model can be used to compute the probability of all possible trajectories in an episodic task based on the current state and action.
- B. A distribution model can be used as a sample model.
- C. Both sample models and distribution models can be used to obtain a possible next state and reward, given the current state and action.
- D. A sample model can be used to obtain a possible next state and reward given the current state and action, whereas a distribution model can only be used to compute the probability of this next state and reward given the current state and action.

**Đáp án đúng: B, C**

## Câu 83

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

Which of the following statements are TRUE for Dyna architecture? (Select all that apply)

- A. Real experience can be used to improve the value function and policy
- B. Real experience can be used to improve the model
- C. Simulated experience can be used to improve the model
- D. Simulated experience can be used to improve the value function and policy

**Đáp án đúng: A, B, D**

## Câu 84

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

Mark all the statements that are TRUE for the tabular Dyna-Q algorithm. (Select all that apply)

- A. For a given state-action pair, the model predicts the next state and reward
- B. The memory requirements for the model in case of a deterministic environment are quadratic in the number of states
- C. The algorithm cannot be extended to stochastic environments.
- D. The environment is assumed to be deterministic.

**Đáp án đúng: A, D**

## Câu 85

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

Which of the following statements are TRUE? (Select all the apply)

- A. Model-based methods often suffer more from bias than model-free methods, because of inaccuracies in the model.
- B. When compared with model-free methods, model-based methods are relatively more sample efficient. They can achieve a comparable performance with comparatively fewer environmental interactions.
- C. Model-based methods like Dyna typically require more memory than model-free methods like Q-learning.
- D. The amount of computation per interaction with the environment is larger in the Dyna-Q algorithm (with non-zero planning steps) as compared to the Q-learning algorithm.

**Đáp án đúng: A, B, C, D**

## Câu 86

_Nguồn: C2 – Practice Assessment (90%)_

Which of the following is generally the most computationally expensive step of the Dyna-Q algorithm? Assume N>1 planning steps are being performed (e.g., N=20). [hình]

- A. Model learning (step e)
- B. Direct RL (step d)
- C. Action selection (step b)
- D. Planning (Indirect RL; step f)

**Đáp án đúng: D**

## Câu 87

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

What are some possible reasons for a learned model to be inaccurate? (Select all that apply)

- A. The transition dynamics of the environment are stochastic, and only a few transitions have been experienced.
- B. The environment has changed.
- C. The agent’s policy has changed significantly from the beginning of training.
- D. There is too much exploration (e.g., epsilon is epsilon-greedy exploration is set to a high value of 0.5)

**Đáp án đúng: A, B**

## Câu 88

_Nguồn: C2 – Practice Assessment (90%)_

In search control, which of the following methods is likely to make a Dyna agent perform better in problems with a large number of states (like the rod maneuvering problem in Chapter 8 of the textbook)? Recall that search control is the process that selects the starting states and actions in planning. Also, recall the navigation example in the video lectures in which a large number of wasteful updates were being made because of the basic search control procedure in the Dyna-Q algorithm. (Select the best option)

- A. Select state-action pairs uniformly at random from all previously experienced pairs.
- B. Start backwards from state-action pairs that have had a non-zero update (e.g., from the state right beside a goal state). This avoids the otherwise wasteful computations from state-action pairs which have had no updates.
- C. Start with state-action pairs enumerated in a fixed order (e.g., in a gridworld, states top-left to bottom-right, actions up, down, left, right)
- D. All of these are equally good/bad.

**Đáp án đúng: B**

## Câu 89

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

In the lectures, we saw how the Dyna-Q+ agent found the newly-opened shortcut in the shortcut maze, whereas the Dyna-Q agent didn’t. Which of the following implications drawn from the figure are TRUE? (Select all that apply) [hình]

- A. The Dyna-Q+ agent performs better than the Dyna-Q agent even in the first half of the experiment because of the increased exploration.
- B. The Dyna-Q agent can never discover shortcuts (i.e., when the environment changes to become better than it was before).
- C. The difference between Dyna-Q+ and Dyna-Q narrowed slightly over the first part of the experiment. This is because the Dyna-Q+ agent keeps exploring even when the environment isn’t changing.
- D. None of the above are true.

**Đáp án đúng: A, C**

## Câu 90

_Nguồn: C2 – Practice Assessment (90%)_

Consider the gridworld depicted in the diagram below. There are four actions corresponding to up, down, right, and left movements. Marked is the path taken by an agent in a single episode, ending at a location of high reward, marked by the G. In this example the values were all zero at the start of the episode, and all rewards were zero during the episode except for a positive reward at G. [hình] Now which of the following figures best depicts the action values that would’ve increased by the end of the episode using one-step Sarsa and 500-step-planning Dyna-Q? (Select the best option)

- A. [hình] Sarsa: cả đường đi | Dyna-Q: cả đường đi
- B. [hình] Sarsa: cả đường đi | Dyna-Q: chỉ ô cạnh G
- C. [hình] Sarsa: chỉ ô cạnh G | Dyna-Q: cả đường đi
- D. [hình] Sarsa: chỉ ô cạnh G | Dyna-Q: chỉ ô cạnh G

**Đáp án đúng: C**

_Ghi chú: Coursera xác nhận A sai. Feedback ghi: one-step Sarsa chỉ cập nhật đúng 1 cặp state-action dẫn vào G, còn Dyna-Q 500 bước planning cập nhật toàn bộ đường đi._

## Câu 91

_Nguồn: C2 – Practice Assessment (90%)_ · _chọn nhiều đáp án_

Which of the following are planning methods? (Select all that apply)

- A. Q-learning
- B. Expected Sarsa
- C. Value Iteration
- D. Dyna-Q

**Đáp án đúng: C, D**

## Câu 92

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following statements is true about function approximation in reinforcement learning? (Select all that apply)

- A. It allows faster training by generalizing between states.
- B. We only use function approximation because we have to for large or continuous state spaces. We would use tabular methods if we could, and learn an independent value per state.
- C. It can be more memory efficient.
- D. It can help the agent achieve good generalization with good discrimination, so that it learns faster and represent the values quite accurately.

**Đáp án đúng: A, C, D**

## Câu 93

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

We learned how value function estimation can be framed as supervised learning. But not all supervised learning methods are suitable. What are some characteristics of reinforcement learning that can make it harder to apply standard supervised learning methods?

- A. Data is available as a fixed batch.
- B. Data is temporally correlated in reinforcement learning.
- C. When using bootstrapping methods like TD, the target labels change.

**Đáp án đúng: B, C**

## Câu 94

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

Value Prediction (or Policy Evaluation) with Function Approximation can be viewed as supervised learning mainly because _________. [choose the most appropriate completion of the proceeding statement]

- A. Each state and its target (used in the Monte Carlo update, TD(0) update, and DP update) forms an input-output training example which we can use to train our approximation to the value function
- B. We use stochastic gradient descent to learn the value function.
- C. We can learn the value function by training with batches of data obtained from the agent’s interaction with the world.

**Đáp án đúng: A**

## Câu 95

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about using Mean Squared Value Error ( $\bar{VE} = \sum \mu(s) [v_\pi(s) - \hat{v}(s,w)]^2$ ) as the prediction objective? $\mu(s)$ represents the weighted distribution of visited states(Select all that apply)

- A. Even if the agent uses a linear representation that cannot represent the true values, the agent can still get zero MSVE.
- B. Gradient Monte Carlo with linear function approximation converges to the global optimum of this objective, if the step size is reduced over time.
- C. The agent can get zero MSVE when using a tabular representation that can represent the true values.
- D. This objective makes it explicit how we should trade-off accuracy of the value estimates across states, using the weighting $\mu$ .

**Đáp án đúng: B, C, D**

## Câu 96

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about $\mu(S)$ in Mean Squared Value Error? (Select all that apply)

- A. It serves as a weighting to minimize the error more in states that we care about.
- B. It is a probability distribution.
- C. If the policy is uniformly random, $\mu(S)$ would have the same value for all states.
- D. It has higher values for states that are visited more often.

**Đáp án đúng: A, B, D**

## Câu 97

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

The stochastic gradient descent update for the MSVE would be as follows.Fill in the blanks (A), (B), (C ) and (D) with correct terms. (Select all correct answers) $\mathbf{w_{t+1}} \doteq \mathbf{w_t} \hspace{0.25em} (A) \hspace{0.25em} \frac{1}{2}\alpha \nabla [\hspace{0.25em} (C) \hspace{0.25em} - \hspace{0.25em} (D)\hspace{0.25em} ]^2$ $\quad\quad = \mathbf{w_t} \hspace{0.25em} (B) \hspace{0.25em} \alpha [\hspace{0.25em} (C) \hspace{0.25em} - \hspace{0.25em} (D)\hspace{0.25em} ] \nabla \hat{v}(S_t,\mathbf{w_t})$ $(\alpha > 0)$

- A. $+, -, v_\pi(S_t), \hat{v}(S_t, \mathbf{w_t})$
- B. $-, -, \hat{v}(S_t, \mathbf{w_t}), v_\pi(S_t)$
- C. $-, +, v_\pi(S_t), \hat{v}(S_t, \mathbf{w_t})$
- D. $+, +, \hat{v}(S_t, \mathbf{w_t}), v_\pi(S_t)$

**Đáp án đúng: B, C** [Inference]

_Ghi chú: Coursera xác nhận D sai (feedback: update tỉ lệ với gradient âm của bình phương sai số). w − ½α∇[v_π − v̂]² = w + α[v_π − v̂]∇v̂ (C). Đảo thứ tự trong ngoặc vuông cũng cho kết quả tương đương: w − α[v̂ − v_π]∇v̂ (B)._

## Câu 98

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

In a Monte Carlo Update with function approximation, we do stochastic gradient descent using the following gradient: $\nabla[G_t - \hat{v}(s,\mathbf{w})]^2 = 2 [G_t - \hat{v}(s, \mathbf{w})]\nabla (-\hat{v}(S_t, \mathbf{w}_t))$ $\quad\quad\quad\qquad\quad= (-1)*2 [G_t - \hat{v}(s, \mathbf{w})]\nabla \hat{v}(S_t, \mathbf{w}_t)$ But the actual Monte Carlo Update rule is the following: $\mathbf{w_{t+1}} = \mathbf{w_t} + \hspace{0.25em} \alpha [G_t - \hat{v}(S_t, \mathbf{w}_t) ] \nabla \hat{v}(S_t, \mathbf{w}_t), \quad\quad (\alpha >0)$ Where did the constant -1 and 2 go when $\alpha$ is positive? (Choose all that apply)

- A. We assume that the 2 is included in $\nabla \hat{v}(S_t, \mathbf{w}_t)$ .
- B. We are performing gradient descent, so we subtract the gradient from the weights, negating -1.
- C. We are performing gradient ascent, so we subtract the gradient from the weights, negating -1.
- D. We assume that the 2 is included in the step-size.

**Đáp án đúng: B, D**

## Câu 99

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

When using stochastic gradient descent for learning the value function, why do we only make a small update towards minimizing the error instead of fully minimizing the error at each encountered state?

- A. Because we want to minimize approximation error for all states, proportionally to $\mu$ .
- B. Because small updates guarantee we can slowly reduce approximation error to zero for all states.
- C. Because the target value may not be accurate initially for both TD(0) and Monte Carlo method.

**Đáp án đúng: A**

## Câu 100

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_

The general stochastic gradient descent update rule for state-value prediction is as follows: $\mathbf{w_{t+1}} \doteq \mathbf{w_t} + \alpha [U_t - \hat{v}(S_t, \mathbf{w_t})] \nabla \hat{v}(S_t,\mathbf{w_t})$ For what values of $U_t$ would this be a semi-gradient method?

- A. $v_\pi(S_t)$
- B. $R_{t+1} + \hat{v}(S_{t+1}, w_t)$
- C. $R_{t+1} + R_{t+2} + … + R_T$
- D. $G_t$

**Đáp án đúng: B**

## Câu 101

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following statements is true about state-value prediction using stochastic gradient descent? $\mathbf{w_{t+1}} \doteq \mathbf{w_t} + \alpha [U_t - \hat{v}(S_t, \mathbf{w_t})] \nabla \hat{v}(S_t,\mathbf{w_t})$ (Select all that apply)

- A. Using the Monte Carlo return as target, and under appropriate stochastic approximation conditions, the value function will converge to a local optimum of the Mean Squared Value Error.
- B. Using the Monte Carlo return or true value function as target results in an unbiased update.
- C. When using $U_t = R_{t+1} +\hat{v}(S_{t+1},\mathbf{w_t})$ , the weight update is not using the true gradient of the TD error.
- D. Stochastic gradient descent updates with Monte Carlo targets always reduce the Mean Squared Value Error at each step.
- E. Semi-gradient TD(0) methods typically learn faster than gradient Monte Carlo methods.

**Đáp án đúng: A, B, C, E**

_Ghi chú: Coursera xác nhận A, C, E đúng và báo còn thiếu đáp án. D sai vì SGD không "always" giảm MSVE ở mỗi bước, nên đáp án còn thiếu là B (MC return / true value là target không chệch) [Inference]._

## Câu 102

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about the TD fixed point? (Select all correct answers)

- A. Semi-gradient TD(0) with linear function approximation converges to the TD fixed point.
- B. The weight vector corresponding to the TD fixed point is a local minimum of the Mean Squared Value Error.
- C. The weight vector corresponding to the TD fixed point is the global minimum of the Mean Squared Value Error.
- D. At the TD fixed point, the mean squared value error is not larger than $\frac{1}{1-\gamma}$ times the minimal mean squared value error, assuming the same linear function approximation.

**Đáp án đúng: A, D**

## Câu 103

_Nguồn: C3 – On-policy Prediction with Approximation (92.08%)_ · _chọn nhiều đáp án_

Which of the following is true about Linear Function Approximation, for estimating state-values? (Select all that apply)

- A. The size of the feature vector is not necessarily equal to the size of the weight vector.
- B. The gradient of the approximate value function $\hat{v}(s, \mathbf{w})$ with respect to $\mathbf{w}$ is just the feature vector.
- C. State aggregation is one way to generate features for linear function approximation.

**Đáp án đúng: B, C**

## Câu 104

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about coarse coding? (Select all that apply)

- A. In coarse coding, generalization occurs between states that have features with overlapping receptive fields.
- B. In coarse coding, generalization between states depend on the size and shape of the receptive fields.
- C. When using features with large receptive fields, the function approximator cannot make discriminations that are finer than the width of the receptive fields.
- D. When training at one state, the learned value function will be updated over all states within the intersection of the receptive fields.

**Đáp án đúng: A, B**

_Ghi chú: Coursera xác nhận A, B đúng; C, D "should not be selected". Độ phân giải tăng được khi thêm feature; khi train, value được cập nhật trên hợp (union) các receptive field, không phải giao (intersection)._

## Câu 105

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Consider a continuous two-dimensional state space. Assuming linear function approximation with the coarse-codings in either A, B or C, which of the following is TRUE? (Select all that apply) [hình]

- A. Generalization is broader in case A as compared to case B.
- B. In case B, when updating the state marked by an ‘x’ , the value function will be affected for a larger number of states as compared to case A.
- C. In case C, each update results in more generalization along the vertical dimension, as compared to horizontal dimension.
- D. In case C, each update results in more generalization along the horizontal dimension, as compared to vertical dimension.

**Đáp án đúng: B, C**

## Câu 106

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following affects generalization in tile coding? (Select all that apply)

- A. The number of tiles.
- B. The number of tilings.
- C. How the tilings are offset from each other.
- D. The shape of the tiles.

**Đáp án đúng: A, B, C, D**

_Ghi chú: Coursera xác nhận B, C, D đúng và báo còn thiếu, nên A cũng đúng._

## Câu 107

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

When tile coding is used for feature construction, the number of active or non-zero features

- A. is the number of tiles.
- B. is the number of tilings.
- C. is the number of tilings multiplied by the number of tiles.
- D. depends on the state.

**Đáp án đúng: B**

## Câu 108

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about neural networks (NNs) ? (Select all that apply)

- A. A NN is feedforward if there are no paths within the network by which a unit’s output can influence its input.
- B. Hidden layers are layers that are neither input nor output layers.
- C. The output of the units in NNs are typically a linear function of their input signals.
- D. NNs are parameterized functions that enable the agent to learn a nonlinear value function of state.
- E. The nonlinear functions applied to the weighted sum of the input signals are called the activation function.

**Đáp án đúng: A, B, D, E**

## Câu 109

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

Which of the following is the rectified linear activation function?

- A. $f(x) = \frac{1}{1 + e^{-x}}$
- B. $f(x) = 1$ if $x>0$ and $0$ otherwise
- C. $f(x) = max(0,x)$
- D. $f(x) = \frac{e ^{x} - e ^{-x}}{e ^{x} +e ^{-x}}$

**Đáp án đúng: C**

## Câu 110

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following are TRUE statements? (Select all that apply)

- A. A disadvantage of linear function approximation methods like tile coding is that they are linear in the input state.
- B. NNs are powerful function approximators and can learn accurate value functions, but typically require many samples to train.
- C. An advantage of linear methods is that they can be more data efficient than NNs, but they rely on an expert to design the features appropriately.
- D. An advantage of NNs is that learning can adapt the features, as compared to methods like tile coding.

**Đáp án đúng: B, C, D**

## Câu 111

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about backpropagation? (Select all that apply)

- A. Backpropagation corresponds to updating the parameters of a neural network using gradient descent.
- B. Backpropagation involves computing the partial derivatives of an objective function with respect to the weights of the network.
- C. The forward pass in backpropagation updates the weights of the network using the partial derivatives computed by the backward passes.
- D. Backpropagation computes partial derivatives starting from the last layer in the network, to save computation.

**Đáp án đúng: A, B, D**

_Ghi chú: Coursera xác nhận B, D đúng và báo còn thiếu. C sai vì forward pass không cập nhật trọng số, nên đáp án còn thiếu là A [Inference]._

## Câu 112

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Training neural networks (NNs) with backpropagation can be challenging because (Select all that apply)

- A. the loss surface might have flat regions, or poor local minima, meaning gradient descent gets stuck at poor solutions.
- B. the initialization can have a big impact on how much progress the gradient updates can make and on the quality of the final solution.
- C. neural networks cannot accurately represent most functions, so the loss stays large.
- D. learning can be slow due to the vanishing gradient problem, where if the partial derivatives for later nodes in the network are zero or near zero then this causes earlier nodes in the network to have small or near zero gradient updates.

**Đáp án đúng: A, B, D**

## Câu 113

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_

Consider the following network: [hình] where for a given input $s$ , value of $s$ is computed by: $\psi = sW^{[0]} + b^{[0]}$ $x = \textit{max}(0, \psi)$ $v = xW^{[1]} + b^{[1]}$ What is the partial derivative of $v(s)$ with respect to $W^{[0]}_{ij}$ ?

- A. $s_i$
- B. $W^{[1]}_js_i$ if $x_j > 0$ and $0$ otherwise
- C. $x_j$
- D. $W^{[1]}_jx_j$ if $x_j > 0$ and $0$ otherwise

**Đáp án đúng: B**

## Câu 114

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE? (Select all that apply)

- A. When using stochastic gradient descent, we often completely eliminate the error for each example.
- B. The difference between stochastic gradient descent methods and batch gradient descent methods is that in the former the weights get updated using one random example whereas in the latter they get updated based on batches of data.
- C. Adagrad, Adam, and AMSGrad are stochastic gradient descent algorithms with adaptive step-sizes.
- D. Setting the step-size parameter for stochastic gradient descent can be challenging because a small step-size makes learning slow and a large step-size can result in divergence.

**Đáp án đúng: B, C, D**

## Câu 115

_Nguồn: C3 – Constructing Features for Prediction (83.33%)_ · _chọn nhiều đáp án_

Which of the following is TRUE about artificial neural networks (ANNs)? (Select all that apply)

- A. It is best to initialize the weights of a NN to large numbers so that the input signal does not get too small as it passes through the network.
- B. It is best to initialize the weights of a NN to small numbers so that the input signal does not grow rapidly as it passes through the network.
- C. If possible, it would be best to initialize the weights of an NN near the global optimum.
- D. A reasonable way to initialize the NN is with random weights, with each weight sampled from a normal distribution with the variance scaled by the number of inputs to the layer for that weight.

**Đáp án đúng: C, D**

_Ghi chú: Coursera xác nhận C, D đúng; B "should not be selected" (khởi tạo nhỏ làm tín hiệu teo lại, học chậm). A không chọn [Inference: khởi tạo quá lớn cũng không tốt]._

## Câu 116

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following are true? (Select all that apply)

- A. In the tabular case, updating the value of one state does not affect the values of other states.
- B. When using state aggregation or coarse coding, updating the value of one state does not affect the values of other states.
- C. When using state aggregation or coarse coding, there is generalization across states.
- D. In the tabular case, there is generalization across states, i.e., updates to the value function of one state influences the value function of other states.

**Đáp án đúng: A, C**

## Câu 117

_Nguồn: C3 – Control with Approximation (83.33%)_

To turn the update of Expected Sarsa algorithm to the update of Q-learning, one must:

- A. Use a neural network to approximate the action-value function.
- B. Expected Sarsa cannot be adapted to represent Q-learning.
- C. Use the maximum over all the actions instead of the expectation in the update function.
- D. Behave greedily with respect to the action-value function.

**Đáp án đúng: C**

## Câu 118

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following are true:

- A. Exploration is not a problem when using function approximation because learning generalizes across states and actions.
- B. When using function approximation, Q-learning will always result in better performance than Sarsa and Expected Sarsa.
- C. When using function approximation and with discrete actions, there is no straightforward way to turn Sarsa into Expected Sarsa.
- D. When learning value functions in the mountain car domain and using tiile coding, where all the rewards are -1 except when the terminal state is reached, initializing the weights of a linear function approximation to zero is an example of optimistic initialization.

**Đáp án đúng: D**

## Câu 119

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following statements about discounted return and differential return algorithms are true:

- A. There is a set of Bellman equations for the value function corresponding to the discounted return. However, there is no set of Bellman equations for differential value functions.
- B. The performance of discounted return algorithms can suffer because the optimal value of gamma is problem dependent.
- C. Algorithms that maximize the discounted return can suffer from an exponentially large variance when using a large discount factor.

**Đáp án đúng: B, C**

## Câu 120

_Nguồn: C3 – Control with Approximation (83.33%)_

Imagine we have 7 state features and 6 actions and we want to use linear function approximation to compute the action-value function. If we use feature stacking (as explained in Week 3), how many features would we need in total to approximate the action-value function of all the different actions?

- A. 67
- B. 13
- C. 42
- D. 76

**Đáp án đúng: C**

## Câu 121

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Imagine we are approximating the action-value function of three different actions (red, green, and blue) using three state features, resulting in the following weights and features: [hình] Which of these statements is true about our function approximation scheme?

- A. The green action will never be selected.
- B. The action-value of the green action will be exactly the same as the action-value of the red action for any state.
- C. There will not be any generalization across states.
- D. The action-value of the red action will be exactly the same as the action-value of the blue action.

**Đáp án đúng: B**

## Câu 122

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following feature and weight vectors corresponding to three state features and three actions (red, green, and blue): [hình] What is the approximate action-value for the blue action?

- A. 12
- B. 42
- C. 16
- D. 53

**Đáp án đúng: C**

## Câu 123

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Which of the following statements about epsilon-greedy policies and optimistic initialization are true:

- A. Implementing optimistic initialization is always straightforward and simple to implement regardless of the function approximation technique.
- B. Optimistic initialization results in a more systematic exploration in the tabular case because the agent takes actions it has not taken as often in a state.
- C. Optimistic initialization is always preferred over using an epsilon-greedy policy.
- D. Epsilon-greedy can be easily combined with any function approximation technique because it only needs to be able to query for the approximate action-values, without needing to know how they are initialized or computed.

**Đáp án đúng: B, D**

## Câu 124

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

Consider the mountain car environment where all the rewards are -1 after every action until reaching the flag on top of the right hill: [hình] Which of the following are examples of optimistic initialization when using linear function approximation?

- A. Initialize all the weights at random using a uniform distribution between -5 and 5.
- B. Initialize all the weights so that the action-value function is -1 everywhere.
- C. Initialize all the weights so that the action-value function is zero everywhere.
- D. Initialize all the weights so that the action-value function is 10 everywhere.

**Đáp án đúng: C, D**

## Câu 125

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following MDP where the red action (L) at state S results in an immediate reward of +1 and 0 afterwards, and the blue action (R) results in 0 immediate reward, but a final reward of +2 when returning to state S. [hình] In this MDP, what is the optimal policy at state S when using discounted return with a value of gamma of 0.5? When using discounted return with a value of gamma of 0.9? When using average reward? (Hint: You can modify the equations used for the task from lesson 3 of this module to get the solution)

- A. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, red action; average reward, blue action.
- B. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, red action; average reward, red action.
- C. The optimal policy is: gamma = 0.5, red action; gamma = 0.9, blue action; average reward, blue action.
- D. The optimal policy is: gamma = 0.5, blue action; gamma = 0.9, blue action; average reward, red action.

**Đáp án đúng: C** [Inference]

_Ghi chú: Coursera xác nhận A sai. Mỗi vòng dài 4 bước. Red: G = 1/(1−γ⁴); Blue: G = 2γ³/(1−γ⁴). γ=0.5: 1 > 0.25 → red. γ=0.9: 1 < 1.458 → blue. Average reward: blue 2/4 > red 1/4 → blue._

## Câu 126

_Nguồn: C3 – Control with Approximation (83.33%)_

Consider the following MDP with two states. State 1 has two actions: staying in the same state (blue) and switching to the other state (red). State 2 has a single (red) action leading to State 1. The rewards are listed next to each arrow/transition. [hình] If the agent is following a policy that takes the blue and red actions with equal probability, what is the average reward? (Hint: the state visitation probability is ⅔ for state 1 and ⅓ for state 2, the target policy probability \pi is the random policy, and all the transitions p are deterministic) Recall the formula is: [hình]

- A. Average reward = 3/4
- B. Average reward = 2
- C. Average reward = 1
- D. Average reward = 4/3

**Đáp án đúng: D** [Inference]

_Ghi chú: Coursera xác nhận A sai. Hình: blue (1→1) +1, red (1→2) +0, red (2→1) +3. r(π) = ⅔·(½·1 + ½·0) + ⅓·3 = ⅓ + 1 = 4/3._

## Câu 127

_Nguồn: C3 – Control with Approximation (83.33%)_ · _chọn nhiều đáp án_

For which of the following tasks is the average reward setting preferable than the discounted return setting if we are interested in maximizing the total amount of reward?

- A. The nearsighted MDP from Week 3. The agent starts at an initial state S that splits into two paths, each leading to a ring that leads back to S after some time. If the agent chooses the left ring, it observes and immediate reward of +1 followed by 0 rewards, whereas choosing the right ring results on immediate reward of 0, but a final reward of +2 when returning to state S.
- B. An Atari 2600 game where the agent can keep playing until it loses all its lives, which are a finite amount.
- C. The job scheduling task from Section 10.3 of Sutton and Barto's RL textbook. The agent manages how jobs are scheduled into three different servers according to the priority of each job. When the agent accepts a job, the job runs in one of the servers and the agent gets a positive reward equal to the priority of the job, whereas when the agent rejects a job, the job returns to the queue and the agent receives a negative reward proportional to the priority of the job. The servers become available as they finish their jobs. Jobs are continually added to the queue and the agent accepts or rejects them.
- D. The episodic mountain car environment.

**Đáp án đúng: A, C**

## Câu 128

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is true about policy gradient methods? (Select all that apply)

- A. Policy gradient methods use generalized policy iteration to learn policies directly.
- B. Policy gradient methods do gradient ascent on the policy objective.
- C. If we have access to the true value function $v_\pi$ , we can perform unbiased stochastic gradient updates using the result from the Policy Gradient Theorem.
- D. The policy gradient theorem provides a form for the policy gradient that does not contain the gradient of the state distribution $\mu$ , which is hard to estimate.

**Đáp án đúng: B, C, D**

## Câu 129

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements about parameterized policies are true? (Select all that apply)

- A. The policy must be approximated using linear function approximation.
- B. The function used for representing the policy must be a softmax function.
- C. The probability of selecting any action must be greater than or equal to zero.
- D. For each state, the sum of all the action probabilities must equal to one.

**Đáp án đúng: C, D**

## Câu 130

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

Assume you’re given the following preferences $h_1 = 44$ , $h_2 = 42$ , and $h_3 = 38$ , corresponding to three different actions ( $a_1, a_2, a_3$ ), respectively. Under a softmax policy, what is the probability of choosing $a_2$ , rounded to three decimal numbers?

- A. 0.119
- B. 0.42
- C. 0.002
- D. 0.879

**Đáp án đúng: A**

## Câu 131

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is true about softmax policy? (Select all that apply)

- A. Similar to epsilon-greedy policy, softmax policy cannot approach a deterministic policy.
- B. It cannot represent an optimal policy that is stochastic, because it reaches a deterministic policy as one action preference dominates others.
- C. It is used to represent a policy in discrete action spaces.
- D. It can be parameterized by any function approximator as long as it can output scalar values for each available action, to form a softmax policy.

**Đáp án đúng: C, D**

## Câu 132

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

What are the differences between using softmax policy over action-values and using softmax policy over action-preferences? (Select all that apply)

- A. When using softmax policy over action-values, assuming a tabular representation, the policy will converge to the optimal policy regardless of whether the optimal policy is stochastic or deterministic.
- B. When using softmax policy over action-preferences, assuming a tabular representation, the policy will converge to the optimal policy regardless of whether the optimal policy is stochastic or deterministic.
- C. When using softmax policy over action-values, even if the optimal policy is deterministic, the policy may never approach a deterministic policy.

**Đáp án đúng: B, C**

## Câu 133

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

What is the following objective, and in which task formulation? $\Large r(\pi) = \Sigma_s \mu(s) \Sigma_a \pi(a|s, \mathbf{\theta}) \Sigma_{s’, r} p(s’, r | s, a) r$

- A. Average reward objective, episodic task
- B. Average reward objective, continuing task
- C. Discounted return objective, continuing task
- D. Undiscounted return objective, episodic task

**Đáp án đúng: B**

## Câu 134

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

The following equation is the outcome of the policy gradient theorem. Which of the following is true about the policy gradient theorem? (Select all that apply) $\Large \nabla r(\pi) = \Sigma_s \mu(s) \Sigma_a \nabla \pi(a|s, \mathbf{\theta}) q_{\pi} (s,a)$

- A. We do not need to compute the gradient of the state distribution $\mu$ .
- B. This expression can be converted into: $\large \mathbb{E}_\pi[\Sigma_a \nabla\pi(a|S, \mathbf{\theta})q_\pi(S,a)]$ In discrete action space, by approximating q_pi we could also use this gradient to update the policy.
- C. The true action value $q_\pi$ can be approximated in many ways, for example using TD algorithms.
- D. This expression can be converted into the following expectation over $\pi$ : $\large \mathbb{E}_\pi [\nabla \ln \pi (A|S, \theta) q_{\pi} (S,A)]$

**Đáp án đúng: A, B, C, D**

## Câu 135

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements is true? (Select all that apply)

- A. The Actor-Critic algorithm consists of two parts: a parameterized policy — the actor — and a value function — the critic.
- B. Subtracting a baseline in the policy gradient update tends to reduce the variance of the update, which results in faster learning.
- C. TD methods do not have a role when estimating the policy directly.
- D. To update the actor in Actor-Critic, we can use TD error in place of $q_\pi$ in the Policy Gradient Theorem.

**Đáp án đúng: A, B, D**

## Câu 136

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

To train the critic, we must use the average reward version of semi-gradient TD(0).

- A. True
- B. False

**Đáp án đúng: B**

## Câu 137

_Nguồn: C3 – Policy Gradient Methods (91.66%)_

Consider the following state features and parameters $\theta$ for three different actions (red, green, and blue): [hình] Compute the action preferences for each of the three different actions using linear function approximation and stacked features for the action preferences.What is the action preference of $a_1$ (green)?

- A. 42
- B. 40
- C. 35
- D. 32

**Đáp án đúng: A**

## Câu 138

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following statements are true about the Actor-Critic algorithm with softmax policies? (Choose all that apply)

- A. The preferences must be approximated using linear function approximation.
- B. Since the policy is written as a function of the current state, it is like having a different softmax distribution for each state.
- C. The actor and the critic share the same set of parameters.
- D. The learning rate parameter of the actor and the critic can be different.

**Đáp án đúng: B, D**

## Câu 139

_Nguồn: C3 – Policy Gradient Methods (91.66%)_ · _chọn nhiều đáp án_

Which of the following is an advantage of Gaussian policy parameterization over discretizing the action space? (Select all that apply)

- A. Gaussian policies are differentiable, whereas policies over discretized actions are not.
- B. Continuous actions also allow learning to generalize over actions.
- C. Even if the true action set is discrete, but very large, it might be better to treat them as a continuous range.
- D. There might not be a straightforward way to choose a discrete set of actions.

**Đáp án đúng: B, C, D**

_Ghi chú: Coursera xác nhận B, C, D đúng; A "should not be selected" (softmax trên action rời rạc vẫn khả vi)._

## Câu 140

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a control setting in which updates will be made at every time step? [Select all that apply]

- A. Expected SARSA
- B. SARSA
- C. Q-learning

**Đáp án đúng: A, B, C**

## Câu 141

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a prediction setting in which updates will be made at the end of each episode? [Select all that apply]

- A. Monte-Carlo Prediction
- B. Exploring Starts Monte-Carlo
- C. Off-Policy Monte-Carlo

**Đáp án đúng: A, C**

## Câu 142

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a tabular setting in which we will be learning a model and using it for planning? [Select all that apply]

- A. Expected SARSA
- B. Dyna-Q
- C. Dyna-Q+

**Đáp án đúng: B, C**

## Câu 143

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a control setting in which we are given access to a model? [Select all that apply]

- A. Iterative Policy Evaluation
- B. Policy Iteration
- C. Value Iteration
- D. Dyna-Q

**Đáp án đúng: B, C, D**

## Câu 144

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in a continuing control setting with a discrete action space and function approximation? [Select all that apply]

- A. Gaussian Actor-Critic
- B. Differential Softmax Actor-Critic
- C. Differential Semi-Gradient SARSA

**Đáp án đúng: B, C**

## Câu 145

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate in an online prediction setting with linear function approximation? [Select all that apply]

- A. Semi-Gradient TD
- B. Gradient Monte Carlo
- C. SARSA

**Đáp án đúng: A**

## Câu 146

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

In the continuing acrobot system (shown below), a double pendulum is fixed to the red square. The goal is to swing the double pendulum such that the height of the mass on the end of the lower pendulum exceeds the height of the black line. When the goal is reached, a reward of one is given and the double pendulum transitions to a vertical position. Otherwise, the reward is zero. Which of the following algorithms are appropriate for control in this context? [Select all that apply] [hình]

- A. Expected SARSA
- B. Q-learning
- C. Average Reward Actor-Critic

**Đáp án đúng: C**

## Câu 147

_Nguồn: C4 – Choosing the Right Algorithm (100%)_ · _chọn nhiều đáp án_

Which of the following algorithms are appropriate for control in the lunar lander MDP, as it is described in the lecture “Initial Project Meeting with Martha: Formalizing the Problem”? [Select all that apply]

- A. Expected SARSA
- B. Q-learning
- C. Average Reward Actor-Critic

**Đáp án đúng: A, B**

## Câu 148

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following meta-parameters can be tuned to improve performance of the agent? Performance refers to the cumulative reward the agent would receive in expectation across different runs. (Select all that apply)

- A. Random seed (for the random number generator)
- B. Exploration parameter (e.g., epsilon in e-greedy or the temperature tau in the softmax policy)
- C. The step size in the update rule of the learning algorithm (e.g., alpha in Q-learning)
- D. Number of hidden-layer units in a neural network approximating the value function

**Đáp án đúng: B, C, D**

## Câu 149

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

Suppose a problem that you have formulated as an MDP has k continuous input dimensions. You are considering using tile coding as a function approximator. With T tilings and t tiles per dimension in each tiling, which of the following represent the resultant number of features? (Assume each tiling covers all k dimensions.)

- A. T∙t^k
- B. k∙T^t
- C. T ∙ t / k
- D. T ∙ t ∙ k

**Đáp án đúng: A**

## Câu 150

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements regarding feature-construction methods are TRUE? (Select all that apply)

- A. A simple implementation of tile coding leads to memory requirements that might be exponential in the number of features.
- B. The feature representation obtained using neural networks changes with time.
- C. The feature representation obtained using tile coding changes with time.
- D. In low-dimensional problems, tile coding is computationally efficient and provides good generalization and discrimination.

**Đáp án đúng: A, B, D**

## Câu 151

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Adding more hidden layers (of a fixed finite width) increases the representation capacity of neural network. For example, if you have a single-hidden layer neural network with 16 units and nonlinear activations, then adding another layer of 16 units to get a neural network with two hidden layers can represent more functions.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 152

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Adding more hidden layers to a neural network increases the number of parameters needed to be learned.

- A. True
- B. False

**Đáp án đúng: A**

## Câu 153

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements regarding the exploration approach are TRUE? (Select all that apply)

- A. A softmax policy is a limited strategy for exploration because it can only be used with action preferences and policy-gradient methods.
- B. Optimistic initial values are difficult to maintain when using neural networks as a function approximator.
- C. Epsilon-greedy exploration is difficult to combine with neural networks.
- D. Both optimistic initial values and epsilon-greedy exploration can be easily used with neural networks, because they are simple exploration strategies.

**Đáp án đúng: B**

## Câu 154

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following are TRUE about the softmax temperature parameter tau?

- A. Tau does not affect the exploration at all.
- B. For very small tau, the agent mostly selects the greedy action.
- C. For very large tau, the agent’s policy is nearly a uniformly-random policy.
- D. If tau is large, the agent’s policy is more stochastic.

**Đáp án đúng: B, C, D**

## Câu 155

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements are true about activation functions? (Select all that apply)

- A. The gradient of flat regions in the range of an activation function w.r.t. the input is zero.
- B. Linear activation functions (such as f(x)=x) have derivatives close to zero for inputs of large magnitude.
- C. Rectified Linear Units (ReLUs) are linear activation functions.
- D. For inputs of large magnitude, the derivative of the sigmoid and tanh functions are close to zero.

**Đáp án đúng: A, D**

## Câu 156

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

Consider you are using a neural network to approximate the action-value function of a reinforcement learning agent. You decide to use a neural network with two hidden layers. Now you want to choose the activation function for the hidden layers and the output layer. One option is to use a neural network with tanh activation functions in both hidden layers, and a linear activation in the output layer. Another option is to use a neural network with linear activations in both the hidden layers and the output layer. True or False: In both cases (option one and option two), the neural network can represent the same class of action-value functions.

- A. True
- B. False

**Đáp án đúng: B**

## Câu 157

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Which of the following statements are TRUE regarding methods for selecting a stepsize for the learning update?

- A. A stepsize that reduces over time (such as 1/N, where N is the number of agent-environment interactions) is necessary when the environment changes over time.
- B. An adaptive stepsize selection method like RMSProp uses a heuristic to change the stepsize during learning.
- C. The heuristic to change the stepsize can be learned from the data collected from the agent-environment interactions.

**Đáp án đúng: B, C**

## Câu 158

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_ · _chọn nhiều đáp án_

Suppose we want to find the optimal policy that obtains the maximum undiscounted return per episode in some task. We are using Expected Sarsa. With the rest of the meta-parameters fixed, we want to find the best setting of the stepsize that results in the best performance in this setting. In the following graph, the blue line represents how the performance measure varies with stepsize. Obviously, we do not have this information beforehand, and we are selecting a range of stepsizes to try out with our agent. Which of the following graphs best represent the range of stepsizes that should be tried out for a given experiment? (the orange points represent the selected stepsizes)

- A. [hình]
- B. [hình]
- C. [hình]

**Đáp án đúng: B**

## Câu 159

_Nguồn: C4 – Impact of Parameter Choices in RL (100%)_

True or False: Epsilon-greedy exploration uses information from all the action values of a particular state when choosing a non-greedy action in that state.

- A. False
- B. True

**Đáp án đúng: A**
