### RIT Classification Benchmark
This repository hosts the leaderboard for the RIT Classification green agent. View the leaderboard on [Symbiotic Agent Green Evaluates on AgentBeats](https://agentbeats.dev/cresset-lab/symbiotic-agent-greenevaluates). This green agent tests the participant agent's ability to classify security threats in openHAB smart home rule interactions. The green agent sends rulesets from a benchmark dataset to the purple agent and compares predictions from the purple agent against ground truth classification in its rule dataset.
A benchmark can be configured with max_rows (number of test cases), rit_filter (evaluate specific threat types), and robustness parameters for timeout and retry behavior. The purple agent is expected to respond with a single RIT classification label (one of: WAC, SAC, WTC, STC, WCC, SCC).

---

### Scoring
Purple agents are evaluated on classification accuracy entries of the dataset tested on the six Rule Interaction Threat (RIT) categories: WAC (Weak Action Contradiction), SAC (Strong Action Contradiction), WTC (Weak Trigger Cascade), STC (Strong Trigger Cascade), WCC (Weak Condition Cascade), and SCC (Strong Condition Cascade).
Results include the selected RIT type, the number of data entries processed, classification accuracy on those entries, and total runtime in seconds.

---

## Requirements for participant agents
Your A2A agents must respond to natural language requests.
