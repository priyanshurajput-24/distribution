# 1. `random.binomialvariate`

The `rd.binomialvariate(n, p)` method from Python’s `random` module generates a binomial random variable, i.e., the number of successes in `n` independent trials with success probability `p`.

- **Mean:** `E[X] = n * p`
- **Variance:** `Var[X] = n * p * (1 - p)`

### Example

```python
l = [rd.binomialvariate(55, 0.3946) for _ in range(50000)]
total_trials = 50000 * 55  # 2,750,000
empirical_p = sum(l) / total_trials  # ≈ 0.394712
mean = 55 * 0.3946 = 21.758
Variance = 55 * 3946 * (1 - 3946) = 13.1389

