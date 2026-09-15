Multi-agents
    - current state of multi-agents (what's in, what's out)
        - durable surface routing with agent requested hand-off (server orchestrated agent routing)


boudnaries (prompt, tools, application code)
    - prompt - instructions
    - tools - data / state, (tools should never output instructions, can cause behavior being not audiable, also weaker controls)
    - context as prefetched when always needed, tools if cannot predicted
    - tools 
    - authorize whatever entitites the model gets to choose.

agent loop
    - what kind of retries (tool level, agent level, what kind of idempotency guarantee)

cost
    - output 5x > input, brievity 
    - structured code when the consumer is code
    - prompt caching
    - **do not routing data through the model!!**

Eval/testing