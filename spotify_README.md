# What Makes a Song Popular? — Spotify EDA

An exploratory data analysis of **32,833 Spotify tracks** using Python (pandas, seaborn), investigating which audio features are associated with a song's popularity.

> *Dataset: [TidyTuesday Spotify songs](https://github.com/rfordatascience/tidytuesday/tree/master/data/2020/2020-01-21) (32,833 tracks, 23 columns). Originally built as a graduate data science EDA assignment.*

## Question

Which characteristics of a track — danceability, energy, valence, tempo, duration, genre, or musical mode — relate to how popular it is?

## Approach

Explored and cleaned the data, selected seven features with a plausible link to popularity, **logit-transformed** the 0–100 popularity score for continuous analysis, then examined each feature's marginal distribution and its relationship to popularity, both individually and grouped by genre and mode.

## Key findings

- **Shorter songs tend to be more popular** — track duration has the clearest (negative) relationship of any audio feature, holding across genres.
- **Danceability is weakly positive; energy is weakly negative** — both small effects.
- **Tempo and valence show no meaningful relationship** with popularity.
- **Genre has a slight edge** (Pop and Latin skew more popular); **mode has none on its own**, but interacts with genre — pop/rap/rock do better in minor, edm/latin/r&b in major.
- **No single strong driver** — popularity comes from a combination of small influences.

## Skills demonstrated

Data exploration & cleaning · variable selection · statistical transformation (logit) · summary statistics · marginal distributions · categorical, continuous, and grouped relationship analysis · visualization with seaborn (count plots, boxplots, regression `lmplot`s, point plots) · interpreting weak/noisy relationships.

## Files

- [`spotify_popularity_eda.ipynb`](spotify_popularity_eda.ipynb) — the full analysis (renders directly on GitHub).
- `spotify_popularity_eda.html` — a styled report version for easy reading.
