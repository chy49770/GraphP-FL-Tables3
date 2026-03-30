**Table 1: Fisher Overhead Analysis**
| Method | GPU Memory Usage | Time per Round |
| :--- | :--- | :--- |
| FedAvg + VIB + MSFF + SSL | 41.52MB | 22.32s |
| **GraphP-FL (Ours)** | **42.87MB** | **23.50s** |

<br>

**Table 2: Model Performance**
| Model | DAPP | COLLAB | NCI1 |
| :--- | :--- | :--- | :--- |
| Ours + GCN | $91.62 \pm 0.65$ | $81.98 \pm 0.72$ | $91.88 \pm 0.58$ |
| Ours + GAT | $87.42 \pm 0.88$ | $84.49 \pm 0.91$ | $87.48 \pm 0.76$ |
| Ours + GraphSAGE | $92.54 \pm 0.71$ | $81.51 \pm 0.68$ | $88.80 \pm 0.82$ |
| Ours + Graph Transformer | $94.42 \pm 0.54$ | $81.98 \pm 0.82$ | $88.12 \pm 0.63$ |
| **Ours** | **$96.81 \pm 0.21$** | **$87.56 \pm 0.35$** | **$92.55 \pm 0.42$** |

<br>

**Table 3: Model Overhead**
| Model | DAPP (GPU Memory / Time) | COLLAB (GPU Memory / Time) | NCI1 (GPU Memory / Time) |
| :--- | :--- | :--- | :--- |
| Ours + GCN | 35.73MB / 28.30s | 350.08MB / 7.73s | 37.82MB / 3.84s |
| Ours + GAT | 41.98MB / 29.53s | 1235.52MB / 12.06s | 51.87MB / 4.11s |
| Ours + GraphSAGE | 38.08MB / 27.02s | 201.35MB / 5.19s | 40.16MB / 3.71s |
| Ours + Graph Transformer | 115.12MB / 27.41s | 807.47MB / 39.67s | 26.26MB / 7.96s |
| **Ours** | **42.87MB / 23.50s** | **216.63MB / 6.92s** | **47.43MB / 4.90s** |

<br>

**Table 4: Performance Analysis**
| Method | DD | DD_noisy | MUTAG | MUTAG_noisy |
| :--- | :--- | :--- | :--- | :--- |
| FedAvg | $81.41 \pm 2.45$ | $72.93 \pm 3.86$ | $83.51 \pm 4.12$ | $60.83 \pm 3.61$ |
| FedAGHN | $83.68 \pm 1.15$ | $76.41 \pm 2.58$ | $80.12 \pm 3.25$ | $65.45 \pm 3.12$ |
| **Ours** | **$74.66 \pm 1.85$** | **$79.32 \pm 1.65$** | **$80.00 \pm 3.05$** | **$84.83 \pm 2.98$** |

<br>

**Table 5: Hyperparameter Sensitivity Analysis**
| Setting | DD | MUTAG |
| :--- | :--- | :--- |
| $\lambda_1 = 0.01$ | $76.43 \pm 1.62$ | $82.83 \pm 2.85$ |
| $\lambda_1 = 0.1$ | $74.66 \pm 1.85$ | $80.00 \pm 3.05$ |
| $\lambda_1 = 0.5$ | $71.32 \pm 2.24$ | $78.03 \pm 3.18$ |
