# Comparing `tmp/pyretailscience-0.3.1.tar.gz` & `tmp/pyretailscience-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyretailscience-0.3.1.tar", max compression
+gzip compressed data, was "pyretailscience-0.3.2.tar", max compression
```

## Comparing `pyretailscience-0.3.1.tar` & `pyretailscience-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     3860 2024-05-05 14:29:57.465611 pyretailscience-0.3.1/LICENSE
--rw-r--r--   0        0        0     2701 2024-05-05 14:29:57.465611 pyretailscience-0.3.1/README.md
--rw-r--r--   0        0        0     1056 2024-05-05 14:31:03.313428 pyretailscience-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/__init__.py
--rw-r--r--   0        0        0    15090 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/customer.py
--rw-r--r--   0        0        0        0 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/__init__.py
--rw-r--r--   0        0        0     1165 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/cli.py
--rw-r--r--   0        0        0    17162 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/contracts.py
--rw-r--r--   0        0        0    16021 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/simulation.py
--rw-r--r--   0        0        0    12898 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/range_planning.py
--rw-r--r--   0        0        0     9192 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/segmentation.py
--rw-r--r--   0        0        0     3528 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/standard_graphs.py
--rw-r--r--   0        0        0     2488 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/style/graph_utils.py
--rw-r--r--   0        0        0     9316 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/style/tailwind.py
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 pyretailscience-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2024-05-14 10:21:07.329111 pyretailscience-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2701 2024-05-14 10:21:07.329111 pyretailscience-0.3.2/README.md
+-rw-r--r--   0        0        0     1056 2024-05-14 10:22:16.281334 pyretailscience-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 10:21:07.337111 pyretailscience-0.3.2/pyretailscience/__init__.py
+-rw-r--r--   0        0        0   153944 2024-05-14 10:21:07.337111 pyretailscience-0.3.2/pyretailscience/assets/fonts/Poppins-Bold.ttf
+-rw-r--r--   0        0        0   184460 2024-05-14 10:21:07.337111 pyretailscience-0.3.2/pyretailscience/assets/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0        0        0   156520 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/assets/fonts/Poppins-Medium.ttf
+-rw-r--r--   0        0        0   158240 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/assets/fonts/Poppins-Regular.ttf
+-rw-r--r--   0        0        0   155232 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/assets/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0        0        0    16211 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/customer.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/data/__init__.py
+-rw-r--r--   0        0        0     1165 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/data/cli.py
+-rw-r--r--   0        0        0    17162 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/data/contracts.py
+-rw-r--r--   0        0        0    16021 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/data/simulation.py
+-rw-r--r--   0        0        0    13536 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/range_planning.py
+-rw-r--r--   0        0        0    11601 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/segmentation.py
+-rw-r--r--   0        0        0    12827 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/standard_graphs.py
+-rw-r--r--   0        0        0     4032 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/style/graph_utils.py
+-rw-r--r--   0        0        0     9316 2024-05-14 10:21:07.341111 pyretailscience-0.3.2/pyretailscience/style/tailwind.py
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 pyretailscience-0.3.2/PKG-INFO
```

### Comparing `pyretailscience-0.3.1/LICENSE` & `pyretailscience-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/README.md` & `pyretailscience-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/pyproject.toml` & `pyretailscience-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyretailscience"
-version = "0.3.1"
+version = "0.3.2"
 description = "Retail Data Science Tools"
 authors = ["Murray Vanwyk <2493311+mvanwyk@users.noreply.github.com>"]
 readme = "README.md"
 license = "Elastic-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `pyretailscience-0.3.1/pyretailscience/customer.py` & `pyretailscience-0.3.2/pyretailscience/customer.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import matplotlib.ticker as mtick
 import pandas as pd
 from matplotlib.axes import Axes, SubplotBase
 
 from pyretailscience.data.contracts import TransactionItemLevelContract
 from pyretailscience.style.graph_utils import GraphStyles as gs
+import pyretailscience.style.graph_utils as gu
 from pyretailscience.style.graph_utils import human_format, standard_graph_styles
 from pyretailscience.style.tailwind import COLORS
 
 
 class PurchasesPerCustomer:
     """A class to plot the distribution of the number of purchases per customer.
 
@@ -32,16 +33,16 @@
         bins: int = 10,
         cumlative: bool = False,
         ax: Axes | None = None,
         draw_percentile_line: bool = False,
         percentile_line: float = 0.5,
         source_text: str | None = None,
         title: str | None = None,
-        xlabel: str | None = None,
-        ylabel: str | None = None,
+        x_label: str | None = None,
+        y_label: str | None = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the distribution of the number of purchases per customer.
 
         Args:
             bins (int, optional): The number of bins to plot. Defaults to 10.
             cumlative (bool, optional): Whether to plot the cumulative distribution. Defaults to False.
@@ -54,47 +55,58 @@
             SubplotBase: The Matplotlib axes of the plot
         """
 
         density = False
         if cumlative:
             density = True
 
-        if xlabel is None:
-            xlabel = "Number of purchases"
+        if x_label is None:
+            x_label = "Number of purchases"
 
         ax = self.cust_purchases_s.hist(
             bins=bins,
             cumulative=cumlative,
             ax=ax,
             density=density,
             color=COLORS["green"][500],
             **kwargs,
         )
 
-        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_xlabel(
+            x_label,
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
         ax.xaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
         ax = standard_graph_styles(ax)
 
         if cumlative:
-            if title is None:
-                title = "Number of Purchases Cumulative Distribution"
-            if ylabel is None:
-                ylabel = "Percentage of customers"
+            default_title = "Number of Purchases Cumulative Distribution"
+            default_y_label = "Percentage of customers"
             ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1, decimals=0))
 
         else:
-            if title is None:
-                title = "Number of Purchases Distribution"
-            if ylabel is None:
-                ylabel = "Number of customers"
+            default_title = "Number of Purchases Distribution"
+            default_y_label = "Number of customers"
             ax.yaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
-        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
-        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_title(
+            gu.not_none(title, default_title),
+            fontproperties=gs.POPPINS_SEMI_BOLD,
+            fontsize=gs.DEFAULT_TITLE_FONT_SIZE,
+            pad=gs.DEFAULT_TITLE_PAD,
+        )
+        ax.set_ylabel(
+            gu.not_none(y_label, default_y_label),
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
 
         if draw_percentile_line:
             if percentile_line > 1 or percentile_line < 0:
                 raise ValueError("Percentile line must be between 0 and 1")
             ax.axvline(
                 x=self.purchases_percentile(percentile_line),
                 color=COLORS["red"][500],
@@ -108,14 +120,16 @@
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
                 fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
+                fontproperties=gs.POPPINS_LIGHT_ITALIC,
+                color="dimgray",
             )
 
         return ax
 
     def purchases_percentile(self, percentile: float = 0.5) -> float:
         """Get the number of purchases at a given percentile.
 
@@ -188,16 +202,16 @@
         self,
         bins: int = 10,
         cumlative: bool = False,
         ax: Axes | None = None,
         draw_percentile_line: bool = False,
         percentile_line: float = 0.5,
         title: str | None = None,
-        xlabel: str | None = None,
-        ylabel: str | None = None,
+        x_label: str | None = None,
+        y_label: str | None = None,
         source_text: str = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the distribution of the average number of days between purchases per customer.
 
         Args:
             bins (int, optional): The number of bins to plot. Defaults to 10.
@@ -219,37 +233,46 @@
             cumulative=cumlative,
             ax=ax,
             density=density,
             color=COLORS["green"][500],
             **kwargs,
         )
 
-        if xlabel is None:
-            xlabel = "Average Number of Days Between Purchases"
-        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_xlabel(
+            gu.not_none(x_label, "Average Number of Days Between Purchases"),
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
         ax.xaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
         ax = standard_graph_styles(ax)
 
         if cumlative:
-            if title is None:
-                title = "Average Days Between Purchases Cumulative Distribution"
-            if ylabel is None:
-                ylabel = "Percentage of Customers"
+            default_title = "Average Days Between Purchases Cumulative Distribution"
+            default_y_label = "Percentage of Customers"
             ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1, decimals=0))
 
         else:
-            if title is None:
-                title = "Average Days Between Purchases Distribution"
-            if ylabel is None:
-                ylabel = "Number of Customers"
+            default_title = "Average Days Between Purchases Distribution"
+            default_y_label = "Number of Customers"
             ax.yaxis.set_major_formatter(lambda x, pos: human_format(x, pos, decimals=0))
 
-        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
-        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
+        ax.set_title(
+            gu.not_none(title, default_title),
+            fontproperties=gs.POPPINS_SEMI_BOLD,
+            fontsize=gs.DEFAULT_TITLE_FONT_SIZE,
+            pad=gs.DEFAULT_TITLE_PAD,
+        )
+        ax.set_ylabel(
+            gu.not_none(y_label, default_y_label),
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
 
         if draw_percentile_line:
             if percentile_line > 1 or percentile_line < 0:
                 raise ValueError("Percentile line must be between 0 and 1")
             ax.axvline(
                 x=self.purchases_percentile(percentile_line),
                 color=COLORS["red"][500],
@@ -264,14 +287,16 @@
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
                 fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
+                fontproperties=gs.POPPINS_LIGHT_ITALIC,
+                color="dimgray",
             )
 
         return ax
 
     def purchases_percentile(self, percentile: float = 0.5) -> float:
         """Get the average number of days between purchases at a given percentile.
 
@@ -331,16 +356,16 @@
         self.n_unique_customers = df["customer_id"].nunique()
 
     def plot(
         self,
         cumlative: bool = False,
         ax: Axes | None = None,
         title: str | None = None,
-        xlabel: str | None = None,
-        ylabel: str | None = None,
+        x_label: str | None = None,
+        y_label: str | None = None,
         source_text: str = None,
         **kwargs: dict[str, any],
     ) -> SubplotBase:
         """Plot the churn rate by number of purchases.
 
         Args:
             cumlative (bool, optional): Whether to plot the cumulative distribution. Defaults to False.
@@ -362,30 +387,40 @@
                 color=COLORS["green"][500],
                 width=0.8,
                 **kwargs,
             )
 
         standard_graph_styles(ax)
 
-        if title is None:
-            title = "Churn Rate by Number of Purchases"
-        if xlabel is None:
-            xlabel = "Number of Purchases"
-        if ylabel is None:
-            ylabel = "% Churned"
-
         ax.yaxis.set_major_formatter(mtick.PercentFormatter(xmax=1.0))
-        ax.set_xlabel(xlabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
-        ax.set_ylabel(ylabel, fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE, labelpad=10)
-        ax.set_title(title, fontsize=gs.DEFAULT_TITLE_FONT_SIZE, pad=15)
+        ax.set_xlabel(
+            gu.not_none(x_label, "Number of Purchases"),
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
+        ax.set_ylabel(
+            gu.not_none(y_label, "% Churned"),
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
+        ax.set_title(
+            gu.not_none(title, "Churn Rate by Number of Purchases"),
+            fontproperties=gs.POPPINS_SEMI_BOLD,
+            fontsize=gs.DEFAULT_TITLE_FONT_SIZE,
+            pad=gs.DEFAULT_TITLE_PAD,
+        )
 
         if source_text:
             ax.annotate(
                 source_text,
                 xy=(-0.1, -0.2),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
                 fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
+                fontproperties=gs.POPPINS_LIGHT_ITALIC,
+                color="dimgray",
             )
 
         return ax
```

### Comparing `pyretailscience-0.3.1/pyretailscience/data/cli.py` & `pyretailscience-0.3.2/pyretailscience/data/cli.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/pyretailscience/data/contracts.py` & `pyretailscience-0.3.2/pyretailscience/data/contracts.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/pyretailscience/data/simulation.py` & `pyretailscience-0.3.2/pyretailscience/data/simulation.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/pyretailscience/range_planning.py` & `pyretailscience-0.3.2/pyretailscience/range_planning.py`

 * *Files 7% similar despite different names*

```diff
@@ -259,26 +259,29 @@
             default_y_label = "Distance"
         else:
             default_x_label = "Distance"
             default_y_label = "Products"
 
         ax.set_title(
             title,
+            fontproperties=gs.POPPINS_SEMI_BOLD,
             fontsize=gs.DEFAULT_TITLE_FONT_SIZE,
-            pad=15,
+            pad=gs.DEFAULT_TITLE_PAD + 5,
         )
         ax.set_xlabel(
-            gu.not_none(y_label, default_x_label),
+            gu.not_none(x_label, default_x_label),
+            fontproperties=gs.POPPINS_REG,
             fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
-            labelpad=10,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
         )
         ax.set_ylabel(
-            gu.not_none(x_label, default_y_label),
+            gu.not_none(y_label, default_y_label),
+            fontproperties=gs.POPPINS_REG,
             fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
-            labelpad=10,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
         )
 
         # Set the y label to be on the right side of the plot
         if orientation == "left":
             ax.yaxis.tick_right()
             ax.yaxis.set_label_position("right")
         if orientation == "bottom":
@@ -305,15 +308,25 @@
             ax.annotate(
                 source_text,
                 xy=(x_axis_offset, y_axis_offset),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
                 fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
+                fontproperties=gs.POPPINS_LIGHT_ITALIC,
+                color="dimgray",
             )
 
+        ax.xaxis.set_tick_params(labelsize=gs.DEFAULT_TICK_LABEL_FONT_SIZE)
+        ax.yaxis.set_tick_params(labelsize=gs.DEFAULT_TICK_LABEL_FONT_SIZE)
+
+        # Rotate the x-axis labels if they are too long
         if orientation in ["top", "bottom"]:
-            ax.xaxis.set_tick_params(labelsize=gs.DEFAULT_TICK_LABEL_FONT_SIZE)
-        else:
-            ax.yaxis.set_tick_params(labelsize=gs.DEFAULT_TICK_LABEL_FONT_SIZE)
+            plt.setp(ax.get_xticklabels(), rotation=45, ha="right")
+
+        # Set the font properties for the tick labels
+        for tick in ax.get_xticklabels():
+            tick.set_fontproperties(gs.POPPINS_REG)
+        for tick in ax.get_yticklabels():
+            tick.set_fontproperties(gs.POPPINS_REG)
 
         return ax
```

### Comparing `pyretailscience-0.3.1/pyretailscience/segmentation.py` & `pyretailscience-0.3.2/pyretailscience/segmentation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,131 @@
 from typing import Literal
 
 import pandas as pd
 from matplotlib.axes import Axes, SubplotBase
 
 import pyretailscience.style.graph_utils as gu
-from pyretailscience.data.contracts import TransactionItemLevelContract, TransactionLevelContract
+from pyretailscience.data.contracts import (
+    TransactionItemLevelContract,
+    TransactionLevelContract,
+    CustomContract,
+    build_expected_columns,
+    build_non_null_columns,
+    build_expected_unique_columns,
+)
+from pyretailscience.style.graph_utils import GraphStyles as gs
 from pyretailscience.style.tailwind import COLORS
 
 
-class HMLSegmentation:
-    def __init__(self, df: pd.DataFrame, value_col: str = "total_price") -> None:
+class BaseSegmentation:
+    def add_segment(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Adds the segment to the dataframe based on the customer_id column.
+
+        Args:
+            df (pd.DataFrame): The dataframe to add the segment to. The dataframe must have a customer_id column.
+
+        Returns:
+            pd.DataFrame: The dataframe with the segment added.
+
+        Raises:
+            ValueError: If the number of rows before and after the merge do not match.
+        """
+        rows_before = len(df)
+        df = df.merge(self.df[["segment_name", "segment_id"]], how="left", left_on="customer_id", right_index=True)
+        rows_after = len(df)
+        if rows_before != rows_after:
+            raise ValueError("The number of rows before and after the merge do not match. This should not happen.")
+
+        return df
+
+
+class ExistingSegmentation(BaseSegmentation):
+    def __init__(self, df: pd.DataFrame) -> None:
+        """
+        Segments customers based on an existing segment in the dataframe.
+
+        Args:
+
+            df (pd.DataFrame): A dataframe with the customer_id, segment_name and segment_id columns.
+
+        Raises:
+            ValueError: If the dataframe does not have the columns customer_id, segment_name and segment_id.
+        """
+        required_cols = "customer_id", "segment_name", "segment_id"
+        contract = CustomContract(
+            df,
+            basic_expectations=build_expected_columns(columns=required_cols),
+            extended_expectations=build_non_null_columns(columns=required_cols)
+            + build_expected_unique_columns(columns=[required_cols]),
+        )
+
+        if contract.validate() is False:
+            raise ValueError(
+                f"The dataframe requires the columns {required_cols} and they must be non-null and unique."
+            )
+
+        self.df = df[["customer_id", "segment_name", "segment_id"]].set_index("customer_id")
+
+
+class HMLSegmentation(BaseSegmentation):
+    def __init__(
+        self,
+        df: pd.DataFrame,
+        value_col: str = "total_price",
+        zero_value_customers: Literal["separate_segment", "exclude", "include_with_light"] = "separate_segment",
+    ) -> None:
         """
         Segments customers into Heavy, Medium, Light and Zero spenders based on the total spend.
 
         Args:
-            df (pd.DataFrame): A dataframe with the transaction data. The dataframe must comply with the
-                TransactionItemLevelContract or the TransactionLevelContract.
+            df (pd.DataFrame): A dataframe with the transaction data. The dataframe must contain a customer_id column.
             value_col (str, optional): The column to use for the segmentation. Defaults to "total_price".
 
         Raises:
-            ValueError: If the dataframe does not comply with the TransactionItemLevelContract or
-                TransactionLevelContract.
+            ValueError: If the dataframe is missing the columns "customer_id" or `value_col`, or these columns contain
+                null values.
         """
+        required_cols = ["customer_id", value_col]
+        contract = CustomContract(
+            df,
+            basic_expectations=build_expected_columns(columns=required_cols),
+            extended_expectations=build_non_null_columns(columns=required_cols),
+        )
 
-        if TransactionItemLevelContract(df).validate() is False and TransactionLevelContract(df).validate() is False:
-            raise ValueError("The dataframe does not comply with the TransactionItemLevelContract")
+        if contract.validate() is False:
+            raise ValueError(f"The dataframe requires the columns {required_cols} and they must be non-null")
 
         # Group by customer_id and calculate total_spend
         grouped_df = df.groupby("customer_id")[value_col].sum().to_frame(value_col)
 
         # Separate customers with zero spend
-        zero_idx = grouped_df[value_col] == 0
-        zero_cust_df = grouped_df[zero_idx]
-        zero_cust_df["segment_name"] = "Zero"
+        hml_df = grouped_df
+        if zero_value_customers in ["separate_segment", "exclude"]:
+            zero_idx = grouped_df[value_col] == 0
+            zero_cust_df = grouped_df[zero_idx]
+            zero_cust_df["segment_name"] = "Zero"
 
-        hml_df = grouped_df[~zero_idx]
+            hml_df = grouped_df[~zero_idx]
 
         # Create a new column 'segment' based on the total_spend
         hml_df["segment_name"] = pd.qcut(
             hml_df[value_col],
             q=[0, 0.500, 0.800, 1],
             labels=["Light", "Medium", "Heavy"],
         )
 
-        hml_df = pd.concat([hml_df, zero_cust_df])
+        if zero_value_customers == "separate_segment":
+            hml_df = pd.concat([hml_df, zero_cust_df])
 
         segment_code_map = {"Light": "L", "Medium": "M", "Heavy": "H", "Zero": "Z"}
 
         hml_df["segment_id"] = hml_df["segment_name"].map(segment_code_map)
 
-        self.df = grouped_df
-
-    def add_segment(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Adds the segment to the dataframe based on the customer_id column.
-
-        Args:
-            df (pd.DataFrame): The dataframe to add the segment to. The dataframe must have a customer_id column.
-
-        Returns:
-            pd.DataFrame: The dataframe with the segment added.
-
-        Raises:
-            ValueError: If the number of rows before and after the merge do not match.
-        """
-
-        # TODO: Add a contract that ensures there's a customer ID column or matches one or more of a set of contracts
-        # efficently - Eg checks all the quick validations and then tries the extended validations
-
-        rows_before = len(df)
-        df = df.merge(self.df[["segment_name", "segment_id"]], how="left", left_on="customer_id", right_index=True)
-        rows_after = len(df)
-        if rows_before != rows_after:
-            raise ValueError("The number of rows before and after the merge do not match. This should not happen.")
-
-        return df
+        self.df = hml_df
 
 
 class SegTransactionStats:
     def __init__(self, df: pd.DataFrame, segment_col: str = "segment_id") -> None:
         """
         Calculates transaction statistics by segment.
 
@@ -191,22 +238,45 @@
             ax.yaxis.set_major_formatter(lambda x, pos: gu.human_format(x, pos, decimals=decimals))
         else:
             plot_y_label = gu.not_none(y_label, "")
             plot_x_label = gu.not_none(x_label, value_col.title())
             decimals = gu.get_decimals(ax.get_xlim(), ax.get_xticks())
             ax.xaxis.set_major_formatter(lambda x, pos: gu.human_format(x, pos, decimals=decimals))
 
-        ax.set_title(gu.not_none(title, default_title))
-        ax.set_ylabel(plot_y_label)
-        ax.set_xlabel(plot_x_label)
+        ax.set_title(
+            gu.not_none(title, default_title),
+            fontproperties=gs.POPPINS_SEMI_BOLD,
+            fontsize=gs.DEFAULT_TITLE_FONT_SIZE,
+            pad=gs.DEFAULT_TITLE_PAD,
+        )
+        ax.set_ylabel(
+            plot_y_label,
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
+        ax.set_xlabel(
+            plot_x_label,
+            fontproperties=gs.POPPINS_REG,
+            fontsize=gs.DEFAULT_AXIS_LABEL_FONT_SIZE,
+            labelpad=gs.DEFAULT_AXIS_LABEL_PAD,
+        )
 
         if source_text is not None:
             ax.annotate(
                 source_text,
-                xy=(-0.1, -0.2),
+                xy=(-0.1, -0.15),
                 xycoords="axes fraction",
                 ha="left",
                 va="center",
-                fontsize=10,
+                fontsize=gs.DEFAULT_SOURCE_FONT_SIZE,
+                fontproperties=gs.POPPINS_LIGHT_ITALIC,
+                color="dimgray",
             )
 
+        # Set the font properties for the tick labels
+        for tick in ax.get_xticklabels():
+            tick.set_fontproperties(gs.POPPINS_REG)
+        for tick in ax.get_yticklabels():
+            tick.set_fontproperties(gs.POPPINS_REG)
+
         return ax
```

### Comparing `pyretailscience-0.3.1/pyretailscience/style/tailwind.py` & `pyretailscience-0.3.2/pyretailscience/style/tailwind.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.1/PKG-INFO` & `pyretailscience-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyretailscience
-Version: 0.3.1
+Version: 0.3.2
 Summary: Retail Data Science Tools
 License: Elastic-2.0
 Author: Murray Vanwyk
 Author-email: 2493311+mvanwyk@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyretailscience Version: 0.3.1 Summary: Retail Data
+Metadata-Version: 2.1 Name: pyretailscience Version: 0.3.2 Summary: Retail Data
 Science Tools License: Elastic-2.0 Author: Murray Vanwyk Author-email:
 2493311+mvanwyk@users.noreply.github.com Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: great-expectations (>=0.18.8,<0.19.0) Requires-
 Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
```

