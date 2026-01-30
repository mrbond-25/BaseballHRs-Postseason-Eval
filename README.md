# BaseballHRs-Postseason-Eval
A project evaluating my mid-season predictions for the 2025 Cleveland Guardians' number of home runs (HRs).

## Data
Data consists of MLB regular season game logs from 2024 and 2025, from [retrosheet](https://www.retrosheet.org/gamelogs/index.html).

## Methods
In my original [blog post](https://mikeystats.wordpress.com/2025/05/18/how-many-home-runs-will-the-guardians-hit-today/), I used a Poisson model for the number of HRs hit per game, and used PyMC to sample the posterior distribution of the Poisson rate under various priors. This project mostly concerns the accuracy of my predictions, but I also repeat the posterior sampling with the full-season data to create a final estimate for the Poisson rate's distrubtion. For this, I use a Gamma(16,14) prior, as discussed in my earlier post.