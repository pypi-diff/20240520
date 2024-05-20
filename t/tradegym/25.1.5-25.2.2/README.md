# Comparing `tmp/tradegym-25.1.5.tar.gz` & `tmp/tradegym-25.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradegym-25.1.5.tar", max compression
+gzip compressed data, was "tradegym-25.2.2.tar", max compression
```

## Comparing `tradegym-25.1.5.tar` & `tradegym-25.2.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1067 2024-04-22 12:25:53.214503 tradegym-25.1.5/LICENSE
--rw-r--r--   0        0        0     6112 2024-04-22 12:25:53.214503 tradegym-25.1.5/README.md
--rw-r--r--   0        0        0      668 2024-04-22 12:56:08.693633 tradegym-25.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-22 12:56:01.773628 tradegym-25.1.5/tradegym/__init__.py
--rw-r--r--   0        0        0      271 2024-04-22 12:25:53.270503 tradegym-25.1.5/tradegym/agents/__init__.py
--rw-r--r--   0        0        0     2139 2024-04-22 12:25:53.270503 tradegym-25.1.5/tradegym/agents/baseline.py
--rw-r--r--   0        0        0      238 2024-04-22 12:25:53.270503 tradegym-25.1.5/tradegym/agents/sb3.py
--rw-r--r--   0        0        0    13542 2024-04-22 12:58:04.305729 tradegym-25.1.5/tradegym/crossval.py
--rw-r--r--   0        0        0     2478 2024-04-22 12:25:53.270503 tradegym-25.1.5/tradegym/rewards.py
--rw-r--r--   0        0        0    21470 2024-04-22 12:35:33.479547 tradegym-25.1.5/tradegym/tradegym.py
--rw-r--r--   0        0        0     7167 1970-01-01 00:00:00.000000 tradegym-25.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-22 12:25:53.214503 tradegym-25.2.2/LICENSE
+-rw-r--r--   0        0        0     6112 2024-04-22 12:25:53.214503 tradegym-25.2.2/README.md
+-rw-r--r--   0        0        0      653 2024-05-19 19:20:34.298030 tradegym-25.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-19 19:20:40.862038 tradegym-25.2.2/tradegym/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-20 02:15:39.922153 tradegym-25.2.2/tradegym/agents/__init__.py
+-rw-r--r--   0        0        0     2781 2024-05-20 02:15:21.094106 tradegym-25.2.2/tradegym/agents/baseline.py
+-rw-r--r--   0        0        0      256 2024-05-18 22:45:25.500335 tradegym-25.2.2/tradegym/agents/sb3.py
+-rw-r--r--   0        0        0    21344 2024-05-20 01:40:34.677248 tradegym-25.2.2/tradegym/crossval.py
+-rw-r--r--   0        0        0     5771 2024-05-19 21:24:09.840260 tradegym-25.2.2/tradegym/plots.py
+-rw-r--r--   0        0        0     2478 2024-04-22 12:25:53.270503 tradegym-25.2.2/tradegym/rewards.py
+-rw-r--r--   0        0        0    22137 2024-05-20 00:42:32.896313 tradegym-25.2.2/tradegym/tradegym.py
+-rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 tradegym-25.2.2/PKG-INFO
```

### Comparing `tradegym-25.1.5/LICENSE` & `tradegym-25.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tradegym-25.1.5/README.md` & `tradegym-25.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tradegym-25.1.5/pyproject.toml` & `tradegym-25.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "tradegym"
-version = "25.1.5"
+version = "25.2.2"
 description = "trading gym"
 authors = ["Alex-Lekov <61644712+Alex-Lekov@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tradegym"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<4.0"
 gym = "^0.26.2"
-stable-baselines3 = "^2.1.0"
 pytest = "^7.4.0"
 plotly = "^5.16.1"
 quantstats = "^0.0.62"
 empyrical = "^0.5.5"
-torch = ">=2.0.0, !=2.0.1"
 tqdm = "^4.66.1"
 pyyaml = "^6.0.1"
 loguru = "^0.7.0"
 matplotlib = "^3.7.2"
 seaborn = "^0.12.2"
 ipykernel = "^6.25.1"
 shimmy = "^1.2.1"
 nbformat = "^5.9.2"
+vectorbt = "^0.26.1"
+filelock = "^3.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tradegym-25.1.5/tradegym/agents/baseline.py` & `tradegym-25.2.2/tradegym/agents/baseline.py`

 * *Files 22% similar despite different names*

```diff
@@ -60,15 +60,31 @@
     __name__ = "NoTradeAgent"
     def predict(self, obs, deterministic=True):
         action = np.zeros(self.env.action_space.shape)
         #action[-1] = 1.
         return action, None
 
 
+class HalfBuyAndHoldAgent(BaseAgent):
+    __name__ = "BuyAndHoldAgent"
+    def __init__(self, police=None, env=None, symbol='BTC-USDT-PERP', lot_weight_pct=20, **kwargs):
+        super().__init__(police=police, env=env, **kwargs)
+        self.symbol = symbol
+        self.lot_weight_pct = lot_weight_pct
+        self.lot_weight = self.lot_weight_pct / 100
+
+    def predict(self, obs, deterministic=True):
+        action = np.zeros(self.env.action_space.shape)
+        index = self.env.symbols.index(self.symbol)
+        action[index] = self.lot_weight  # Buy coin
+        return action, None
+
+
 #################### Baseline Agents ##################################################
 
 baseline_agents = {
     "BuyAndHoldAgent": BuyAndHoldAgent,
     "RandomAgent": RandomAgent,
     "EqualWeightingAgent": EqualWeightingAgent,
     "NoTradeAgent": NoTradeAgent,
+    "HalfBuyAndHoldAgent": HalfBuyAndHoldAgent,
 }
```

### Comparing `tradegym-25.1.5/tradegym/rewards.py` & `tradegym-25.2.2/tradegym/rewards.py`

 * *Files identical despite different names*

### Comparing `tradegym-25.1.5/tradegym/tradegym.py` & `tradegym-25.2.2/tradegym/tradegym.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,538 +1,528 @@
 import pandas as pd
 import numpy as np
 import gym
 from gym import spaces
-from stable_baselines3.common.vec_env import DummyVecEnv, VecNormalize, SubprocVecEnv
-import empyrical as ep
 from typing import List, Tuple, Any, Optional, Dict
 from tradegym.rewards import all_rewards_func
 
-
 class TradingEnv(gym.Env):
     """Trading environment for reinforcement learning.
 
-    This environment is for training trading algorithms using reinforcement learning. It 
-    allows the agent to take actions representing portfolio weights for different assets.
+    This environment is for training trading algorithms using reinforcement learning.
+    It allows the agent to take actions representing portfolio weights for different assets.
 
     Attributes:
-        metadata: Metadata for the environment rendering.
+        metadata (dict): Metadata for the environment rendering.
     """
     metadata = {"render.modes": ["human"]}
 
-    def __init__(self, 
-            data: pd.DataFrame,
-            window: int = 1, 
-            features_list: list = None,
-            mode_train: bool = False, 
-            random_start_step: bool = False,
-            reward_type: str = "tanh_rew", 
-            reward_settings: dict = {'alpha': 0.19, 'beta': 0.145},
-            risk_free_rate: float = 0.0005,
-            reward_metric_window: int = 24, 
-            init_balance: float = 10_000,
-            verbose: int = 0, 
-            random_seed: int = 10,
-            buy_commission: float = 0.03, # in percentage
-            sell_commission: float = 0.03, # in percentage
-            obs_type: str = 'np' # 'pd'
-            ):
+    def __init__(self,
+                 data: pd.DataFrame,
+                 window: int = 1,
+                 features_list: Optional[List[str]] = None,
+                 mode_train: bool = False,
+                 random_start_step: bool = False,
+                 reward_type: str = "tanh_rew",
+                 reward_settings: dict = {'alpha': 0.19, 'beta': 0.145},
+                 risk_free_rate: float = 0.0005,
+                 reward_metric_window: int = 24,
+                 initial_balance: float = 10_000,
+                 verbose: int = 0,
+                 random_seed: int = 10,
+                 buy_commission_pct: float = 0.03,  # in percentage
+                 sell_commission_pct: float = 0.03,  # in percentage
+                 obs_type: str = 'np',
+                 rebalance_threshold_pct: float = 0.0):  # in percentage
+        """
+        Initializes the trading environment.
+
+        Args:
+            data (pd.DataFrame): Historical market data.
+            window (int): Window size for observation.
+            features_list (Optional[List[str]]): List of feature names to be used.
+            mode_train (bool): Flag for training mode.
+            random_start_step (bool): Flag for random start step.
+            reward_type (str): Type of reward function.
+            reward_settings (dict): Settings for the reward function.
+            risk_free_rate (float): Risk-free rate for reward calculation.
+            reward_metric_window (int): Window size for reward metric.
+            initial_balance (float): Initial balance for the agent.
+            verbose (int): Verbosity level.
+            random_seed (int): Random seed for reproducibility.
+            buy_commission_pct (float): Commission for buying.
+            sell_commission_pct (float): Commission for selling.
+            obs_type (str): Type of observation ('np' или 'pd').
+            rebalance_threshold_pct (float): Threshold for rebalancing the portfolio in percentage.
+
+        Raises:
+            ValueError: If data is None or empty, or if window size is less than or equal to 0.
+        """
+        # Проверка корректности данных
+        if data is None or data.empty:
+            raise ValueError("Data cannot be None or empty.")
         
+        # Проверка корректности размера окна
+        if window <= 0:
+            raise ValueError("Window size must be greater than 0.")
+
+        # Инициализация параметров среды
         self.data = data
         self.window = window
-
-        if features_list is None or len(features_list) == 0:
-            self.features_list = ['open', 'high', 'low', 'close', 'volume']
-        else:
-            self.features_list = features_list
+        self.features_list = features_list if features_list else ['open', 'high', 'low', 'close', 'volume']
         self.reward_settings = reward_settings
         self.mode_train = mode_train
         self.random_start_step = random_start_step
         self.reward_type = reward_type
         self.risk_free_rate = risk_free_rate
         self.reward_metric_window = reward_metric_window
-        self.init_balance = init_balance
+        self.initial_balance = initial_balance
         self.verbose = verbose
         self.random_seed = random_seed
-        self.buy_commission = buy_commission
-        self.sell_commission = sell_commission
+        self.buy_commission_pct = buy_commission_pct
+        self.sell_commission_pct = sell_commission_pct
         self.obs_type = obs_type
+        self.rebalance_threshold = rebalance_threshold_pct / 100  # Convert to decimal
 
-        # data preprocessing
+        # Предобработка данных
         self.data = self.data.sort_values(['date', 'symbol'])
         self.data.reset_index(drop=True, inplace=True)
         self.data.ffill(inplace=True)
         self.data.fillna(0, inplace=True)
 
+        # Проверка на корректность дат
         self._check_dates(self.data)
 
-        fe_lst = self.features_list.copy()
-        fe_lst.extend(['date', 'symbol'])
-        #fe_lst = list(set(('date', 'symbol', *self.features_list)))
+        # Формирование списка фичей
+        feature_columns = self.features_list.copy()
+        feature_columns.extend(['date', 'symbol'])
 
+        # Преобразование данных в 3D тензор для numpy или pandas
         if self.obs_type == 'np':
-            self.fe_data = self._data_to_3d_tensor(self.data[fe_lst])
-
-            self.data_close = self._data_to_3d_tensor(self.data[['date', 'symbol', 'close']].copy())
-            self.data_close = self.data_close[:, :, 0]
+            self.fe_data = self._data_to_3d_tensor(self.data[feature_columns])
+            self.close_prices = self._data_to_3d_tensor(self.data[['date', 'symbol', 'close']].copy())[:, :, 0]
         elif self.obs_type == 'pd':
             self.fe_data = self.data.copy()
-            self.data_close = self._data_to_3d_tensor(self.data[['date', 'symbol', 'close']].copy())
-            self.data_close = self.data_close[:, :, 0]
+            self.close_prices = self._data_to_3d_tensor(self.data[['date', 'symbol', 'close']].copy())[:, :, 0]
         else:
             raise ValueError("Invalid observation type. Use 'pd' or 'np'.")
-            
 
-        # Unique symbols and dates in the dataset
+        # Уникальные даты и символы
         self.all_dates = np.array(self.data.date.unique())
-        self.total_dates = len(self.data.date.unique())
+        self.total_dates = len(self.all_dates)
 
         self.symbols = list(self.data.symbol.unique())
-        self.stock_dimension = len(self.symbols)
+        self.num_assets = len(self.symbols)
 
         if self.window > self.total_dates:
             raise ValueError("Window size is larger than the number of dates.")
 
-        # Observation and action spaces
+        # Определение пространства наблюдений и действий
         if self.obs_type == 'np':
             if self.window > 1:
-                self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(self.window, self.fe_data.shape[1], self.fe_data.shape[2]), dtype=np.float32)
+                self.observation_space = spaces.Box(low=-np.inf, high=np.inf,
+                                                    shape=(self.window, self.fe_data.shape[1], self.fe_data.shape[2]),
+                                                    dtype=np.float32)
             else:
-                self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(self.fe_data.shape[1], self.fe_data.shape[2]))
+                self.observation_space = spaces.Box(low=-np.inf, high=np.inf,
+                                                    shape=(self.fe_data.shape[1], self.fe_data.shape[2]))
         elif self.obs_type == 'pd':
             if self.window > 1:
-                self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(self.window, len(self.features_list), self.stock_dimension),)
+                self.observation_space = spaces.Box(low=-np.inf, high=np.inf,
+                                                    shape=(self.window, len(self.features_list), self.num_assets))
             else:
-                self.observation_space = spaces.Box(low=-np.inf, high=np.inf, shape=(len(self.features_list), self.stock_dimension),)
-
+                self.observation_space = spaces.Box(low=-np.inf, high=np.inf,
+                                                    shape=(len(self.features_list), self.num_assets))
 
-        # The agent can choose to buy from 0% to 100% of any stock or future contracts available in the portfolio
-        self.action_space = spaces.Box(low=-1, high=1, shape=(self.stock_dimension,)) #STOCKS + USDT
+        self.action_space = spaces.Box(low=-1, high=1, shape=(self.num_assets,))
 
-        # seed for reproducibility
-        _ = self.seed(self.random_seed)
+        # Установка seed для воспроизводимости
+        self.seed(self.random_seed)
 
-        # initialize memory structures
+        # Инициализация структур памяти
         self.reset()
 
     def _check_dates(self, df: pd.DataFrame):
         """Check that the number of dates for each symbol matches.
         
         Args:
-            df (DataFrame): Input data.
+            df (pd.DataFrame): Input data.
             
-            Raises:
-                ValueError: If the number of dates for each symbol does not match.
+        Raises:
+            ValueError: If the number of dates for each symbol does not match.
         """
         symbol_counts = df.groupby('symbol')['date'].count()
         if symbol_counts.std() != 0:
             raise ValueError('The number of dates for each symbol does not match.')
 
     def _data_to_3d_tensor(self, data: pd.DataFrame) -> np.array:
         """
         Convert input data to 3D tensor.
 
         Args:
-            data (DataFrame): Input data.
+            data (pd.DataFrame): Input data.
 
         Returns:
             np.array: Transformed 3D tensor.
         """
         df = data.sort_values(['date', 'symbol']).copy()
         df = df.set_index(['date', 'symbol'])
         dates = df.index.get_level_values('date').unique()
         data_3d = np.array([df.loc[date].values for date in dates])
         return data_3d
-    
+
     def reset(self) -> np.array:
-        """Reset the state of the environment to an initial state.
+        """
+        Reset the state of the environment to an initial state.
 
         Returns:
             np.array: The initial state.
-
         """
-        # Initialize memory structures
-        self.actions_memory = [np.zeros(self.stock_dimension),]
+        # Инициализация структур памяти
+        self.actions_memory = [np.zeros(self.num_assets),]
         self.total_commission = 0
         self.total_commission_memory = [0,]
-        self.balance = self.init_balance
-        self.balance_memory = [self.init_balance,]
+        self.balance = self.initial_balance
+        self.balance_memory = [self.initial_balance,]
         self.finish_portfolio_value = 0
         self.portfolio_value_memory = [0,]
         self.date_memory = [self.all_dates[0],]
-        self.portfolio_weights = np.zeros(self.stock_dimension)
+        self.portfolio_weights = np.zeros(self.num_assets)
         self.portfolio_weights_memory = [self.portfolio_weights,]
-
-        # Initialize an empty array to store the asset prices
-        self.asset_prices = np.zeros(self.stock_dimension)
+        self.asset_prices = np.zeros(self.num_assets)
         self.asset_prices_memory = [self.asset_prices,]
-        self.positions = np.zeros(self.stock_dimension)
-        self.positions_memory = [np.zeros(self.stock_dimension),]
+        self.positions = np.zeros(self.num_assets)
+        self.positions_memory = [np.zeros(self.num_assets),]
         self.total_profit_memory = [0,]
-        # Rewards received for each trading step i.e profit or loss
         self.reward_memory = [0,]
         self.trades = 0
-
-        # Initialize reward
         self.reward = 0
         self.episode = 0
-
-        # Reset counters and memory
         self.current_step = 0
         self.total_step_profit = 0
         self.done = False
 
-        # if self.mode_train and self.random_start_step:
-        #     # Randomly select a starting point for each episode
-        #     # This introduces some randomness in the data the agent sees in each episode, 
-        #     # helping the agent to explore different market conditions.
-        #     max_starting_point = self.total_dates - (self.reward_metric_window * 3)  # Reserve 500 timesteps for the episode
-        #     self.data_step = np.random.randint(self.window, max_starting_point)
-        # else:
-        self.data_step = self.window+1
-
+        # Начальная позиция в данных
+        self.data_step = self.window + 1
         self.current_date = self.all_dates[self.data_step]
         self.date_memory = [self.current_date,]
 
-        # get the first state
+        # Получение начального состояния
         state = self.get_state(self.data_step)
         return state
-    
+
     def get_state(self, data_step: int) -> np.array:
-        """Retrieve the current state of the environment.
+        """
+        Retrieve the current state of the environment.
 
         Args:
             data_step (int): The current step in the data.
 
         Returns:
             np.array: The current state.
-
         """
-        # Get the current window of data
         if self.obs_type == 'np':
             if self.window > 1:
-                obs = self.fe_data[(data_step-self.window + 1):data_step + 1]
+                obs = self.fe_data[(data_step - self.window + 1):data_step + 1]
             else:
                 obs = np.array(self.fe_data[data_step])
         elif self.obs_type == 'pd':
-            # slice windows df
-            obs = self.fe_data[((data_step-self.window + 1)*len(self.symbols)):(data_step + 1)*len(self.symbols)].copy()
-            #obs = obs.drop(['date', 'symbol'], axis=1)
-            #obs = obs.values
-
-        # Get the current date
+            obs = self.fe_data[((data_step - self.window + 1) * len(self.symbols)):(data_step + 1) * len(self.symbols)].copy()
         self.current_date = self.all_dates[data_step]
-
-        # Get the current asset prices
-        self.asset_prices = self.data_close[data_step]
+        self.asset_prices = self.close_prices[data_step]
         return obs
-    
+
     def seed(self, seed: int = 1) -> list:
-        """Set the random seed for the environment.
+        """
+        Set the random seed for the environment.
 
         Args:
             seed (int, optional): The random seed value.
 
         Returns:
             list: The random seed.
-
         """
         self.np_random, seed = gym.utils.seeding.np_random(seed)
         return [seed]
 
-    def get_sb_env(self, num_workers = 1) -> Tuple[DummyVecEnv, np.array]:
-        """Get Stable Baselines Environment.
-
-        Returns:
-            A tuple containing the DummyVecEnv and initial observation.
-        """
-        
-        if num_workers > 1:
-            e = SubprocVecEnv([lambda: self for i in range(num_workers)])
-        else:
-            e = DummyVecEnv([lambda: self])
-        obs = e.reset()
-        return e, obs
-    
     def render(self, mode: str = "human"):
-        """Render the environment.
+        """
+        Render the environment.
 
         Args:
             mode (str, optional): The mode for rendering.
-
         """
-        # simple rendering of the current state
         print(
-            f"Date: {self.date_memory[-1]}, Balance: {self.balance:.2f}, " \
-            f"Portfolio Value: {self.finish_portfolio_value:.2f}, " \
-            f"Profit: {self.total_step_profit:.2f}, " \
-            f"Trades: {self.trades}, " \
+            f"Date: {self.date_memory[-1]}, Balance: {self.balance:.2f}, "
+            f"Portfolio Value: {self.finish_portfolio_value:.2f}, "
+            f"Profit: {self.total_step_profit:.2f}, "
+            f"Trades: {self.trades}, "
             f"Total Commission: {self.total_commission:.5f}"
-            )
+        )
 
-    def _calculate_commission(self, balance, portfolio_weights, old_portfolio_weights, positions, asset_prices, buy_commission, sell_commission):
-        """Calculate commission for the trading.
+    def _calculate_commission(self, balance, new_weights, old_weights, positions, asset_prices, buy_commission_pct, sell_commission_pct):
+        """
+        Calculate commission for the trading.
 
         Args:
             balance: Current balance.
-            portfolio_weights: New portfolio weights.
-            old_portfolio_weights: Old portfolio weights.
+            new_weights: New portfolio weights.
+            old_weights: Old portfolio weights.
             positions: Current positions.
             asset_prices: Current asset prices.
-            buy_commission: Buy commission rate.
-            sell_commission: Sell commission rate.
+            buy_commission_pct: Buy commission rate.
+            sell_commission_pct: Sell commission rate.
 
         Returns:
-            Total commission cost.
+            float: Total commission cost.
         """
-
-        changes_in_quantity = (np.divide(portfolio_weights, old_portfolio_weights, out=np.zeros_like(portfolio_weights), where=old_portfolio_weights!=0) * positions) - positions
-        changes_in_quantity[old_portfolio_weights==0] = (balance*portfolio_weights/asset_prices)[old_portfolio_weights==0]
-
-
-        buy_cost = np.sum(np.maximum(changes_in_quantity*asset_prices, 0))
-        sell_cost = np.sum(np.abs(np.minimum(changes_in_quantity*asset_prices, 0)))
-        total_buy_commission = buy_cost * (buy_commission / 100)
-        total_sell_commission = sell_cost * (sell_commission / 100)
+        changes_in_quantity = (np.divide(new_weights, old_weights, out=np.zeros_like(new_weights), where=old_weights != 0) * positions) - positions
+        changes_in_quantity[old_weights == 0] = (balance * new_weights / asset_prices)[old_weights == 0]
+        buy_cost = np.sum(np.maximum(changes_in_quantity * asset_prices, 0))
+        sell_cost = np.sum(np.abs(np.minimum(changes_in_quantity * asset_prices, 0)))
+        total_buy_commission = buy_cost * (buy_commission_pct / 100)
+        total_sell_commission = sell_cost * (sell_commission_pct / 100)
         total_commission = total_buy_commission + total_sell_commission
-
         if np.isfinite(total_commission):
             total_commission = round(total_commission, 10)
-
         if np.isnan(total_commission):
             total_commission = 0
         return total_commission
-    
-    def _norm_portfolio_weights(self, actions):
-        """Normalize portfolio weights.
+
+    def _normalize_weights(self, actions):
+        """
+        Normalize portfolio weights.
 
         Args:
             actions: Actions representing raw portfolio weights.
 
         Returns:
-            Normalized portfolio weights.
+            np.array: Normalized portfolio weights.
         """
-        # Calculating the portfolio weights based on actions
-        total_action = np.sum(np.abs(actions)) 
+        total_action = np.sum(np.abs(actions))
         if total_action > 1:
-            portfolio_weights = actions / total_action if total_action != 0 else np.zeros(self.stock_dimension)
+            normalized_weights = actions / total_action if total_action != 0 else np.zeros(self.num_assets)
         else:
-            portfolio_weights = actions
-        portfolio_weights = np.clip(portfolio_weights, -1, 1)
-        portfolio_weights = np.round(portfolio_weights, 3)
-        return portfolio_weights
-    
+            normalized_weights = actions
+        normalized_weights = np.clip(normalized_weights, -1, 1)
+        normalized_weights = np.round(normalized_weights, 4)
+        return normalized_weights
+
     def _get_reward(self):
-        """Calculate the reward based on the selected reward type."""
+        """
+        Calculate the reward based on the selected reward type.
+        """
         if self.reward_type in ["sharpe", "sortino", 'mean_return', 'alpha_penalize']:
             if self.current_step < self.reward_metric_window or len(self.balance_memory) < self.reward_metric_window:
                 self.reward = 0
             else:
-                # Setup
-                self.reward_settings['balances'] = self.balance_memory[(self.current_step - self.reward_metric_window) -1: self.current_step]
+                self.reward_settings['balances'] = self.balance_memory[(self.current_step - self.reward_metric_window) - 1: self.current_step]
                 self.reward_settings['returns'] = np.diff(self.reward_settings['balances']) / self.reward_settings['balances'][:-1]
                 self.reward_settings['risk_free_rate'] = self.risk_free_rate
                 self.reward_settings['total_commission'] = self.total_commission
-                
-                # Calculate metrics
                 self.reward = all_rewards_func[self.reward_type](**self.reward_settings)
-        
         else:
             self.reward_settings['asset_prices'] = self.asset_prices
             self.reward_settings['old_asset_prices'] = self.old_asset_prices
             self.reward_settings['portfolio_weights'] = self.portfolio_weights
             self.reward_settings['total_step_profit'] = self.total_step_profit
-
-            # Calculate metrics
             self.reward = all_rewards_func[self.reward_type](**self.reward_settings)
-
-        # Handling edge cases to avoid NaN or infinite rewards
         if not np.isfinite(self.reward):
             self.reward = 0
-    
-    def _calc_positions(self, portfolio_weights: np.array, balance: float, asset_prices: np.array):
-        """Calculate positions based on portfolio weights and current balance.
+
+    def _calculate_positions(self, weights: np.array, balance: float, prices: np.array) -> np.array:
+        """
+        Calculate positions based on portfolio weights and current balance.
 
         Args:
-            portfolio_weights: Portfolio weights.
-            balance: Current balance.
-            asset_prices: Current asset prices.
+            weights (np.array): Portfolio weights.
+            balance (float): Current balance.
+            prices (np.array): Current asset prices.
 
         Returns:
-            Positions.
+            np.array: Positions.
         """
-        positions = (portfolio_weights * balance) / asset_prices
+        positions = (weights * balance) / prices
         return positions
-    
-    def _calc_portfolio_value(self, positions: np.array, asset_prices: np.array):
-        """Calculate portfolio value based on positions and current asset prices.
+
+    def _calculate_portfolio_value(self, positions: np.array, prices: np.array) -> float:
+        """
+        Calculate portfolio value based on positions and current asset prices.
 
         Args:
-            positions: Current positions.
-            asset_prices: Current asset prices.
+            positions (np.array): Current positions.
+            prices (np.array): Current asset prices.
 
         Returns:
-            Portfolio value.
+            float: Portfolio value.
         """
-        portfolio_value = np.round(np.sum(np.abs(positions) * asset_prices), 3)
+        portfolio_value = np.round(np.sum(np.abs(positions) * prices), 4)
         return portfolio_value
-    
-    def _calc_portfolio_weights(self, balance: int, positions: np.array, asset_prices: np.array):
-        """Calculate portfolio weights based on current positions and asset prices."""
-        asset_values = positions * asset_prices #+ self.portfolio_weights[-1]*self.balance  # Value of each asset
-        total_portfolio_value = np.sum(np.abs(asset_values))  # Total portfolio value
-        allocate_cash_pcr = (balance - total_portfolio_value)/balance  # Value to allocate to cash
-        
-        portfolio_weights_full = np.zeros(len(asset_prices))
 
-        if total_portfolio_value > 0: # if there are assets in the portfolio
-            portfolio_weights = (asset_values / total_portfolio_value)*(1-allocate_cash_pcr)  # Portfolio weights
-            #portfolio_weights_full[:len(asset_prices)] =  portfolio_weights
-            portfolio_weights_full =  portfolio_weights
+    def _calculate_weights(self, balance: float, positions: np.array, prices: np.array) -> np.array:
+        """
+        Calculate portfolio weights based on current positions and asset prices.
 
-        #portfolio_weights_full[-1] = allocate_cash_pcr
+        Args:
+            balance (float): Current balance.
+            positions (np.array): Current positions.
+            prices (np.array): Current asset prices.
 
-        return np.round(portfolio_weights_full, 2)
+        Returns:
+            np.array: Portfolio weights.
+        """
+        asset_values = positions * prices
+        total_portfolio_value = np.sum(np.abs(asset_values))
+        cash_allocation = (balance - total_portfolio_value) / balance
+        full_weights = np.zeros(len(prices))
+        if total_portfolio_value > 0:
+            weights = (asset_values / total_portfolio_value) * (1 - cash_allocation)
+            full_weights = weights
+        return np.round(full_weights, 4)
 
-    def _step_profit(self, asset_prices: np.array, old_asset_prices: np.array, positions: np.array):
-        """Calculate the total profit or loss from the current step.
+    def _calculate_step_profit(self, prices: np.array, old_prices: np.array, positions: np.array) -> float:
+        """
+        Calculate the total profit or loss from the current step.
 
         Args:
-            asset_prices: Current asset prices.
-            old_asset_prices: Asset prices from the previous step.
-            positions: Current positions.
+            prices (np.array): Current asset prices.
+            old_prices (np.array): Asset prices from the previous step.
+            positions (np.array): Current positions.
 
         Returns:
-            Total profit
+            float: Total profit.
         """
-        price_change = asset_prices - old_asset_prices
-
-        # Calculate the profit or loss for long and short positions
+        price_change = prices - old_prices
         long_profit_loss = np.sum(np.where(positions > 0, positions * price_change, 0))
         short_profit_loss = np.sum(np.where(positions < 0, positions * -price_change, 0))
-
         step_profit = (long_profit_loss - short_profit_loss)
         return step_profit
 
-    def _update_memory_structures(self):
-        # Update portfolio_weights
-        self.portfolio_value = self._calc_portfolio_value(self.positions, self.asset_prices)
-        self.portfolio_weights = self._calc_portfolio_weights(self.balance, self.positions, self.asset_prices)
-
-        # Update the memory structures
-        #self.actions_memory.append(actions)
+    def _update_memory(self):
+        """
+        Update the memory structures with the latest values.
+        """
+        self.portfolio_value = self._calculate_portfolio_value(self.positions, self.asset_prices)
+        self.portfolio_weights = self._calculate_weights(self.balance, self.positions, self.asset_prices)
         self.portfolio_value_memory.append(self.portfolio_value)
         self.total_profit_memory.append(self.total_step_profit)
         self.portfolio_weights_memory.append(self.portfolio_weights.copy())
         self.asset_prices_memory.append(self.asset_prices.copy())
         self.reward_memory.append(self.reward)
         self.balance_memory.append(self.balance)
         self.total_commission_memory.append(self.total_commission)
         self.date_memory.append(self.current_date)
 
     def step(self, actions: np.array) -> Tuple[np.array, float, bool, Dict[str, Any]]:
-        """Execute one time step within the environment.
+        """
+        Execute one time step within the environment.
 
         Args:
-            actions: An array of actions to execute in the environment.
+            actions (np.array): An array of actions to execute in the environment.
 
         Returns:
-            A tuple containing the next state, reward, done, and info.
+            Tuple[np.array, float, bool, Dict[str, Any]]: A tuple containing the next state, reward, done, and info.
         """
-        ####################################### Chenge positions #######################################
         self.actions_memory.append(actions.copy())
-        
         self.old_portfolio_weights = self.portfolio_weights.copy()
-        self.old_asset_prices = self.asset_prices.copy() 
+        self.old_asset_prices = self.asset_prices.copy()
+        self.new_portfolio_weights = self._normalize_weights(actions)
         
-        self.new_portfolio_weights = self._norm_portfolio_weights(actions)
-        # Commission
-        self.total_commission = self._calculate_commission(
-            self.balance,
-            self.new_portfolio_weights, #[:-1], #the last is usdt
-            self.old_portfolio_weights, #[:-1],
-            self.positions,
-            self.asset_prices,
-            self.buy_commission,
-            self.sell_commission,
+        # Calculate the change in weights directly
+        weight_change = np.abs(self.old_portfolio_weights - self.new_portfolio_weights)
+
+        if np.any(weight_change > self.rebalance_threshold):
+            # If change exceeds the threshold, apply commissions and update positions
+            self.total_commission = self._calculate_commission(
+                balance=self.balance,
+                new_weights=self.new_portfolio_weights,
+                old_weights=self.old_portfolio_weights,
+                positions=self.positions,
+                asset_prices=self.asset_prices,
+                buy_commission_pct=self.buy_commission_pct,
+                sell_commission_pct=self.sell_commission_pct,
             )
-        # Update the balance based on the commission
-        
-        self.balance -= self.total_commission
-        # Trades
-        if self.total_commission > 0:
-            self.trades+=1
-
-        ## Calculate the updated positions after accounting for commissions
-        self.positions = self._calc_positions(self.new_portfolio_weights, self.balance, self.asset_prices)
-        ####################################### Get new prices ##########################################
-        # Move to the next time step
+            self.balance -= self.total_commission
+            #if self.total_commission > 0:
+            self.trades += 1
+
+            self.positions = self._calculate_positions(self.new_portfolio_weights, self.balance, self.asset_prices)
+            self.portfolio_weights = self.new_portfolio_weights.copy()
+            self.total_commission_memory.append(self.total_commission)
+        else:
+            #self.total_commission_memory.append(0)
+            self.total_commission = 0
+            
+            #self.positions = self._calculate_positions(self.new_portfolio_weights, self.balance, self.asset_prices)
+
         self.current_step += 1
         self.data_step += 1
 
-        # Get the new state
         state = self.get_state(self.data_step)
-        
-        # total profit from the current step
-        self.step_profit = self._step_profit(self.asset_prices, self.old_asset_prices, self.positions)
+        self.step_profit = self._calculate_step_profit(self.asset_prices, self.old_asset_prices, self.positions)
         self.total_step_profit = self.step_profit - self.total_commission
-        # Update the balance based on the reward
         self.balance += self.step_profit
-
-        # Calculate reward
         self._get_reward()
 
-        # Check if the episode is done
         if self.data_step == self.total_dates - 1 or self.balance <= 0:
             self.done = True
 
-        ####################################### Save data ##############################################
-        # Update the memory structures
-        #self.portfolio_weights = self.new_portfolio_weights
-        self._update_memory_structures()
-
+        self._update_memory()
         info = {}
         return state, self.reward, self.done, info
 
-    def save_balance_memory(self):
-        df_memory = pd.DataFrame(
-            {
-                "date": self.date_memory, 
-                "account_value": self.balance_memory,
-            }
-            )
+    def save_balance_memory(self) -> pd.DataFrame:
+        """
+        Save the balance memory to a DataFrame.
+
+        Returns:
+            pd.DataFrame: DataFrame containing the balance memory.
+        """
+        df_memory = pd.DataFrame({"date": self.date_memory, "account_value": self.balance_memory})
         return df_memory
 
-    def save_memory(self):
+    def save_memory(self) -> pd.DataFrame:
+        """
+        Save the memory to a DataFrame.
+
+        Returns:
+            pd.DataFrame: DataFrame containing the memory.
+        """
         df_memory = pd.DataFrame(
             {
-                "date": self.date_memory, 
+                "date": self.date_memory,
                 "account_value": self.balance_memory,
                 "actions": self.actions_memory,
                 "portfolio_weights": self.portfolio_weights_memory,
                 "portfolio_value": self.portfolio_value_memory,
                 "reward": self.reward_memory,
             }
         )
         return df_memory
 
-    def save_action_memory(self, action_list=None):
-        if self.stock_dimension > 1:
-            # date and close price length must match actions length
+    def save_action_memory(self, action_list=None) -> pd.DataFrame:
+        """
+        Save the action memory to a DataFrame.
+
+        Args:
+            action_list (list, optional): List of actions.
+
+        Returns:
+            pd.DataFrame: DataFrame containing the action memory.
+        """
+        if self.num_assets > 1:
             date_list = self.date_memory
             df_date = pd.DataFrame(date_list)
             df_date.columns = ["date"]
 
             if action_list is None:
                 action_list = self.actions_memory
-            else:
-                action_list = action_list
-            
+
             df_actions = pd.DataFrame(action_list)
             df_actions.columns = self.symbols
             df_actions.index = df_date.date
         else:
             date_list = self.date_memory[:-1]
             action_list = self.actions_memory
             df_actions = pd.DataFrame({"date": date_list, "actions": action_list})
             
-        return df_actions
+        return df_actions
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tradegym-25.1.5/PKG-INFO` & `tradegym-25.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: tradegym
-Version: 25.1.5
+Version: 25.2.2
 Summary: trading gym
 License: MIT
 Author: Alex-Lekov
 Author-email: 61644712+Alex-Lekov@users.noreply.github.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: empyrical (>=0.5.5,<0.6.0)
+Requires-Dist: filelock (>=3.14.0,<4.0.0)
 Requires-Dist: gym (>=0.26.2,<0.27.0)
 Requires-Dist: ipykernel (>=6.25.1,<7.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: plotly (>=5.16.1,<6.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: quantstats (>=0.0.62,<0.0.63)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: shimmy (>=1.2.1,<2.0.0)
-Requires-Dist: stable-baselines3 (>=2.1.0,<3.0.0)
-Requires-Dist: torch (>=2.0.0,!=2.0.1)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Requires-Dist: vectorbt (>=0.26.1,<0.27.0)
 Description-Content-Type: text/markdown
 
 # AlphaProfit Trading Gym Env
 
 **Trading Gym Env** - это "тренажер", где можно имитировать торговлю активами и обучать торговых роботов с помощью специальных методов RL. Он был разработан для быстрой и настраиваемой реализации алгоритмов RL для торговли.
 
 **Reinforcement Learning** (RL) - это одна из областей машинного обучения, где агент учится принимать решения, выполняя действия в некоторой среде, чтобы максимизировать некоторый кумулятивный выигрыш.
```

