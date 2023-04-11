# Comparing `tmp/gym-trading-env-0.1.2.tar.gz` & `tmp/gym-trading-env-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.2.tar", last modified: Mon Apr 10 19:40:21 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.3.tar", last modified: Tue Apr 11 09:32:00 2023, max compression
```

## Comparing `gym-trading-env-0.1.2.tar` & `gym-trading-env-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.403118 gym-trading-env-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    14061 2023-04-10 19:40:21.401123 gym-trading-env-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    12199 2023-04-10 19:39:58.000000 gym-trading-env-0.1.2/README.md
--rw-rw-rw-   0        0        0      848 2023-04-10 19:19:49.000000 gym-trading-env-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 19:40:21.404119 gym-trading-env-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.302708 gym-trading-env-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.337043 gym-trading-env-0.1.2/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.2/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     3855 2023-04-10 19:15:33.000000 gym-trading-env-0.1.2/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.2/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2471 2023-04-05 13:55:23.000000 gym-trading-env-0.1.2/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.399128 gym-trading-env-0.1.2/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.2/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-10 19:40:21.375193 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14061 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 19:40:21.000000 gym-trading-env-0.1.2/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.376202 gym-trading-env-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    14011 2023-04-11 09:32:00.374198 gym-trading-env-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.3/README.md
+-rw-rw-rw-   0        0        0      854 2023-04-11 09:28:09.000000 gym-trading-env-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:32:00.377196 gym-trading-env-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.290425 gym-trading-env-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.318349 gym-trading-env-0.1.3/src/gym_trading_env/
+-rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.3/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     3855 2023-04-10 19:15:33.000000 gym-trading-env-0.1.3/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.3/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.3/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.372205 gym-trading-env-0.1.3/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.357280 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14011 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.2/LICENSE.txt` & `gym-trading-env-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/PKG-INFO` & `gym-trading-env-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,16 +65,17 @@
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
 
 But if you want to use a really basic environment, you can use only 2 positions : ```1``` and ```0``` which is more of less equivalent to **BUY ALL** and **SELL ALL** actions.
 
+### Complex positions
 
-Plus, this environment supports more complex positions such as:
+This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
 **1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
@@ -116,41 +117,28 @@
 **(Optional)3 - Create your own reward function**. Use the history object described below to create your own ! For example : 
 ```python
 import numpy as np
 def reward_function(history):
     return np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2]) #log (p_t / p_t-1 )
 ```
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
-- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
-- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
-- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
+>- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
+>- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
+>- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step``` : Step = t.
-- ```date``` : Date at step t, datetime.
-- ```reward``` : Reward at step t.
-- ```position_index``` : Index of the position at step t amoung your position argument.
-- ```position``` : Portfolio position at step t.
-- ```portfolio_valuation```: Global valuation of the portfolio.
-
-    *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close``` : Close price.
-- ```data_open``` : Open price.
-- ```data_high``` : High price.
-
-    *......*
-
-    *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
-- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
-- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
-- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
+>- ```step``` : Step = t.
+>- ```date``` : Date at step t, datetime.
+>- ```reward``` : Reward at step t.
+>- ```position_index``` : Index of the position at step t amoung your position argument.
+v- ```position``` : Portfolio position at step t.
+>- ```portfolio_valuation```: Global valuation of the portfolio.
+>- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
+>- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
 ```python
 env = TradingEnv(
         name= "BTCUSD",
@@ -161,46 +149,46 @@
         trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
         borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
         reward_function = reward_function,
         portfolio_initial_value = 1000, # here, in USDT
     )
 ```
 Parameters :
-- ```name``` (required) : Name of your asset / symbol
-- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
-- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
-- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
-- ```initial_position``` (optional, default : 0). Initial position of the portfolio
-- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
-- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
-- ```reward_function``` (Optional, default : the reward function used above). Reward function.
-- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
+>- ```name``` (required) : Name of your asset / symbol
+>- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
+>- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
+>- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
+>- ```initial_position``` (optional, default : 0). Initial position of the portfolio
+>- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
+>- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
+>- ```reward_function``` (Optional, default : the reward function used above). Reward function.
+>- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
 
 **5 - Run the environment**
 ```python
 truncated, done = False, False
 observation, info = env.reset()
 while not truncated and not done:
     action = env.action_space.sample()
     observation, reward, done, truncated, info = env.step(action)
 ```
-- ```observation``` : Returns a dict with items :
-    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
-    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
-- ```reward``` : The step reward following the action taken.
-- ```done```: Always False.
-- ```truncated``` : is true if the end of the DataFrame is reached.
-- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
+>- ```observation``` : Returns a dict with items :
+>    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
+>    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
+>- ```reward``` : The step reward following the action taken.
+>- ```done```: Always False.
+>- ```truncated``` : is true if the end of the DataFrame is reached.
+>- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
 
 
-**6 - Render** performed with Dash Plotly (local app).
+### 6 - Render performed with Flask (local app).
 
-<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.PNG?raw=true" height = "800"/>
+<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.gif?raw=true" width = "800"/>
 
-For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
+For the render not to perturb the training, it needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
@@ -208,14 +196,15 @@
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
+#### Custom render
 
 You can add **metrics** and plot **lines** with :
 ```python
 renderer = Renderer(render_logs_dir="render_logs")
 
 # Add Custom Lines (Simple Moving Average)
 renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
@@ -235,23 +224,23 @@
 renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_line``` takes arguments :
-- ```name``` (*required*): The name of the scatter
-- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
-
-
-```.add_metric``` takes arguments :
-- ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
+>```.add_line``` takes arguments :
+>- ```name``` (*required*): The name of the scatter
+>- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+>- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
+>
+>
+>```.add_metric``` takes arguments :
+>- ```name``` : The name of the metric
+>- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

### Comparing `gym-trading-env-0.1.2/README.md` & `gym-trading-env-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
 
 But if you want to use a really basic environment, you can use only 2 positions : ```1``` and ```0``` which is more of less equivalent to **BUY ALL** and **SELL ALL** actions.
 
+### Complex positions
 
-Plus, this environment supports more complex positions such as:
+This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
 **1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
@@ -81,41 +82,28 @@
 **(Optional)3 - Create your own reward function**. Use the history object described below to create your own ! For example : 
 ```python
 import numpy as np
 def reward_function(history):
     return np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2]) #log (p_t / p_t-1 )
 ```
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
-- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
-- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
-- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
+>- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
+>- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
+>- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step``` : Step = t.
-- ```date``` : Date at step t, datetime.
-- ```reward``` : Reward at step t.
-- ```position_index``` : Index of the position at step t amoung your position argument.
-- ```position``` : Portfolio position at step t.
-- ```portfolio_valuation```: Global valuation of the portfolio.
-
-    *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close``` : Close price.
-- ```data_open``` : Open price.
-- ```data_high``` : High price.
-
-    *......*
-
-    *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
-- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
-- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
-- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
+>- ```step``` : Step = t.
+>- ```date``` : Date at step t, datetime.
+>- ```reward``` : Reward at step t.
+>- ```position_index``` : Index of the position at step t amoung your position argument.
+v- ```position``` : Portfolio position at step t.
+>- ```portfolio_valuation```: Global valuation of the portfolio.
+>- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
+>- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
 ```python
 env = TradingEnv(
         name= "BTCUSD",
@@ -126,46 +114,46 @@
         trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
         borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
         reward_function = reward_function,
         portfolio_initial_value = 1000, # here, in USDT
     )
 ```
 Parameters :
-- ```name``` (required) : Name of your asset / symbol
-- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
-- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
-- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
-- ```initial_position``` (optional, default : 0). Initial position of the portfolio
-- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
-- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
-- ```reward_function``` (Optional, default : the reward function used above). Reward function.
-- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
+>- ```name``` (required) : Name of your asset / symbol
+>- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
+>- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
+>- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
+>- ```initial_position``` (optional, default : 0). Initial position of the portfolio
+>- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
+>- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
+>- ```reward_function``` (Optional, default : the reward function used above). Reward function.
+>- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
 
 **5 - Run the environment**
 ```python
 truncated, done = False, False
 observation, info = env.reset()
 while not truncated and not done:
     action = env.action_space.sample()
     observation, reward, done, truncated, info = env.step(action)
 ```
-- ```observation``` : Returns a dict with items :
-    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
-    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
-- ```reward``` : The step reward following the action taken.
-- ```done```: Always False.
-- ```truncated``` : is true if the end of the DataFrame is reached.
-- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
+>- ```observation``` : Returns a dict with items :
+>    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
+>    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
+>- ```reward``` : The step reward following the action taken.
+>- ```done```: Always False.
+>- ```truncated``` : is true if the end of the DataFrame is reached.
+>- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
 
 
-**6 - Render** performed with Dash Plotly (local app).
+### 6 - Render performed with Flask (local app).
 
-<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.PNG?raw=true" height = "800"/>
+<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.gif?raw=true" width = "800"/>
 
-For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
+For the render not to perturb the training, it needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
@@ -173,14 +161,15 @@
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
+#### Custom render
 
 You can add **metrics** and plot **lines** with :
 ```python
 renderer = Renderer(render_logs_dir="render_logs")
 
 # Add Custom Lines (Simple Moving Average)
 renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
@@ -200,23 +189,23 @@
 renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_line``` takes arguments :
-- ```name``` (*required*): The name of the scatter
-- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
-
-
-```.add_metric``` takes arguments :
-- ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
+>```.add_line``` takes arguments :
+>- ```name``` (*required*): The name of the scatter
+>- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+>- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
+>
+>
+>```.add_metric``` takes arguments :
+>- ```name``` : The name of the metric
+>- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

### Comparing `gym-trading-env-0.1.2/pyproject.toml` & `gym-trading-env-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.2"
+version = "0.1.3"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gym>=0.26.2", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt>=3.0.59", "numpy>=1.24.2"]
+dependencies = ["pandas>=1.5.3", "numpy>=1.23.1", "gymnasium>=0.28.1", "flask>=2.2.3", "pyecharts>=2.0.2", "ccxt>=3.0.59", "numpy>=1.24.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementPerroud/Gym-Trading-Env"
 "Bug Tracker" = "https://github.com/ClementPerroud/Gym-Trading-Env/issues"
```

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.3/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.3/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.3/src/gym_trading_env/renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import glob
 import pandas as pd
 
 
 class Renderer():
     def __init__(self, render_logs_dir):
         self.app = Flask(__name__, static_folder="./templates/")
+        self.app.debug = True
         self.app.config["EXPLAIN_TEMPLATE_LOADING"] = True
         self.df = None
         self.render_logs_dir = render_logs_dir
         self.metrics = [
             {
                 "name": "Market Return",
                 "function" : lambda df : f"{(df['close'].iloc[-1] / df['close'].iloc[0] - 1)*100:0.2f}%",
```

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.3/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.3/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.3/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.3/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,16 +65,17 @@
 ....
 
 
 In fact, it is way simpler for a RL-agent to work with positions. This way, it can easily make complex operation with a simple action space.
 
 But if you want to use a really basic environment, you can use only 2 positions : ```1``` and ```0``` which is more of less equivalent to **BUY ALL** and **SELL ALL** actions.
 
+### Complex positions
 
-Plus, this environment supports more complex positions such as:
+This environment supports more complex positions such as:
 - ```-1``` : Bet 100% of the portfolio value on the decline of asset Y (=SHORT). To perform this action, the environment borrows 100% of the portfolio valuation as stock Y to an imaginary person, and immediately sells it. When the agent closes this position, the environment buys the owed amount of stock Y and repays the imaginary person with it. If the price has fallen during the operation, we buy cheaper than we sold what we need to repay : the difference is our gain. The imaginary person is paid a small rent (parameter : ```borrow_interest_rate```)
 - ```+2``` : Bet 100% of the portfolio value of the rise of asset Y. We use the same mechanism explained above, but we borrow currency and buy stock Y.
 - ```-10``` ? : We can BUT ...  We need to borrow 1000% of the portfolio valuation as asset Y. You need to understand that such a "leverage" is very risky. As if the stock price rise by 10%, you need to repay the original 1000% of your portfolio valuation at 1100% (1000%*1.10) of your current portfolio valuation. Well, 100% (1100% - 1000%) of your portfolio is used to repay your debt. **GAME OVER, you have 0$ left**. The leverage is very useful but also risky, as it increases your **gains** AND your **losses**. Always keep in mind that you can lose everything.
 
 ### How to use ?
 
 **1 - Import and clean your data**. They need to be ordered by ascending date. Index must be a date. Your DataFrame needs to contain a close price labelled ```close``` to run. If you want to render your results, your DataFrame needs to contain open, high, low, volume features respectively labelled ```open```, ```high```, ```low```, ```volume```.
@@ -116,41 +117,28 @@
 **(Optional)3 - Create your own reward function**. Use the history object described below to create your own ! For example : 
 ```python
 import numpy as np
 def reward_function(history):
     return np.log(history["portfolio_valuation", -1] / history["portfolio_valuation", -2]) #log (p_t / p_t-1 )
 ```
 The history object is similar to a DataFrame. It uses timestep and/or columns to access its values. You can use it this way :
-- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
-- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
-- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
+>- ```history['column name', t]``` returns the a *scalar* value of the metrics 'column name' at time step t.
+>- ```history['column name']``` returns a *numpy array* with all the values from timestep 0 to current timestep.
+>- ```history[t]``` returns a *dictionnary* with of the metrics as keys with the associated values.
 
 
 Accessible columns of history object :
-- ```step``` : Step = t.
-- ```date``` : Date at step t, datetime.
-- ```reward``` : Reward at step t.
-- ```position_index``` : Index of the position at step t amoung your position argument.
-- ```position``` : Portfolio position at step t.
-- ```portfolio_valuation```: Global valuation of the portfolio.
-
-    *It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :*
-- ```data_close``` : Close price.
-- ```data_open``` : Open price.
-- ```data_high``` : High price.
-
-    *......*
-
-    *It stores the distribution of the portfolio :*
-- ```portfolio_distribution_asset``` : The amount of owned asset (stock).
-- ```portfolio_distribution_fiat``` : The amount of owned fiat currency.
-- ```portfolio_distribution_borrowed_asset``` : The amount of borrowed asset.
-- ```portfolio_distribution_borrowed_fiat``` : The amount of borrowed fiat currency.
-- ```portfolio_distribution_interest_asset``` : The total of cumalated interest generated by the borrowed asset.
-- ```portfolio_distribution_interest_fiat``` : The total of cumalated interest generated by the borrowed fiat currency.
+>- ```step``` : Step = t.
+>- ```date``` : Date at step t, datetime.
+>- ```reward``` : Reward at step t.
+>- ```position_index``` : Index of the position at step t amoung your position argument.
+v- ```position``` : Portfolio position at step t.
+>- ```portfolio_valuation```: Global valuation of the portfolio.
+>- It gathers every data (not used as features) from your DataFrame and labels them with 'data_{column}'. For example :```data_close```, ```data_open```,  ```data_high```....
+>- It stores the distribution of the portfolio : ```portfolio_distribution_asset``` the amount of owned asset (stock), ```portfolio_distribution_fiat``` the amount of owned fiat currency, ```portfolio_distribution_borrowed_asset``` amount of borrowed asset, ```portfolio_distribution_borrowed_fiat``` the amount of borrowed fiat currency, ```portfolio_distribution_interest_asset``` the total of cumalated interest generated by the borrowed asset, ```portfolio_distribution_interest_fiat``` the total of cumalated interest generated by the borrowed fiat currency.
 
 
 **4 - Initiate the environment**
 
 ```python
 env = TradingEnv(
         name= "BTCUSD",
@@ -161,46 +149,46 @@
         trading_fees = 0.01/100, # 0.01% per stock buy / sell (Binance fees)
         borrow_interest_rate= 0.0003/100, # 0.0003% per timestep (= 1h here)
         reward_function = reward_function,
         portfolio_initial_value = 1000, # here, in USDT
     )
 ```
 Parameters :
-- ```name``` (required) : Name of your asset / symbol
-- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
-- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
-- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
-- ```initial_position``` (optional, default : 0). Initial position of the portfolio
-- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
-- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
-- ```reward_function``` (Optional, default : the reward function used above). Reward function.
-- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
+>- ```name``` (required) : Name of your asset / symbol
+>- ```df``` (required) : DataFrame containing technical indicators ```open```, ```high```, ```low```, ```close```, ```volume```, and the features you want to be returned as observations (containing ```feature``` in their column names).
+>- ```windows```(optional, default : None), If None, observation at t are the features at step t  (classic mode). If windows = i (int),  observation at t are the features from steps [t-i+1 :  t] (useful for reccurent models)
+>- ```positions``` (optional, default : [0, 1]). Positions that the agent can choose (Explained in "Actions space : positions")
+>- ```initial_position``` (optional, default : 0). Initial position of the portfolio
+>- ```trading_fees``` (optional, default : 0). Trading fee for buy and sell.
+>- ```borrow_interest_rate``` (optional, default : 0). Borrow interest rate PER STEP.
+>- ```reward_function``` (Optional, default : the reward function used above). Reward function.
+>- ```portfolio_initial_value``` (optional, default : 1000). Initial value of the portfolio (in FIAT currency)
 
 **5 - Run the environment**
 ```python
 truncated, done = False, False
 observation, info = env.reset()
 while not truncated and not done:
     action = env.action_space.sample()
     observation, reward, done, truncated, info = env.step(action)
 ```
-- ```observation``` : Returns a dict with items :
-    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
-    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
-- ```reward``` : The step reward following the action taken.
-- ```done```: Always False.
-- ```truncated``` : is true if the end of the DataFrame is reached.
-- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
+>- ```observation``` : Returns a dict with items :
+>    - ```features``` : Contains the features created. If windows is None, it contains the features of the current step (shape = (n_features,)). If windows is i (int), it contains the features the last i steps (shape = (5, n_features)).
+>    - ```position``` : The last position of the environments. It can be useful to include this to the features, so the agent knows which position it is.
+>- ```reward``` : The step reward following the action taken.
+>- ```done```: Always False.
+>- ```truncated``` : is true if the end of the DataFrame is reached.
+>- ```info``` : Returns the last history step of the object "history" presented above (in "3 - Create your own reward function")
 
 
-**6 - Render** performed with Dash Plotly (local app).
+### 6 - Render performed with Flask (local app).
 
-<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.PNG?raw=true" height = "800"/>
+<img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render.gif?raw=true" width = "800"/>
 
-For the render not to perturb the training, the render needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
+For the render not to perturb the training, it needs to be performed in a separate python script. This way you have plenty of time to perform analysis on your results. 
 
 First, you need to save your results at the end of every episode you want to render with ```env.save_for_render(...)```. And decide which file you want your logs to be stored in with paramter ```dir```. For example :
 
 ```python
 ...
 # At the end of the episode you want to render
 env.save_for_render(dir = "render_logs")
@@ -208,14 +196,15 @@
 
 Then in the separated render script. You can import and initiate a render object, and run the render in a localhost web app :
 ```python
 from gym_trading_env.renderer import Renderer
 renderer = Renderer(render_logs_dir="render_logs")
 renderer.run()
 ```
+#### Custom render
 
 You can add **metrics** and plot **lines** with :
 ```python
 renderer = Renderer(render_logs_dir="render_logs")
 
 # Add Custom Lines (Simple Moving Average)
 renderer.add_line( name= "sma10", function= lambda df : df["close"].rolling(10).mean(), line_options ={"width" : 1, "color": "purple"})
@@ -235,23 +224,23 @@
 renderer.run()
 ```
 
 <img alt="Render example" src ="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/readme_images/render_customization.gif?raw=true" width = "800"/>
 
 
 
-```.add_line``` takes arguments :
-- ```name``` (*required*): The name of the scatter
-- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
-- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
-
-
-```.add_metric``` takes arguments :
-- ```name``` : The name of the metric
-- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
+>```.add_line``` takes arguments :
+>- ```name``` (*required*): The name of the scatter
+>- ```function``` (*required*): The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a Series, 1D-Array or list.
+>- ```line_options``` : Can contain a dict with keys ```color``` and ```width```
+>
+>
+>```.add_metric``` takes arguments :
+>- ```name``` : The name of the metric
+>- ```function``` : The function used to compute the line. The function must take an argument ```df``` which is a DateFrame and return a **string** !
 
 
 Enjoy :)
```

### Comparing `gym-trading-env-0.1.2/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.3/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

