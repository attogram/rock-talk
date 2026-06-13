# Example: Agentic Coordination and Semantic Drift

In Multi-Agent Systems (MAS), instructions are often passed through multiple "hops" (Sub-agents). Standard prose introduces linguistic noise at each hop, increasing the probability of "Semantic Drift"—where the final agent receives a distorted version of the original intent.

| Standard Multi-Agent Handover | Rock Talk Handover |
| :--- | :--- |
| **Agent A to Agent B** | **Agent A to Agent B** |
| "I've analyzed the user request and it seems we need to implement a new authentication middleware. Could you please take a look at the `auth.py` file and see if we can add a JWT validation step before the request hits the main handler? Make sure it handles expired tokens gracefully." | Task: Auth middleware. Target: `auth.py`. Action: Add JWT validation. Requirement: Pre-handler. Edge case: Handle expired tokens. |
| **Agent B to Agent C (Sub-task)** | **Agent B to Agent C (Sub-task)** |
| "Agent A wants us to update the authentication. I need you to write a helper function in a new file that validates JWTs. It should return a boolean. If the token is expired, it should probably throw an error or something so the middleware knows." | Sub-task: JWT validator. Input: JWT. Output: Boolean. Edge: Expired = Error. New file. |
| **Agent C Execution (Potential Drift)** | **Agent C Execution (High Signal)** |
| *Agent C might focus on "throwing an error" and implement a generic Exception that crashes the service, or forgets the "middleware" context because the instruction was buried in "Could you please...".* | *Agent C has a checklist of data. No ambiguity. Direct mapping from instruction to code logic.* |
| **Result** | **Result** |
| High risk of "Instruction Bloat" and semantic decay. | Low surface area for error. 1:1 mapping of intent. |
