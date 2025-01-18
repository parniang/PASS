Analysis of ETTh2 Dataset with PASS Algorithm
This document explains the steps followed to analyze the ETTh2 dataset using the PASS algorithm. Additionally, it highlights the process of testing various thresholds and concludes that a threshold of 0.01 provides the best results for this dataset. 
The PASS algorithm was implemented to reduce the dataset by selecting key points based on a threshold (θ) that determines significant transitions in the data.
The analysis determined that a threshold of 0.01 provides the most accurate representation of the ETTh2 dataset when using the PASS algorithm. The notebook includes visualizations and detailed metrics to support this conclusion, making it easy to share and reproduce results.

Key Steps in the Algorithm:
Calculate the angle between data points.
Select points if the angle exceeds the threshold.
Output the reduced dataset.

Testing Different Thresholds:
Several thresholds were tested to determine the optimal value. Threshold values of 5, 0.5, 0.1, and 0.01 were evaluated, and their performance was measured using metrics such as:
Mean Squared Error (MSE)
Structural Similarity Index (SSIM)
DSSIM (1 - SSIM)
Peak Signal-to-Noise Ratio (PSNR)
Approximation Percentage Score (APScore)
Running Time
Sampled Data Points

Observations:
Higher thresholds (e.g., 5) resulted in overly simplified datasets, losing significant detail.
A threshold of 0.01 preserved crucial transitions and minimized error metrics, providing the best balance of accuracy and reduction.

Threshold 0.01 provided the best results with a high SSIM and low MSE while maintaining a reasonable number of sampled points.

Visualization
Two types of visualizations were included:

Original Dataset:
A plot showing the raw ETTh2 data.

Reduced Dataset (PASS):
A comparison of the original dataset (blue) and the reduced dataset (red).
