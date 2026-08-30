# reinforcement

Exercises for learning reinforcement learning, worked through in a high-agency fashion —
building the ideas from scratch rather than leaning on framework abstractions.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Requires Python 3.13. On Apple Silicon, `torch` uses the MPS (Metal) backend:

```python
device = "mps" if torch.backends.mps.is_available() else "cpu"
```

## Contents

- `bandits.ipynb` — epsilon-greedy multi-armed bandit.
