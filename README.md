# fBM + GARCH Path Generation

Generate realistic price paths using fractional Brownian motion seeded with GARCH characteristics.

## Purpose
- Improve realism of synthetic time series
- Match stylized facts like fat tails and volatility clustering
- GARCH model: HAR, Student-t GARCH(1,1,1)
- converts returns back to prices to see how it matches real data

## Modules
- `fbm_simulator.py`: Generate fBM paths matching statistical properties

## Example Output
Compare synthetic and real return distributions:
<p align="center">
  <img src="simulations/dist_comparison.png" width="500">
</p>

## Usage
```bash
python models/fbm_simulator.py --config config.yaml
