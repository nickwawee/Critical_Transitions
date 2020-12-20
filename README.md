# Critical Transitions
This repo will contain select material regarding the analysis of the developmental trajectory of liver cells. It includes dimensionality reduction, implementation of a custom time series model, and visualizations. Large files were removed from the repo. The report document explains the entire project.

## Future Work
Listed below are improvements that could be done to the algorithm workflow.

- Create two separate linear grids for the pre and post branch expression values so that the expression values are identitical prior to the branch point
- Instead of manually fitting an AR model to the data, automatically fit an AR model based on the successful pass of the KPSS or ADF test-- this will allow for the algorithm to scale to several features without the visual inspection limitation
- Implement a two-sample t test (or other method) for step detection of autocorrelation (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2134886/)
- Make the time series algorithm part parallelizable if it takes too long, this can help with large grid sizes
- Create classification metrics based on the step detection results and the results from Monocle's BEAM (FDR <= 0.05) results as a baseline
