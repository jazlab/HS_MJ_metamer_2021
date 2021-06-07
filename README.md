# HS_MJ_metamer_2021
Data from Sohn &amp; Jazayeri, (2021) in Matlab MAT format

data_RSG is a cell array whose element corresponds to each subject. In each cell/subject, there are 5 sessions (some subjects only completed a subset of 5 sessions).
Each session is a structure whose fields contain the following ([] denotes size of data matrix).
- ts: sample time interval (ts) [number of trials x 1]
- tp: production time interval (tp) [number of trials x 1]
- deltaT: offset for metamer cost function [number of trials x 1]. This can be used to identify trials' condition. If 0, trials are for original prior-cost condition.
- reward: reward score subjects received [number of trials x 1].
- wm: weber fraction parameter for measurement [1 (1st session) or 2 (later sessions) x 1]. Fit for ideal-observer Bayesian-least-square model.
- wp: weber fraction parameter for production [1 (1st session) or 2 (later sessions) x 1]. Fit for ideal-observer Bayesian-least-square model.
- offset: offset parameter for ideal-observer Bayesian-least-square model [1 (1st session) or 2 (later sessions) x 1].
- sessDate: session data (YYYYMMDD) [1 x 1].
- GMM: Gaussian mixture model object for metamer prior [1 x 1].
- k: scaling factor for metamer cost function to match expected reward [1 x 1].
- pOptimal: p(optimal) for sessions with transitions [number of trials x 1].
- pPriorSensitive: p(prior-sensitive) for sessions with transitions [number of post-transition trials x 1].
- pCostSensitive: p(cost-sensitive) for sessions with transitions [number of post-transition trials x 1].
    <subjective prior and cost function>
- subjMu: inferred subjective prior mean [5 blocks of ~100 trials x 1].
- subjDeltaT: inferred subjective prior mean [5 blocks of ~100 trials x 1].
- subjSigma: inferred subjective prior SD [5 blocks of ~100 trials x 1].
- subjWm: inferred subjective weber fraction for measurement [5 blocks of ~100 trials x 1].
- subjWp: inferred subjective weber fraction for production [5 blocks of ~100 trials x 1].
    <learning time constant>
- tauMu: learning time constant for prior mean [1 x 1]
- tauDeltaT:  learning time constant for cost offset [1 x 1]
- tauSigma:  learning time constant for prior SD [1 x 1]
 
data_VMR is a cell array whose element corresponds to each subject. In each cell/subject, there are 5 sessions (some subjects only completed a subset of 5 sessions).
Each session is a structure whose fields contain the following ([] denotes size of data matrix).
- xs: sample rotation angle [number of trials x 1]
- xp: response counter-rotation angle [number of trials x 1]
- deltaX: offset for metamer cost function [number of trials x 1]. This can be used to identify trials' condition. If 0, trials are for original prior-cost condition.
- reward: reward score subjects received [number of trials x 1].
- sigmaM: noise parameter for measurement [1 (1st session) or 2 (later sessions) x 1]. Fit for ideal-observer Bayesian-least-square model.
- sigmaP: noise parameter for production [1 (1st session) or 2 (later sessions) x 1]. Fit for ideal-observer Bayesian-least-square model.
- offset: offset parameter for ideal-observer Bayesian-least-square model [1 (1st session) or 2 (later sessions) x 1].
- sessDate: session data (YYYYMMDD) [1 x 1].
- k: scaling factor for metamer cost function to match expected reward [1 x 1].
- pOptimal: p(optimal) for sessions with transitions [number of trials x 1].
- pPriorSensitive: p(prior-sensitive) for sessions with transitions [number of post-transition trials x 1].
- pCostSensitive: p(cost-sensitive) for sessions with transitions [number of post-transition trials x 1].
