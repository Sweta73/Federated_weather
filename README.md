# FedTail-CP: Federated Conformal Prediction for Calibrated Rainfall Forecasting

FedTail-CP is a federated conformal prediction framework designed to improve the reliability and calibration of upper prediction bounds in one-day-ahead rainfall forecasting. Using NASA POWER daily rainfall data across India from 2000 to 2024, this project investigates 90th-percentile coverage calibration at both global and rainfall-regime levels.

The proposed approach combines risk-bin-based calibration with shrinkage-based threshold adjustment using compact score sketches shared across the federated server. It aims to address the challenges of heterogeneous rainfall patterns and limited historical calibration data across distributed weather stations while preserving the federated learning setting.

**Key Contributions:**
- Federated calibration of 90th-percentile rainfall prediction intervals.
- Risk-bin-based calibration to address heterogeneous rainfall regimes.
- Shrinkage-based threshold adjustment using compact calibration score sketches.
- Theoretical high-probability coverage bounds and MSE-optimal shrinkage weighting.
- Evaluation against uncalibrated, station-only, and pooled calibration approaches.

**Key Results:**
- Achieved a mean absolute deviation of **0.020 ± 0.001** from the target 90% coverage in the top risk bin across five training seeds.
- Improved worst-station top-bin coverage from **0.804 to 0.853**.
- Demonstrated statistically significant improvements over station-only and pooled calibration.
- Identified limitations under short calibration windows (30 days) and outcome-defined extreme rainfall events.

This project explores more reliable uncertainty quantification in federated rainfall forecasting, with potential applications in flood risk assessment, water resource management, and irrigation planning.

**Dataset:** NASA POWER Daily Rainfall Data (India, 2000–2024)

**Method:** Federated Learning | Conformal Prediction | Quantile Regression | Coverage Calibration
