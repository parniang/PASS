
This project demonstrates the application of various dataset reduction techniques (PAA, MinMax, ASAP, M4, RS, SS, VW, PASS) on the ETTh2 dataset, evaluates their performance based on multiple metrics, and visualizes the results.

Comparison of reduced datasets with the original using quantitative metrics such as:
<br /> Mean Squared Error (MSE)
<br /> Structural Similarity Index (SSIM)
<br /> DSSIM (1 - SSIM)
<br /> Peak Signal-to-Noise Ratio (PSNR)
<br /> Approximation Percentage Score (APScore)
<br /> Running Time
<br /> Sampled Data Points

Visualization of both the original and reduced datasets for intuitive understanding:
<br /> Original Dataset Plot: Complete time-series data.
<br /> Reduced Dataset Plots: Overlaid comparison of reduced vs. original data.

The PASS algorithm was implemented to reduce the dataset by selecting key points based on a threshold (θ) that determines significant transitions in the data. Several thresholds were tested to determine the optimal value. Threshold values of 5, 0.5, 0.1, and 0.01 were evaluated, and their performance was measured using mentioned metrics. Higher thresholds (e.g., 5) resulted in overly simplified datasets, losing significant detail. A threshold of 0.01 preserved crucial transitions and minimized error metrics, providing the best balance of accuracy and reduction, providing the most accurate representation of the ETTh2 dataset when using the PASS algorithm.

Key Steps in the PASS Algorithm:
<br /> 1-Calculate the angle between data points.  
2-Select points if the angle exceeds the threshold.  
3-Output the reduced dataset.



