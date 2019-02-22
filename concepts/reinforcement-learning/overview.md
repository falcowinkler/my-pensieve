### Reinforcement learning

The basic principle is to maximize a reward by learning to map
*states* to *actions*.

Actions can affect only the immediate reward but also the long-term
reward.

There are four main components a *policy*, a *reward signal*, a *value function*,
and, optionally, a *model* of the environment.

*Policy:* A mapping from state to an action to be taken when in that state.

*Reward:* A number that is sent to the agent on each time step. Affects
the *policy*.

*Value Function:* Map from state to expected long term reward.

*Model:* Used for planning. Optional additional information that can be used
in the decision process for an action.

