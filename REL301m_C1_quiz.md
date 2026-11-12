# REL301m – C1: Fundamentals of Reinforcement Learning – Quiz Coursera

Nguồn: trang "View feedback" của lượt nộp gần nhất trên Coursera (chỉ đọc, không nộp lượt mới). Câu hỏi/lựa chọn giữ nguyên tiếng Anh; công thức dạng LaTeX `$...$`. `[hình]` = câu có hình minh họa không trích được. Các câu ở lượt cuối bị chấm sai/chưa đủ đã được bổ sung đáp án từ feedback từng lựa chọn của Coursera và/hoặc tự giải; phần tự suy luận được gắn **[Inference]** và có giải thích trong _Ghi chú_.

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
