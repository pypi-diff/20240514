# Comparing `tmp/peak_performance-0.6.4-py3-none-any.whl.zip` & `tmp/peak_performance-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 42503 bytes, number of entries: 13
--rw-r--r--  2.0 unx      261 b- defN 23-Dec-04 12:45 peak_performance/__init__.py
--rw-r--r--  2.0 unx    25130 b- defN 23-Dec-04 12:45 peak_performance/models.py
--rw-r--r--  2.0 unx    64311 b- defN 23-Dec-04 12:45 peak_performance/pipeline.py
--rw-r--r--  2.0 unx     9280 b- defN 23-Dec-04 12:45 peak_performance/plots.py
--rw-r--r--  2.0 unx       97 b- defN 23-Dec-04 12:45 peak_performance/test_main.py
--rw-r--r--  2.0 unx     9334 b- defN 23-Dec-04 12:45 peak_performance/test_models.py
--rw-r--r--  2.0 unx    22652 b- defN 23-Dec-04 12:45 peak_performance/test_pipeline.py
--rw-r--r--  2.0 unx     4100 b- defN 23-Dec-04 12:45 peak_performance/test_plots.py
--rw-r--r--  2.0 unx    32387 b- defN 23-Dec-04 12:45 peak_performance-0.6.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4796 b- defN 23-Dec-04 12:45 peak_performance-0.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-04 12:45 peak_performance-0.6.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Dec-04 12:45 peak_performance-0.6.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1121 b- defN 23-Dec-04 12:45 peak_performance-0.6.4.dist-info/RECORD
-13 files, 173578 bytes uncompressed, 40619 bytes compressed:  76.6%
+Zip file size: 43993 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      261 b- defN 24-May-14 07:39 peak_performance/__init__.py
+-rw-r--r--  2.0 unx    27457 b- defN 24-May-14 07:39 peak_performance/models.py
+-rw-r--r--  2.0 unx    64395 b- defN 24-May-14 07:39 peak_performance/pipeline.py
+-rw-r--r--  2.0 unx     9455 b- defN 24-May-14 07:39 peak_performance/plots.py
+-rw-r--r--  2.0 unx       97 b- defN 24-May-14 07:39 peak_performance/test_main.py
+-rw-r--r--  2.0 unx    11592 b- defN 24-May-14 07:39 peak_performance/test_models.py
+-rw-r--r--  2.0 unx    22961 b- defN 24-May-14 07:39 peak_performance/test_pipeline.py
+-rw-r--r--  2.0 unx     4100 b- defN 24-May-14 07:39 peak_performance/test_plots.py
+-rw-r--r--  2.0 unx    32387 b- defN 24-May-14 07:39 peak_performance-0.7.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5076 b- defN 24-May-14 07:39 peak_performance-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 07:39 peak_performance-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-14 07:39 peak_performance-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1122 b- defN 24-May-14 07:39 peak_performance-0.7.0.dist-info/RECORD
+13 files, 179012 bytes uncompressed, 42109 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: peak_performance/test_pipeline.py
 Comment: 
 
 Filename: peak_performance/test_plots.py
 Comment: 
 
-Filename: peak_performance-0.6.4.dist-info/LICENSE.md
+Filename: peak_performance-0.7.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: peak_performance-0.6.4.dist-info/METADATA
+Filename: peak_performance-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: peak_performance-0.6.4.dist-info/WHEEL
+Filename: peak_performance-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: peak_performance-0.6.4.dist-info/top_level.txt
+Filename: peak_performance-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: peak_performance-0.6.4.dist-info/RECORD
+Filename: peak_performance-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## peak_performance/models.py

```diff
@@ -32,14 +32,34 @@
 
     Normal = "normal"
     SkewNormal = "skew_normal"
     DoubleNormal = "double_normal"
     DoubleSkewNormal = "double_skew_normal"
 
 
+def guess_noise(intensity):
+    """
+    Function for providing a guess for the noise width of a given signal
+    based on the first and last 15 % of data points in a time series.
+
+    Parameters
+    ----------
+    time
+        NumPy array with the time values of the relevant timeframe.
+    intensity
+        NumPy array with the intensity values of the relevant timeframe.
+    """
+    n = len(intensity)
+    ifrom = int(np.ceil(0.15 * n))
+    ito = int(np.floor(0.85 * n))
+    start_ints = intensity[:ifrom]
+    end_ints = intensity[ito:]
+    return np.std([*(start_ints - np.mean(start_ints)), *(end_ints - np.mean(end_ints))])
+
+
 def initial_guesses(time: np.ndarray, intensity: np.ndarray):
     """
     Provide initial guesses for priors.
 
     Parameters
     ----------
     time
@@ -75,20 +95,24 @@
     intensity_tuple.sort(key=lambda x: x[1])
     noise_range = int(np.round(0.35 * len(intensity_corrected), decimals=0))
     noise_tuple = intensity_tuple[:noise_range]
     noise_index = sorted([x[0] for x in noise_tuple])
     # use the indeces in noise_index to get the time and intensity of all noise data points
     noise_time = [time[n] for n in noise_index]
     noise_intensity = [intensity[n] for n in noise_index]
-    # calculate the width of the noise
-    noise_width_guess = max(noise_intensity) - min(noise_intensity)
 
     # use scipy to fit a linear regression through the noise as a prior for the eventual baseline
     baseline_fit = st.linregress(noise_time, noise_intensity)
 
+    # calculate the width of the noise
+    noise_width_guess = guess_noise(intensity)
+
+    # clip the noise to at least 10
+    noise_width_guess = np.clip(noise_width_guess, 10, np.inf)
+
     return baseline_fit.slope, baseline_fit.intercept, noise_width_guess
 
 
 def baseline_intercept_prior_params(intercept_guess: Union[float, int]) -> Mapping[str, float]:
     """
     Centralized function for supplying parameters for the baseline intercept prior.
 
@@ -114,17 +138,17 @@
     """
     return {
         "mu": slope_guess,
         "sigma": np.clip(abs(slope_guess / 5), 0.5, np.inf),
     }
 
 
-def normal_posterior(baseline, time: np.ndarray, mean, std, *, height):
+def normal_peak_shape(baseline, time: np.ndarray, mean, std, *, height):
     """
-    Model a peak shaped like the PDF of a normal distribution.
+    Model a peak shaped like a normal distribution.
 
     Parameters
     ----------
     baseline
         Baseline of the data.
     time
         NumPy array with the time values of the relevant timeframe.
@@ -162,76 +186,120 @@
     with pm.Model() as pmodel:
         # add observations to the pmodel as ConstantData
         pm.ConstantData("time", time)
         pm.ConstantData("intensity", intensity)
         # add guesses to the pmodel as ConstantData
         pm.ConstantData("intercept_guess", intercept_guess)
         pm.ConstantData("slope_guess", slope_guess)
-        pm.ConstantData("noise_width_guess", noise_width_guess)
+        noise_guess = pm.ConstantData("noise_width_guess", noise_width_guess)
 
         # priors plus error handling in case of mathematically impermissible values
         baseline_intercept = pm.Normal(
             "baseline_intercept", **baseline_intercept_prior_params(intercept_guess)
         )
         baseline_slope = pm.Normal("baseline_slope", **baseline_slope_prior_params(slope_guess))
         baseline = pm.Deterministic("baseline", baseline_intercept + baseline_slope * time)
-        noise = pm.LogNormal("noise", np.clip(np.log(noise_width_guess), np.log(10), np.inf), 1)
+        noise = pm.LogNormal("noise", pt.log(noise_guess))
         # define priors for parameters of a normally distributed posterior
         mean = pm.Normal("mean", np.mean(time[[0, -1]]), np.ptp(time) / 2)
         std = pm.HalfNormal("std", np.ptp(time) / 3)
         height = pm.HalfNormal("height", 0.95 * np.max(intensity))
         pm.Deterministic("area", height / (1 / (std * np.sqrt(2 * np.pi))))
         pm.Deterministic("sn", height / noise)
         # posterior
-        y = normal_posterior(baseline, time, mean, std, height=height)
+        y = normal_peak_shape(baseline, time, mean, std, height=height)
         y = pm.Deterministic("y", y)
 
         # likelihood
         pm.Normal("L", mu=y, sigma=noise, observed=intensity)
 
     return pmodel
 
 
 def double_model_mean_prior(time):
     """
-    Function creating prior probability distributions for double peaks using a ZeroSumNormal distribution.
+    Function creating prior probability distributions for the mean retention times of a dual-peak.
 
     Parameters
     ----------
     time
         NumPy array with the time values of the relevant timeframe.
 
     Returns
     -------
     mean
-        Normally distributed prior for the ordered means of the double peak model.
+        Normally distributed prior for the ordered means of the multi-peak model.
     diff
-        Difference between meanmean and mean.
+        Difference between the group mean and peak-wise mean.
+    meanmean
+        Normally distributed prior for the group mean of the peak means.
+    """
+    tmin = np.min(time)
+    tdelta = np.ptp(time)
+    meanmean = pm.Normal("meanmean", mu=tmin + tdelta / 2, sigma=tdelta / 6)
+    separation = pm.Gamma(
+        "separation",
+        mu=tdelta / 6,
+        sigma=tdelta / 12,
+    )
+    offset = pm.Deterministic("offset", pt.stack([-separation / 2, separation / 2]), dims="subpeak")
+    mean = pm.Deterministic(
+        "mean",
+        meanmean + offset,
+        dims=("subpeak",),
+    )
+    return mean, offset, meanmean
+
+
+def multi_peak_means_prior(time):
+    """
+    Function creating prior probability distributions for multi-peaks using a ZeroSumNormal distribution.
+
+    The number of peaks is determined from the `"subpeak"` model coordinates.
+
+    Parameters
+    ----------
+    time
+        NumPy array with the time values of the relevant timeframe.
+
+    Returns
+    -------
+    mean
+        Normally distributed prior for the ordered means of the multi-peak model.
+    offset
+        Time offset between the group mean and peak-wise mean.
     meanmean
-        Normally distributed prior for the mean of the double peak means.
+        Normally distributed prior for the group mean of the peak means.
     """
+    pmodel = pm.modelcontext(None)
     meanmean = pm.Normal("meanmean", mu=np.min(time) + np.ptp(time) / 2, sigma=np.ptp(time) / 6)
-    diff = pm.ZeroSumNormal(
-        "diff",
-        sigma=1,
-        shape=(2,),  # currently no dims due to bug with ordered transformation
+    offset_unsorted = pm.ZeroSumNormal(
+        "offset_unsorted",
+        sigma=2,
+        # Support arbitrary number of subpeaks
+        shape=len(pmodel.coords["subpeak"]),
+        # NOTE: As of PyMC v5.14, the OrderedTransform and ZeroSumTransform are incompatible.
+        # See https://github.com/pymc-devs/pymc/issues/6975.
+        # As a workaround we'll call pt.sort a few lines below.
     )
-    mean = pm.Normal(
+    offset = pm.Deterministic("offset", pt.sort(offset_unsorted), dims="subpeak")
+    mean = pm.Deterministic(
         "mean",
-        mu=meanmean + diff,
-        sigma=1,
-        transform=pm.distributions.transforms.ordered,
+        meanmean + offset,
+        # Introduce a small jitter to the subpeak means to decouple them
+        # from the strictly asymmetric ZeroSumNormal entries.
+        # This reduces the chances of unwanted bimodality.
         dims=("subpeak",),
     )
-    return mean, diff, meanmean
+    return mean, offset, meanmean
 
 
-def double_normal_posterior(baseline, time: np.ndarray, mean, std, *, height):
+def double_normal_peak_shape(baseline, time: np.ndarray, mean, std, *, height):
     """
-    Define a univariate ordered normal distribution as the posterior.
+    Model a peak shaped like a univariate ordered normal distribution.
 
     Parameters
     ----------
     baseline
         Baseline of the data.
     time
         NumPy array with the time values of the relevant timeframe.
@@ -277,36 +345,37 @@
     with pm.Model(coords=coords) as pmodel:
         # add observations to the pmodel as ConstantData
         pm.ConstantData("time", time)
         pm.ConstantData("intensity", intensity)
         # add guesses to the pmodel as ConstantData
         pm.ConstantData("intercept_guess", intercept_guess)
         pm.ConstantData("slope_guess", slope_guess)
-        pm.ConstantData("noise_width_guess", noise_width_guess)
+        noise_guess = pm.ConstantData("noise_width_guess", noise_width_guess)
 
         # priors
         baseline_intercept = pm.Normal(
             "baseline_intercept", **baseline_intercept_prior_params(intercept_guess)
         )
         baseline_slope = pm.Normal("baseline_slope", **baseline_slope_prior_params(slope_guess))
         baseline = pm.Deterministic("baseline", baseline_intercept + baseline_slope * time)
-        noise = pm.LogNormal("noise", np.clip(np.log(noise_width_guess), np.log(10), np.inf), 1)
-        std = pm.HalfNormal("std", sigma=[np.ptp(time) / 3, np.ptp(time) / 3], dims=("subpeak",))
+        noise = pm.LogNormal("noise", pt.log(noise_guess))
+        # NOTE: We expect dobule-peaks to be narrower w.r.t. the time frame, compare to single peaks.
+        std = pm.HalfNormal("std", sigma=[np.ptp(time) / 6, np.ptp(time) / 6], dims=("subpeak",))
         height = pm.HalfNormal(
             "height", sigma=[0.95 * np.max(intensity), 0.95 * np.max(intensity)], dims=("subpeak",)
         )
         pm.Deterministic("area", height / (1 / (std * np.sqrt(2 * np.pi))), dims=("subpeak",))
         pm.Deterministic("sn", height / noise, dims=("subpeak",))
         # use univariate ordered normal distribution for the mean values
         # use a zero sum normal distribution to describe the distance of the mean values
         # from the mean of the mean values ("meanmean")
         mean, diff, meanmean = double_model_mean_prior(time)
 
         # posterior
-        y = double_normal_posterior(baseline, time, mean, std, height=height)
+        y = double_normal_peak_shape(baseline, time, mean, std, height=height)
         y = pm.Deterministic("y", y)
 
         # likelihood
         pm.Normal("L", mu=y, sigma=noise, observed=intensity)
 
     return pmodel
 
@@ -426,17 +495,17 @@
     return area * (
         2
         * (1 / (scale * np.sqrt(2 * np.pi)) * pt.exp(-0.5 * ((mode_skew - loc) / scale) ** 2))
         * (0.5 * (1 + pt.erf(((alpha * (mode_skew - loc) / scale)) / np.sqrt(2))))
     )
 
 
-def skew_normal_posterior(baseline, time, mean, std, alpha, *, area):
+def skew_normal_peak_shape(baseline, time, mean, std, alpha, *, area):
     """
-    Define a skew normally distributed posterior.
+    Model a peak shaped like a skew normal distribution.
 
     Parameters
     ----------
     baseline
         Baseline of the data.
     time
         NumPy array with the time values of the relevant timeframe.
@@ -485,23 +554,23 @@
     with pm.Model() as pmodel:
         # add observations to the pmodel as ConstantData
         pm.ConstantData("time", time)
         pm.ConstantData("intensity", intensity)
         # add guesses to the pmodel as ConstantData
         pm.ConstantData("intercept_guess", intercept_guess)
         pm.ConstantData("slope_guess", slope_guess)
-        pm.ConstantData("noise_width_guess", noise_width_guess)
+        noise_guess = pm.ConstantData("noise_width_guess", noise_width_guess)
 
         # priors plus error handling in case of mathematically impermissible values
         baseline_intercept = pm.Normal(
             "baseline_intercept", **baseline_intercept_prior_params(intercept_guess)
         )
         baseline_slope = pm.Normal("baseline_slope", **baseline_slope_prior_params(slope_guess))
         baseline = pm.Deterministic("baseline", baseline_intercept + baseline_slope * time)
-        noise = pm.LogNormal("noise", np.clip(np.log(noise_width_guess), np.log(10), np.inf), 1)
+        noise = pm.LogNormal("noise", pt.log(noise_guess))
         mean = pm.Normal("mean", np.mean(time[[0, -1]]), np.ptp(time) / 2)
         std = pm.HalfNormal("std", np.ptp(time) / 3)
         alpha = pm.Normal("alpha", 0, 3.5)
         area = pm.HalfNormal("area", np.max(intensity) * 0.9)
 
         # calculate standard deviation and arithmetic mean of a skew normal distribution
         std_skew_formula = std_skew_calculation(std, alpha)
@@ -524,26 +593,26 @@
         # then calculate the height based on the mode
         height_formula = height_calculation(area, mean, std, alpha, mode_skew)
         height = pm.Deterministic(
             "height",
             height_formula,
         )
         pm.Deterministic("sn", height / noise)
-        y = skew_normal_posterior(baseline, time, mean, std, alpha, area=area)
+        y = skew_normal_peak_shape(baseline, time, mean, std, alpha, area=area)
         y = pm.Deterministic("y", y)
 
         # likelihood
         pm.Normal("L", mu=y, sigma=noise, observed=intensity)
 
     return pmodel
 
 
-def double_skew_normal_posterior(baseline, time: np.ndarray, mean, std, alpha, *, area):
+def double_skew_normal_peak_shape(baseline, time: np.ndarray, mean, std, alpha, *, area):
     """
-    Define a univariate ordered skew normal distribution as the posterior.
+    Model a peak shaped like the a univariate ordered skew normal distribution.
 
     Parameters
     ----------
     baseline
         Baseline of the data.
     time
         NumPy array with the time values of the relevant timeframe.
@@ -601,23 +670,23 @@
     with pm.Model(coords=coords) as pmodel:
         # add observations to the pmodel as ConstantData
         pm.ConstantData("time", time)
         pm.ConstantData("intensity", intensity)
         # add guesses to the pmodel as ConstantData
         pm.ConstantData("intercept_guess", intercept_guess)
         pm.ConstantData("slope_guess", slope_guess)
-        pm.ConstantData("noise_width_guess", noise_width_guess)
+        noise_guess = pm.ConstantData("noise_width_guess", noise_width_guess)
 
         # priors plus error handling in case of mathematically impermissible values
         baseline_intercept = pm.Normal(
             "baseline_intercept", **baseline_intercept_prior_params(intercept_guess)
         )
         baseline_slope = pm.Normal("baseline_slope", **baseline_slope_prior_params(slope_guess))
         baseline = pm.Deterministic("baseline", baseline_intercept + baseline_slope * time)
-        noise = pm.LogNormal("noise", np.clip(np.log(noise_width_guess), np.log(10), np.inf), 1)
+        noise = pm.LogNormal("noise", pt.log(noise_guess))
         # use univariate ordered normal distribution for the mean values
         # use a zero sum normal distribution to describe the distance of the mean values
         # from the mean of the mean values ("meanmean")
         mean, diff, meanmean = double_model_mean_prior(time)
         std = pm.HalfNormal(
             "std",
             sigma=[np.ptp(time) / 3, np.ptp(time) / 3],
@@ -652,15 +721,15 @@
         height = pm.Deterministic(
             "height",
             height_formula,
         )
         pm.Deterministic("sn", height / noise, dims=("subpeak",))
 
         # posterior
-        y = double_skew_normal_posterior(baseline, time, mean, std, alpha, area=area)
+        y = double_skew_normal_peak_shape(baseline, time, mean, std, alpha, area=area)
         y = pm.Deterministic("y", y)
 
         # likelihood
         pm.Normal("L", mu=y, sigma=noise, observed=intensity)
 
     return pmodel
```

## peak_performance/pipeline.py

```diff
@@ -485,14 +485,15 @@
         Number of samples after tuning (default = 2000).
 
     Returns
     -------
     idata
         Inference data object.
     """
+    sample_kwargs.setdefault("chains", 4)
     sample_kwargs.setdefault("tune", 2000)
     sample_kwargs.setdefault("draws", 2000)
     # check if nutpie is available; if so, use it to enhance performance
     if importlib.util.find_spec("nutpie"):
         nuts_sampler = "nutpie"
     else:
         nuts_sampler = "pymc"
@@ -643,15 +644,15 @@
 
     Returns
     -------
     idata
         Inference data object updated with the posterior predictive samples.
     """
     with pmodel:
-        idata.extend(pm.sample_posterior_predictive(idata, var_names=["y"]))
+        idata.extend(pm.sample_posterior_predictive(idata))
     return idata
 
 
 def report_save_idata(idata, ui: UserInput, filename: str):
     """
     Saves inference data object as a .nc file.
 
@@ -1405,15 +1406,15 @@
     for r in dataframe_to_rows(signals, index=False, header=False):
         wb_signals.append(r)
     wb.save(Path(path_raw_data) / "Template.xlsx")
     return
 
 
 def model_selection_check(
-    result_df: pandas.DataFrame, ic: str, elpd_threshold: Union[str, float] = 25
+    result_df: pandas.DataFrame, ic: str, elpd_threshold: Union[str, float] = 35
 ) -> str:
     """
     During model seleciton, double peak models are sometimes incorrectly preferred due to their increased complexity.
     Therefore, they have to outperform single peak models by an empirically determined value of the elpd.
 
     Parameters
     ----------
@@ -1431,18 +1432,19 @@
     ----------
     selected_model
         Name of the selected model type.
     """
     selected_model = str(result_df.index[0])
     if "double" in selected_model:
         df_single_peak_models = result_df[~result_df.index.str.contains("double")]
-        elpd_single = max(list(df_single_peak_models[f"elpd_{ic}"]))
-        elpd_double = max(list(result_df[f"elpd_{ic}"]))
-        if not elpd_double > elpd_single + elpd_threshold:
-            selected_model = str(df_single_peak_models.index[0])
+        if len(df_single_peak_models) > 0:
+            elpd_single = max(list(df_single_peak_models[f"elpd_{ic}"]))
+            elpd_double = max(list(result_df[f"elpd_{ic}"]))
+            if not elpd_double > elpd_single + elpd_threshold:
+                selected_model = str(df_single_peak_models.index[0])
     return selected_model
 
 
 def selection_loop(
     path_raw_data: Union[str, os.PathLike],
     *,
     files_for_selection: Mapping[str, str],
```

## peak_performance/plots.py

```diff
@@ -14,28 +14,28 @@
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import os
 from pathlib import Path
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
 import arviz as az
 import numpy as np
 import pandas
 import pymc as pm
 from matplotlib import pyplot as plt
 
 
 def plot_raw_data(
     identifier: str,
     time: np.ndarray,
     intensity: np.ndarray,
-    path: Union[str, os.PathLike],
+    path: Optional[Union[str, os.PathLike]],
     save_formats: Sequence[str] = ("png", "svg"),
 ):
     """
     Plot just the raw data in case no peak was found.
 
     Parameters
     ----------
@@ -58,27 +58,27 @@
     ax.scatter(time, intensity, marker="x", color="black", label="data")
     plt.legend()
     ax.set_xlabel("time / min", fontsize=12, fontweight="bold")
     ax.set_ylabel("intensity / a.u.", fontsize=12, fontweight="bold")
     plt.xticks(size=11.5)
     plt.yticks(size=11.5)
     fig.tight_layout()
-    for format in save_formats:
-        fig.savefig(Path(path) / f"{identifier}_NoPeak.{format}", format=format)
-    plt.close(fig)
+    if path is not None:
+        for format in save_formats:
+            fig.savefig(Path(path) / f"{identifier}_NoPeak.{format}", format=format)
+        plt.close(fig)
 
     return
 
 
 def plot_density(
     *, ax, x: np.ndarray, samples, percentiles=(5, 95), percentile_kwargs=None, **kwargs
 ):
     """
     Method to plot the original data points alongside the posterior predictive plot (percentiles marked with a black, dashed line).
-    Serves as a more accurate comparison between data and model than comparing data and posterior distribution.
 
     Parameters
     ----------
     ax
         Axes of a matplotlib figure.
     x
         Values of the x dimension of the plot (here: time).
@@ -131,15 +131,15 @@
     return
 
 
 def plot_posterior_predictive(
     identifier: str,
     time: np.ndarray,
     intensity: np.ndarray,
-    path: Union[str, os.PathLike],
+    path: Optional[Union[str, os.PathLike]],
     idata: az.InferenceData,
     discarded: bool,
     save_formats: Sequence[str] = ("png", "svg"),
 ):
     """
     Save plot of posterior_predictive with 95 % HDI and original data points.
 
@@ -164,44 +164,47 @@
     time = np.array(time)
     intensity = np.array(intensity)
     fig, ax = plt.subplots()
     # plot the posterior predictive
     plot_density(
         ax=ax,
         x=time,
-        samples=idata.posterior_predictive.y.stack(sample=("chain", "draw")).T.values,
+        samples=idata.posterior_predictive["L"].stack(sample=("chain", "draw")).T.values,
         percentiles=(2.5, 97.5),
     )
     # plot the raw data points
     ax.scatter(time, intensity, marker="x", color="black", label="data")
     ax.set_xlabel("time / min", fontsize=11.5, fontweight="bold")
     ax.set_ylabel("intensity / a.u.", fontsize=11.5, fontweight="bold")
     plt.xticks(size=11.5)
     plt.yticks(size=11.5)
     plt.legend()
     fig.tight_layout()
-    # if signal was discarded, add a "_NoPeak" to the file name
-    if discarded:
-        for format in save_formats:
-            fig.savefig(
-                Path(path) / f"{identifier}_predictive_posterior_NoPeak.{format}", format=format
-            )
-    else:
-        for format in save_formats:
-            fig.savefig(Path(path) / f"{identifier}_predictive_posterior.{format}", format=format)
-    plt.close(fig)
+    if path is not None:
+        # if signal was discarded, add a "_NoPeak" to the file name
+        if discarded:
+            for format in save_formats:
+                fig.savefig(
+                    Path(path) / f"{identifier}_predictive_posterior_NoPeak.{format}", format=format
+                )
+        else:
+            for format in save_formats:
+                fig.savefig(
+                    Path(path) / f"{identifier}_predictive_posterior.{format}", format=format
+                )
+        plt.close(fig)
 
     return
 
 
 def plot_posterior(
     identifier: str,
     time: np.ndarray,
     intensity: np.ndarray,
-    path: Union[str, os.PathLike],
+    path: Optional[Union[str, os.PathLike]],
     idata: az.InferenceData,
     discarded: bool,
     save_formats: Sequence[str] = ("png", "svg"),
 ):
     """
     Saves plot of posterior, estimated baseline, and original data points.
 
@@ -242,30 +245,31 @@
     plt.plot(x, y)
     plt.legend()
     ax.set_xlabel("time / min", fontsize=12, fontweight="bold")
     ax.set_ylabel("intensity / a.u.", fontsize=12, fontweight="bold")
     plt.xticks(size=11.5)
     plt.yticks(size=11.5)
     fig.tight_layout()
-    # if signal was discarded, add a "_NoPeak" to the file name
-    if discarded:
-        for format in save_formats:
-            fig.savefig(Path(path) / f"{identifier}_posterior_NoPeak.{format}", format=format)
-    else:
-        for format in save_formats:
-            fig.savefig(Path(path) / f"{identifier}_posterior.{format}", format=format)
-    plt.close(fig)
+    if path is not None:
+        # if signal was discarded, add a "_NoPeak" to the file name
+        if discarded:
+            for format in save_formats:
+                fig.savefig(Path(path) / f"{identifier}_posterior_NoPeak.{format}", format=format)
+        else:
+            for format in save_formats:
+                fig.savefig(Path(path) / f"{identifier}_posterior.{format}", format=format)
+        plt.close(fig)
 
     return
 
 
 def plot_model_comparison(
     df_comp: pandas.DataFrame,
     identifier: str,
-    path: Union[str, os.PathLike],
+    path: Optional[Union[str, os.PathLike]],
     save_formats: Sequence[str] = ("png", "svg"),
 ):
     """
     Function to plot the results of a model comparison.
 
     Parameters
     ----------
@@ -278,12 +282,13 @@
     save_formats
         Which file formats to save as.
         Must be supported by `plt.savefig()`, e.g. ``("png", "svg", "pdf")``.
     """
     axes = az.plot_compare(df_comp, insample_dev=False)
     fig = axes.figure
     plt.tight_layout()
-    for format in save_formats:
-        fig.savefig(Path(path) / f"model_comparison_{identifier}.{format}", format=format)
-    plt.close(fig)
+    if path is not None:
+        for format in save_formats:
+            fig.savefig(Path(path) / f"model_comparison_{identifier}.{format}", format=format)
+        plt.close(fig)
 
     return
```

## peak_performance/test_models.py

```diff
@@ -1,52 +1,128 @@
 from pathlib import Path
 
 import arviz as az
 import numpy as np
 import pymc as pm
+import pytensor.tensor as pt
 import pytest
 import scipy.integrate
 import scipy.stats as st
 
 from peak_performance import models
 
+_DP_ROOT = Path(__file__).absolute().parent.parent
+_REQUIRED_VARIABLES = {
+    "baseline_slope",
+    "baseline_intercept",
+    "baseline",
+    "std",
+    "height",
+    "area",
+    "sn",
+    "mean",
+    "y",
+    "noise",
+}
+_REQUIRED_DATA = {
+    "slope_guess",
+    "intercept_guess",
+    "noise_width_guess",
+}
+
+
+def test_noise_guessing():
+    expected = 0.7
+    intensities = [
+        *np.random.normal(10, expected, size=200),
+        *np.random.normal(0, 6, size=600),
+        *np.random.normal(40, expected, size=200),
+    ]
+    actual = models.guess_noise(intensities)
+    assert 0.6 < actual < 0.8
+    pass
+
 
 def test_initial_guesses():
     # define time and intensity for example with known result
     time = 2 + 0.1 * np.arange(17)
     intensity = [1, 5, 3] + 11 * [1000] + [7, 9, 11]
     # define expected results
-    expected_noise_width = np.ptp([1, 5, 3, 7, 9, 11])
     expected_baseline_fit = st.linregress([2, 2.1, 2.2, 3.4, 3.5, 3.6], [1, 5, 3, 7, 9, 11])
     # get the values from the initial guesses function
     slope, intercept, noise_width = models.initial_guesses(time, intensity)
     # compare the outcome with the expected values
     assert expected_baseline_fit.slope == slope
     assert expected_baseline_fit.intercept == intercept
-    assert expected_noise_width == noise_width
+    # With this example the noise is clipped to at least 10
+    assert noise_width == 10
+    pass
+
+
+def test_zsn_sorting():
+    """This tests a workaround that we rely on for multi-peak models."""
+    coords = {
+        "thing": ["left", "center", "right"],
+    }
+    with pm.Model(coords=coords) as pmodel:
+        hyper = pm.Normal("hyper", mu=0, sigma=3)
+        offset_unsorted = pm.ZeroSumNormal(
+            "offset_unsorted",
+            sigma=1,
+            shape=3,
+        )
+        # Create a sorted deterministic without using transforms
+        offset = pm.Deterministic("offset", pt.sort(offset_unsorted), dims="thing")
+        pos = pm.Deterministic(
+            "pos",
+            hyper + offset,
+            dims="thing",
+        )
+        # Observe the two things in incorrect order to provoke the model 😈
+        dat = pm.Data("dat", [0.2, 0.05, -0.3], dims="thing")
+        pm.Normal("L", pos, observed=dat, dims="thing")
+
+    # Check draws from the prior
+    drawn = pm.draw(offset, draws=69)
+    np.testing.assert_array_less(drawn[:, 0], drawn[:, 1])
+
+    # And check MCMC draws too
+    with pmodel:
+        idata = pm.sample(
+            chains=1, tune=10, draws=69, step=pm.Metropolis(), compute_convergence_checks=False
+        )
+    for vname in ["offset", "pos"]:
+        np.testing.assert_array_less(
+            idata.posterior[vname].sel(thing="left"),
+            idata.posterior[vname].sel(thing="center"),
+        )
+        np.testing.assert_array_less(
+            idata.posterior[vname].sel(thing="center"),
+            idata.posterior[vname].sel(thing="right"),
+        )
     pass
 
 
 class TestDistributions:
-    def test_normal_posterior(self):
+    def test_normal_peak_shape(self):
         x = np.linspace(-5, 10, 10000)
         expected = st.norm.pdf(x, 3, 2)
-        actual_pt = models.normal_posterior(0, x, 3, 2, height=np.max(expected))
+        actual_pt = models.normal_peak_shape(0, x, 3, 2, height=np.max(expected))
         # cast arrays to float data type in order to avoid error of np.testing.assert_allclose() due to using np.isfinite under the hood
         actual = actual_pt.eval().astype(float)
         expected = expected.astype(float)
         # testing; allow minor difference due to differences in float precision etc.
         np.testing.assert_allclose(expected, actual, atol=0.0000001)
         pass
 
-    def test_double_normal_posterior(self):
+    def test_double_normal_peak_shape(self):
         x = np.linspace(5, 12, 10000)
         y1 = st.norm.pdf(x, loc=7.5, scale=0.6)
         y2 = st.norm.pdf(x, loc=9, scale=0.4) * 2
-        y_double_pt = models.double_normal_posterior(
+        y_double_pt = models.double_normal_peak_shape(
             0, x, (7.5, 9), (0.6, 0.4), height=(np.max(y1), np.max(y2))
         )
         y_double = y_double_pt.eval().astype(float)
         np.testing.assert_allclose(y1 + y2, y_double, rtol=1, atol=1e-20)
         pass
 
     def test_height_calculation_without_baseline(self):
@@ -101,94 +177,113 @@
         actual_height = height_pt.eval().astype(float)
         # testing; allow slight difference due to shift of distribution by baseline
         # (this numerical calculation does not consider the baseline)
         np.testing.assert_allclose(expected_height, actual_height, atol=1e-4)
         np.testing.assert_allclose(expected_mode_skew, actual_mode, atol=5e-3)
         pass
 
-    def test_skew_normal_posterior(self):
+    def test_skew_normal_peak_shape(self):
         x = np.linspace(-1, 5.5, 10000)
         # test first with positive alpha
         expected = st.skewnorm.pdf(x, 3, loc=1.2, scale=1.1)
-        actual_pt = models.skew_normal_posterior(0, x, 1.2, 1.1, 3, area=1)
+        actual_pt = models.skew_normal_peak_shape(0, x, 1.2, 1.1, 3, area=1)
         # cast arrays to float data type in order to avoid error of np.testing.assert_allclose() due to using np.isfinite under the hood
         actual = actual_pt.eval().astype(float)
         expected = expected.astype(float)
         # testing; allow minor difference due to differences in float precision etc.
         np.testing.assert_allclose(expected, actual, atol=1e-8)
 
         # test again with negative alpha
         expected = st.skewnorm.pdf(x, -3, loc=1.2, scale=1.1)
-        actual_pt = models.skew_normal_posterior(0, x, 1.2, 1.1, -3, area=1)
+        actual_pt = models.skew_normal_peak_shape(0, x, 1.2, 1.1, -3, area=1)
         # cast arrays to float data type in order to avoid error of np.testing.assert_allclose() due to using np.isfinite under the hood
         actual = actual_pt.eval().astype(float)
         expected = expected.astype(float)
         # testing; allow minor difference due to differences in float precision etc.
         np.testing.assert_allclose(expected, actual, atol=1e-8)
         pass
 
     def test_compare_normal_and_skew_as_normal(self):
         """A skew normal distribution with skewness alpha = 0 should be a normal distribution. Test if that is so for our distributions."""
         x = np.linspace(-10, 10, 10000)
         y = st.norm.pdf(x, loc=1, scale=0.5)
         height = np.max(y)
         area = scipy.integrate.quad(lambda x: st.norm.pdf(x, loc=1, scale=1), -10, 10)[0]
         x = np.linspace(-10, 10, 10000)
-        y_actual_pt = models.normal_posterior(0, x, 1, 1, height=height)
-        y_skew_actual_pt = models.skew_normal_posterior(0, x, 1, 1, 0, area=area)
+        y_actual_pt = models.normal_peak_shape(0, x, 1, 1, height=height)
+        y_skew_actual_pt = models.skew_normal_peak_shape(0, x, 1, 1, 0, area=area)
         y_actual = y_actual_pt.eval().astype(float)
         y_skew_actual = y_skew_actual_pt.eval().astype(float)
         # many values are extremely close to zero so rtol was increased.
         # As guaranteed by the absurdly low atol, this will not mask any actual differences.
         np.testing.assert_allclose(y_skew_actual, y_actual, atol=1e-20, rtol=0.9)
         pass
 
-    def test_double_skew_normal_posterior(self):
+    def test_double_skew_normal_peak_shape(self):
         x1 = np.arange(4, 6, 0.1)
         x2 = np.arange(6, 8, 0.1)
         alpha = 5
         y1 = st.skewnorm.pdf(x1, alpha, loc=5, scale=0.2)
         y2 = st.skewnorm.pdf(x2, alpha, loc=6.3, scale=0.2)
         time = np.array(list(x1) + list(x2))
         intensity = np.array(list(y1) + list(y2))
-        y_double_pt = models.double_skew_normal_posterior(
+        y_double_pt = models.double_skew_normal_peak_shape(
             0, time, (5, 6.3), (0.2, 0.2), (5, 5), area=(1, 1)
         )
         y_double = y_double_pt.eval().astype(float)
         np.testing.assert_allclose(intensity, y_double, rtol=1, atol=1e-20)
 
 
 @pytest.mark.parametrize(
-    "model_type", ["normal", "skew_normal", "double_normal", "double_skew_normal"]
+    "define_func",
+    [
+        models.define_model_normal,
+        models.define_model_skew,
+    ],
 )
-def test_pymc_sampling(model_type):
-    timeseries = np.load(
-        Path(__file__).absolute().parent.parent / "example" / "A2t2R1Part1_132_85.9_86.1.npy"
-    )
+def test_singlepeak_sampling(define_func):
+    timeseries = np.load(_DP_ROOT / "example" / "A2t2R1Part1_132_85.9_86.1.npy")
+
+    pmodel = define_func(timeseries[0], timeseries[1])
+    with pmodel:
+        idata = pm.sample(cores=2, chains=2, tune=3, draws=5)
+    assert set(idata.posterior.keys()) >= _REQUIRED_VARIABLES
+    assert set(idata.constant_data.keys()) >= _REQUIRED_DATA
+    pass
 
-    if model_type == models.ModelType.Normal:
-        pmodel = models.define_model_normal(timeseries[0], timeseries[1])
-    elif model_type == models.ModelType.SkewNormal:
-        pmodel = models.define_model_skew(timeseries[0], timeseries[1])
-    elif model_type == models.ModelType.DoubleNormal:
-        pmodel = models.define_model_double_normal(timeseries[0], timeseries[1])
-    elif model_type == models.ModelType.DoubleSkewNormal:
-        pmodel = models.define_model_double_skew_normal(timeseries[0], timeseries[1])
+
+@pytest.mark.parametrize(
+    "define_func",
+    [
+        models.define_model_double_normal,
+        models.define_model_double_skew_normal,
+    ],
+)
+def test_doublepeak_sampling(define_func):
+    timeseries = np.load(_DP_ROOT / "example" / "A2t2R1Part1_132_85.9_86.1.npy")
+
+    pmodel = define_func(timeseries[0], timeseries[1])
     with pmodel:
         idata = pm.sample(cores=2, chains=2, tune=3, draws=5)
-    if model_type in [models.ModelType.DoubleNormal, models.ModelType.DoubleSkewNormal]:
-        summary = az.summary(idata)
-        # test whether the ordered transformation and the subpeak dimension work as intended
-        assert summary.loc["mean[0]", "mean"] < summary.loc["mean[1]", "mean"]
-        # assert summary.loc["area[0]", "mean"] < summary.loc["area[1]", "mean"]
+    assert set(idata.posterior.keys()) >= _REQUIRED_VARIABLES
+    assert set(idata.constant_data.keys()) >= _REQUIRED_DATA
+    # Confirm the order of peaks is as intended
+    np.testing.assert_array_less(
+        idata.posterior["offset"].sel(subpeak=0),
+        idata.posterior["offset"].sel(subpeak=1),
+    )
+    np.testing.assert_array_less(
+        idata.posterior["mean"].sel(subpeak=0),
+        idata.posterior["mean"].sel(subpeak=1),
+    )
     pass
 
 
 def test_model_comparison():
-    path = Path(__file__).absolute().parent.parent / "test_data/test_model_comparison"
+    path = _DP_ROOT / "test_data/test_model_comparison"
     idata_normal = az.from_netcdf(path / "idata_normal.nc")
     idata_skew = az.from_netcdf(path / "idata_skew.nc")
     compare_dict = {
         "normal": idata_normal,
         "skew_normal": idata_skew,
     }
     ranking = models.model_comparison(compare_dict)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## peak_performance/test_pipeline.py

```diff
@@ -632,19 +632,26 @@
         {"elpd_loo": [50, 30, 29, -5], "ic": ["loo", "loo", "loo", "loo"]},
         index=["double_normal", "double_skew_normal", "normal", "skew_normal"],
     )
     selected_model = pl.model_selection_check(result_df, "loo", 25)
     assert selected_model == "normal"
     # case 2: double peak exceeds elpd score difference threshold and is thusly accepted
     result_df = pandas.DataFrame(
-        {"elpd_loo": [50, 30, 10, -5], "ic": ["loo", "loo", "loo", "loo"]},
+        {"elpd_loo": [50, 30, 20, -5], "ic": ["loo", "loo", "loo", "loo"]},
         index=["double_normal", "double_skew_normal", "normal", "skew_normal"],
     )
     selected_model = pl.model_selection_check(result_df, "loo", 25)
     assert selected_model == "double_normal"
+    # case 3: single peak models were excluded
+    result_df = pandas.DataFrame(
+        {"elpd_loo": [50, 30], "ic": ["loo", "loo"]},
+        index=["double_normal", "double_skew_normal"],
+    )
+    selected_model = pl.model_selection_check(result_df, "loo", 25)
+    assert selected_model == "double_normal"
     pass
 
 
 def test_model_selection():
     """
     Test the model_selection function from the pipeline modul.
     The function contains the model selection pipeline.
```

## Comparing `peak_performance-0.6.4.dist-info/LICENSE.md` & `peak_performance-0.7.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `peak_performance-0.6.4.dist-info/METADATA` & `peak_performance-0.7.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-performance
-Version: 0.6.4
+Version: 0.7.0
 Summary: A Python toolbox to fit chromatography peaks with uncertainty.
 Author-email: Jochen Nießer <j.niesser@fz-juelich.de>, Michael Osthege <m.osthege@fz-juelich.de>
 License: AGPLv3
 Project-URL: homepage, https://jugit.fz-juelich.de/IBG-1/micropro/peak-performance
 Project-URL: documentation, https://jugit.fz-juelich.de/IBG-1/micropro/peak-performance
 Project-URL: repository, https://jugit.fz-juelich.de/IBG-1/micropro/peak-performance
 Keywords: hplc,mass-spectrometry,uncertainty quantification
@@ -20,48 +20,49 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pymc >=5.9.1
 Requires-Dist: pytensor
 Requires-Dist: scipy
 Requires-Dist: openpyxl
 Requires-Dist: numpy <1.26.0
-Provides-Extra: test
-Requires-Dist: pytest ; extra == 'test'
-Requires-Dist: pytest-cov ; extra == 'test'
-Requires-Dist: twine ; extra == 'test'
-
-[![PyPI version](https://img.shields.io/pypi/v/bletl)](https://pypi.org/project/peak-performance/)
-[![pipeline](https://github.com/jubiotech/bletl/workflows/pipeline/badge.svg)](https://github.com/JuBiotech/peak-performance/actions)
-[![coverage](https://codecov.io/gh/jubiotech/bletl/branch/main/graph/badge.svg)](https://app.codecov.io/gh/JuBiotech/peak-performance)
+
+[![PyPI version](https://img.shields.io/pypi/v/peak-performance)](https://pypi.org/project/peak-performance/)
+[![pipeline](https://github.com/jubiotech/peak-performance/workflows/pipeline/badge.svg)](https://github.com/JuBiotech/peak-performance/actions)
+[![coverage](https://codecov.io/gh/jubiotech/peak-performance/branch/main/graph/badge.svg)](https://app.codecov.io/gh/JuBiotech/peak-performance)
+[![documentation](https://readthedocs.org/projects/peak-performance/badge/?version=latest)](https://peak-performance.readthedocs.io/en/latest)
+[![DOI](https://zenodo.org/badge/713469041.svg)](https://zenodo.org/doi/10.5281/zenodo.10255543)
 
 # How to use PeakPerformance
 For installation instructions, see `Installation.md`.
 For instructions regarding the use of PeakPerformance, check out the example notebook(s) under `notebooks`, the complementary example data under `example`, and the following introductory explanations.
 
 ## Preparing raw data
 This step is crucial when using PeakPerformance. Raw data has to be supplied as time series meaning for each signal you want to analyze, save a NumPy array consisting of time in the first dimension and intensity in the second dimension (compare example data). Both time and intensity should also be NumPy arrays. If you e.g. have time and intensity of a singal as lists, you can use the following code to convert, format, and save them in the correct manner:
-```
+
+```python
 import numpy as np
 from pathlib import Path
 
 time_series = np.array([np.array(time), np.array(intensity)])
 np.save(Path(r"example_path/time_series.npy"), time_series)
 ```
+
 The naming convention of raw data files is `<acquisition name>_<precursor ion m/z or experiment number>_<product ion m/z start>_<product ion m/z end>.npy`. There should be no underscores within the named sections such as `acquisition name`. Essentially, the raw data names include the acquisition and mass trace, thus yielding a recognizable and unique name for each isotopomer/fragment/metabolite/sample.
 
 ## Model selection
 When it comes to selecting models, PeakPerformance has a function performing an automated selection process by analyzing one acquisiton per mass trace with all implemented models. Subsequently, all models are ranked based on an information criterion (either pareto-smoothed importance sampling leave-one-out cross-validation or widely applicable information criterion). For this process to work as intended, you need to specify acquisitions with representative peaks for each mass trace (see example notebook 1). If e.g. most peaks of an analyte show a skewed shape, then select an acquisition where this is the case. For double peaks, select an acquision where the peaks are as distinct and comparable in height as possible.
 Since model selection is a computationally demanding and time consuming process, it is suggested to state the model type as the user (see example notebook 1) if possible.
 
 ## Troubleshooting
 ### A batch run broke and I want to restart it.
 If an error occured in the middle of a batch run, then you can use the `pipeline_restart` function in the `pipeline` module to create a new batch which will analyze only those samples, which have not been analyzed previously.
 
 ### The model parameters don't converge and/or the fit does not describe the raw data well.
-Check the separate file `How to adapt PeakPerformance to you data`.
+Check the separate file `How to adapt PeakPerformance to your data`.
 
 # How to contribute
 If you encounter bugs while using PeakPerformance, please bring them to our attention by opening an issue. When doing so, describe the problem in detail and add screenshots/code snippets and whatever other helpful material you can provide.
 When contributing code, create a local clone of PeakPerformance, create a new branch, and open a pull request (PR).
 
 # How to cite
-Will be updated once the paper has been released and a zenodo DOI has been created.
+Head over to Zenodo to [generate a BibTeX citation](https://doi.org/10.5281/zenodo.10255543) for the latest release.
+A publication has just been submitted to a scientific journal. Once published, this section will be updated.
```

## Comparing `peak_performance-0.6.4.dist-info/RECORD` & `peak_performance-0.7.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 peak_performance/__init__.py,sha256=yTq4THYewbWRnrs2Qkv4nCd-7MyvDlu_t0fPeWeKxQc,261
-peak_performance/models.py,sha256=L47mNU1HItYv5cB-cs2H0ooswhdcLfBdg8X1MHeiTUY,25130
-peak_performance/pipeline.py,sha256=A-eIwhbn9hCIvWgrG5ksfQLn--ISBKVBjq09nVDwFO8,64311
-peak_performance/plots.py,sha256=OO5rSC-kTCzH8-Fh0diz0Cq86fyrZ_FSOiDjcboZRAU,9280
+peak_performance/models.py,sha256=HpJzjf9Eq1ZXUxKlX6GZDj21icL4s_G0naJrCgWntcM,27457
+peak_performance/pipeline.py,sha256=8yy2-hTNozBJeLE_dulQJCzCBWv2CoRRdXSHDN2UwD8,64395
+peak_performance/plots.py,sha256=5F-s7ZcFgZuN5xGIWRSJ5-_Pl99-vqbcr3F8dYnBFQc,9455
 peak_performance/test_main.py,sha256=xQiLDjhldxZzY5sp3RyIJUTtXxX46auWY9Qy7nuifxw,97
-peak_performance/test_models.py,sha256=X3fy-kNih7TNrr4jKzgcx8qRnmh6cA27hSr2b6Tmf18,9334
-peak_performance/test_pipeline.py,sha256=wyzVgVYT0pK_Lnh5VZEgL8Rxn8sjiCa1dRp1tF79foM,22652
+peak_performance/test_models.py,sha256=r6kqAVBtAbycf4IoRaXcSCZp6Lras3afK6o9qcLZbH8,11592
+peak_performance/test_pipeline.py,sha256=gTZAxcJEVwJ0XW4IewmIWGLmx1n7KaK8egrovKHsCFI,22961
 peak_performance/test_plots.py,sha256=lGwPWzezAhzEnyu_NMx2lFtyzzb1wxy-jnRMtOaaniY,4100
-peak_performance-0.6.4.dist-info/LICENSE.md,sha256=zj-4LZ7oChyw5Uj5sFYOrVI3juK06Cb9lFm0rPcHXYk,32387
-peak_performance-0.6.4.dist-info/METADATA,sha256=X7qWgjCWDwi9KseQnDasaijG0k9u-L6CbGTH0qj8Zd4,4796
-peak_performance-0.6.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-peak_performance-0.6.4.dist-info/top_level.txt,sha256=-lZSmgn2fZA-xPVmddLwaRt2hQeeWj7TYVefOk7_T58,17
-peak_performance-0.6.4.dist-info/RECORD,,
+peak_performance-0.7.0.dist-info/LICENSE.md,sha256=zj-4LZ7oChyw5Uj5sFYOrVI3juK06Cb9lFm0rPcHXYk,32387
+peak_performance-0.7.0.dist-info/METADATA,sha256=uAz1t9qggYqguLgLPJ611PjUOYKM8CWJQLXbH3u8RsY,5076
+peak_performance-0.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+peak_performance-0.7.0.dist-info/top_level.txt,sha256=-lZSmgn2fZA-xPVmddLwaRt2hQeeWj7TYVefOk7_T58,17
+peak_performance-0.7.0.dist-info/RECORD,,
```

