# Introduction:
A comparative analysis of asset pricing and stock return forecasting by evaluating the performance of traditional finance models against modern machine learning architectures and assess their results.
The repository includes code files for data acquiring, data preparation, model constructing and performance results.
# Models:
1. Traditional Models: CAPM and Fama-French Three Factors.
2. Machine Learning Models: Random Forest and Neural Network.
# Objectives:
1. Benchmarking: Compare the R-square and Mean Squared Error (MSE) across all four models.
2. Feature Importance: Analyze which financial ratios and macroeconomic indicators drive predictability in ML models versus traditional factors.
3. Risk-Adjusted Performance: Assess whether ML-driven predictions can generate superior Sharpe ratios in a backtested portfolio.
# Data:
1. Historical stock prices and other finanical metrics: acquire data from 1985 Vietnamese firms using the Vnstock library.
2. Market returns: use VNI Index historical returns as the benchmark.
3. Risk-free rate: use VN 10-Year Bond Yield historical data.
# Summary of results:
More complex models do not necessarily yield better point-in-time predictions. In fact, the Neural Network underperformed significantly compared to simpler benchmarks.
- Random Forest: achieved a cumulative return of ~20% and the highest Sharpe Ratio (1.7). The success comes from its ability to rank sectors correctly, even if the specific return numbers are slightly off.
- Neural Network: despite having the worst predictive accuracy, it managed a positive return of 8% and a Sharpe Ratio of 0.6. However, the model's performance was highly volatile with significant drawdowns.
- CAPM & FF3: both failed as investment tools, generating cumulative losses of 25–30%. They systematically misranked sectors, leading to poor long-short decisions. Thus, these models are better to be used as foundational frameworks for valuing assets, calculating expected returns, and managing portfolio risk.
