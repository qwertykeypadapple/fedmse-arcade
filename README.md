# FedMSE Arcade

Eight short browser games that explain the research paper
[FedMSE: Semi-supervised federated learning approach for IoT network intrusion detection](https://www.jaist.ac.jp/~razvan/publications/fedmse_iot_network_intrusion_detection.pdf)
(Nguyen & Beuran, *Computers & Security*, 2025) to high-school and early-college students.

| # | Game | Idea it teaches |
|---|---|---|
| 1 | The Copy Machine | What an autoencoder does: squeeze, rebuild, and flag big copy errors |
| 2 | Spot the Intruder | Shrink autoencoder + centroid: far from normal means suspicious |
| 3 | Fair or Lopsided? | Non-IID data across gateways (Dirichlet split) |
| 4 | Who Should We Trust? | MSEAvg (trust = 1 ÷ mistakes) versus FedAvg (trust = data size) |
| 5 | Teamwork Round | The steps of one federated learning round, then detection |
| 6 | What Leaves the Building? | What stays private and what is shared |
| 7 | Word Hunt | Key vocabulary |
| 8 | Myth or Fact? | The paper's results and limitations |

## Play

Play online: https://qwertykeypadapple.github.io/fedmse-arcade/

Or open `index.html` in any modern browser. It is a single self-contained file with no build step.

`fedmse_arcade.html` is the source (the same page without the `<!doctype html>` wrapper). After editing it, rebuild `index.html` with:

```bash
{ printf '<!doctype html>\n<html lang="en">\n'; cat fedmse_arcade.html; printf '\n</html>\n'; } > index.html
```

Some visuals (the dartboard in game 4, the 8-bar messages in game 1) are simplified teaching models, not the paper's real model. The page says where.
