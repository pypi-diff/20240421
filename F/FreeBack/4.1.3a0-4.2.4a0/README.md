# Comparing `tmp/FreeBack-4.1.3a0.tar.gz` & `tmp/FreeBack-4.2.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-4.1.3a0.tar", last modified: Sat Apr 20 07:21:42 2024, max compression
+gzip compressed data, was "FreeBack-4.2.4a0.tar", last modified: Sat Apr 20 19:05:28 2024, max compression
```

## Comparing `FreeBack-4.1.3a0.tar` & `FreeBack-4.2.4a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.154640 FreeBack-4.1.3a0/
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.153264 FreeBack-4.1.3a0/FreeBack/
--rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.1.3a0/FreeBack/__init__.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.1.3a0/FreeBack/alpha.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-11 18:28:29.000000 FreeBack-4.1.3a0/FreeBack/barbybar.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    12237 2024-04-20 06:25:35.000000 FreeBack-4.1.3a0/FreeBack/display.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.1.3a0/FreeBack/event.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    15856 2024-04-20 07:06:42.000000 FreeBack-4.1.3a0/FreeBack/my_pd.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    31210 2024-04-20 06:21:59.000000 FreeBack-4.1.3a0/FreeBack/post.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     3757 2024-04-20 02:54:09.000000 FreeBack-4.1.3a0/FreeBack/strat.py
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 07:21:42.154192 FreeBack-4.1.3a0/FreeBack.egg-info/
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/SOURCES.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/dependency_links.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/requires.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-20 07:21:42.000000 FreeBack-4.1.3a0/FreeBack.egg-info/top_level.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.1.3a0/LICENSE
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 07:21:42.154379 FreeBack-4.1.3a0/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.1.3a0/README.md
--rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-20 07:21:42.154685 FreeBack-4.1.3a0/setup.cfg
--rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-20 07:14:27.000000 FreeBack-4.1.3a0/setup.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 19:05:28.706712 FreeBack-4.2.4a0/
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 19:05:28.705259 FreeBack-4.2.4a0/FreeBack/
+-rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.2.4a0/FreeBack/__init__.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.2.4a0/FreeBack/alpha.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-11 18:28:29.000000 FreeBack-4.2.4a0/FreeBack/barbybar.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    12237 2024-04-20 06:25:35.000000 FreeBack-4.2.4a0/FreeBack/display.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.2.4a0/FreeBack/event.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15856 2024-04-20 07:06:42.000000 FreeBack-4.2.4a0/FreeBack/my_pd.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35412 2024-04-20 19:03:23.000000 FreeBack-4.2.4a0/FreeBack/post.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     3791 2024-04-20 07:58:39.000000 FreeBack-4.2.4a0/FreeBack/strat.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-20 19:05:28.706189 FreeBack-4.2.4a0/FreeBack.egg-info/
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 19:05:28.000000 FreeBack-4.2.4a0/FreeBack.egg-info/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-20 19:05:28.000000 FreeBack-4.2.4a0/FreeBack.egg-info/SOURCES.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-20 19:05:28.000000 FreeBack-4.2.4a0/FreeBack.egg-info/dependency_links.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-20 19:05:28.000000 FreeBack-4.2.4a0/FreeBack.egg-info/requires.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-20 19:05:28.000000 FreeBack-4.2.4a0/FreeBack.egg-info/top_level.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.2.4a0/LICENSE
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-20 19:05:28.706401 FreeBack-4.2.4a0/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.2.4a0/README.md
+-rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-20 19:05:28.706762 FreeBack-4.2.4a0/setup.cfg
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-20 19:04:22.000000 FreeBack-4.2.4a0/setup.py
```

### Comparing `FreeBack-4.1.3a0/FreeBack/alpha.py` & `FreeBack-4.2.4a0/FreeBack/alpha.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/FreeBack/barbybar.py` & `FreeBack-4.2.4a0/FreeBack/barbybar.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/FreeBack/display.py` & `FreeBack-4.2.4a0/FreeBack/display.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/FreeBack/event.py` & `FreeBack-4.2.4a0/FreeBack/event.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/FreeBack/my_pd.py` & `FreeBack-4.2.4a0/FreeBack/my_pd.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/FreeBack/post.py` & `FreeBack-4.2.4a0/FreeBack/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,86 +22,128 @@
         os.mkdir('output')
 
 ############################################################################################
 ####################### 处理收益率序列（简单收益率，非对数收益率） ###########################
 ############################################################################################
 class ReturnsPost():
     # benchmark dataframe 收益率序列
-    def __init__(self, returns, benchmark=0, stratname='策略'):
+    def __init__(self, returns, benchmark=0, stratname='策略', rf=0.03):
         self.stratname = stratname
-        self.returns = returns
-        self.net = (1+returns).cumprod()
+        self.returns = returns.fillna(0)
         # 无风险利率
-        self.rf = 0.03
-        # 基准
-        if benchmark==0:
-            benchmark = pd.DataFrame(index = returns.index)
+        self.rf = rf
+        # 基准指数
+        if type(benchmark)==int:
+            benchmark = pd.DataFrame(index = self.returns.index)
             benchmark['zero'] = 0
             self.benchmark = benchmark
-        self.benchmark = benchmark.loc[returns.index].fillna(0)
-        # 基准波动率
+        self.benchmark = benchmark.loc[self.returns.index].fillna(0)
         self.sigma_benchmark = np.exp(np.log(self.benchmark[\
             self.benchmark.columns[0]]+1).std())-1
-        # 净值曲线
+        self.cal_detail()
+    # 详细评价表
+    def cal_detail(self):
+        # 策略绝对表现
+        self.net = (1+self.returns).cumprod()
         self.lr = np.log(self.returns + 1)
-        # 超额收益 默认第一个benchmark
-        self.excess_lr = self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1)
-        self.returns.index.name = 'date'
-        # 评价指标
-        # 年化收益率（+1）
-        self.years = (returns.index[-1]-returns.index[0]).days/365  
-        self.return_total = (returns+1).prod()                             
-        self.return_annual = self.return_total**(1/self.years)-1    
-        excess_total = np.exp(self.excess_lr.sum())                  # 超额收益
-        self.excess_return_annual = excess_total**(1/self.years)-1
-        # 年化波动率 shrpe
-        self.sigma = np.exp(self.lr.std())-1
+        #self.returns.index.name = 'date'
+        self.years = (self.returns.index[-1]-self.returns.index[0]).days/365  
+        self.return_total = self.net[-1]/self.net[0]-1                    
+        self.return_annual = (self.return_total+1)**(1/self.years)-1   
+        self.sigma = np.exp(self.lr.std())-1 
         self.sharpe = (self.return_annual - self.rf)/(self.sigma*np.sqrt(250))
-        # 超额年化波动率 shrpe
-        self.excess_sigma = np.exp(self.excess_lr.std())-1
-        self.excess_sharpe = (self.excess_return_annual - self.rf)/(self.excess_sigma*np.sqrt(250))
-        # 回撤
         a = np.maximum.accumulate(self.net)
         self.drawdown = (a-self.net)/a
-    def cal_complex(self):
-        # 复杂指标 
-        win = self.lr[self.lr>0]
-        loss = self.lr[self.lr<0]
-        excesswin = self.excess_lr[self.excess_lr>0]
-        excessloss = self.excess_lr[self.excess_lr<0]
-        # 下行波动率
-        self.sigma_down = np.exp((self.lr-\
-                            self.lr.mean()).apply(lambda x: min(x,0)).std())-1
-        # 跟踪误差
-        self.sigma_alpha = np.exp(np.std(self.lr-\
-                             np.log(self.benchmark[self.benchmark.columns[0]]+1)))-1
-        # 超额回撤
-        excess_net = np.exp(self.excess_lr.fillna(0).cumsum())
-        a = np.maximum.accumulate(excess_net)
-        self.excess_drawdown = (a-excess_net)/a
+        # 超额表现
+        self.excess_lr = self.lr-np.log(self.benchmark[self.benchmark.columns[0]]+1) 
+        self.excess_net = np.exp(self.excess_lr.cumsum())
+        self.excess_total = self.excess_net[-1]/self.excess_net[0]                 
+        self.excess_return_annual = self.excess_total**(1/self.years)-1
+        self.excess_sigma = np.exp(self.excess_lr.std())-1
+        self.excess_sharpe = self.excess_return_annual/(self.excess_sigma*np.sqrt(250))
+        a = np.maximum.accumulate(self.excess_net)
+        self.excess_drawdown = (a-self.excess_net)/a
         # CAPM (无风险收益为0)
         y = self.returns.fillna(0)
         x = self.benchmark[self.benchmark.columns[0]].fillna(0)
         x = sm.add_constant(x)
         model = sm.OLS(y, x).fit()
-        # T-M 模型(无风险收益为0)
-        y = self.returns.fillna(0)
-        x = self.benchmark[self.benchmark.columns[0]].fillna(0)
-        x = sm.add_constant(x)
-        model = sm.OLS(y, x).fit()
         # 市场风险暴露
         self.beta = model.params[self.benchmark.columns[0]]
         # 市场波动无法解释的截距项
-        self.alpha = model.params['const'] 
+        self.alpha = model.params['const']
         #model.summary()
-        ## 索提诺比率   单位下行风险的超额收益
-        #self.sortino = (self.return_annual - self.rf)/(self.sigma_down*np.sqrt(250))
-        # 特雷诺指数  单位beta的超额收益
-        self.treynor  = (self.return_annual - self.rf)/self.beta 
-# 净值曲线
+
+        col0 = pd.DataFrame(columns=['col0'])
+        col0.loc[0] = '回测时间（年, 日）'
+        col0.loc[1] = '%s, %s'%(round(self.years,1), len(self.net))
+        col1 = pd.DataFrame(columns=['col1'])
+        col1.loc[0] = '年化收益率（%）'
+        col1.loc[1] = round(self.return_annual*100,1)
+        col1.loc[2] = '年化超额收益率（%）'
+        col1.loc[3] = round(self.excess_return_annual*100,1)
+        col2 = pd.DataFrame(columns=['col2'])
+        col2.loc[0] = '日胜率（%）'
+        col2.loc[1] = round(100*(self.returns>0).mean(),1) 
+        col2.loc[2] = '超额日胜率（%）'
+        col2.loc[3] = round(100*(self.excess_lr>0).mean(),1) 
+        col3 = pd.DataFrame(columns=['col3'])
+        col3.loc[0] = '最大回撤（%）'
+        col3.loc[1] = round(max(self.drawdown)*100, 1)
+        col3.loc[2] = '超额最大回撤（%）'
+        col3.loc[3] = round(max(self.excess_drawdown)*100, 1)
+        col3.loc[4] = '波动率（%）'
+        col3.loc[5] = round(self.sigma*np.sqrt(250)*100, 1)
+        col4 = pd.DataFrame(columns=['col4'])
+        col4.loc[0] = 'beta系数'
+        col4.loc[1] = round(self.beta,2) 
+        col4.loc[2] = '詹森指数（%）'
+        col4.loc[3] = round(self.alpha*250*100,1)
+        col5 = pd.DataFrame(columns=['col5'])
+        col5.loc[0] = '夏普比率'
+        col5.loc[1] = round(self.sharpe,2)
+        col5.loc[2] = '超额夏普' 
+        col5.loc[3] = round(self.excess_sharpe,2)
+        col5.loc[4] = '卡玛比率'
+        col5.loc[5] = round(self.return_annual/max(self.drawdown),2)
+        col6 = pd.DataFrame(columns=['col6'])
+        col6.loc[0] = ''
+        col6.loc[1] = '' 
+        col7 = pd.DataFrame(columns=['col7'])
+        col7.loc[0] = 'Hurst指数' 
+        col7.loc[1] = '' 
+        df_details = pd.concat([col0, col1, col2, col3, \
+                col4, col5, col6, col7], axis=1).fillna('')
+        self.df_details = df_details
+    def detail(self):
+        plt, fig, ax = matplot(w=22)
+        column_definitions = [ColumnDefinition(name='col0', group="基本参数"), \
+                              ColumnDefinition(name='col1', group="收益能力"), \
+                            ColumnDefinition(name='col2', group='收益能力'), \
+                            ColumnDefinition(name='col3', group='风险水平'), \
+                            ColumnDefinition(name="col4", group='风险调整'), \
+                            ColumnDefinition(name="col5", group='风险调整'), \
+                            ColumnDefinition(name="col6", group='策略执行'),
+                            ColumnDefinition(name="col7", group='业绩持续性分析')] +\
+                            [ColDef("index", title="", width=1.5, textprops={"ha":"right"})]
+        tab = Table(self.df_details, row_dividers=False, col_label_divider=False, 
+                    column_definitions=column_definitions,
+                    odd_row_color="#e0f6ff", even_row_color="#f0f0f0", 
+                    textprops={"ha": "center"})
+        #ax.set_xlim(2,5)
+        # 设置列标题文字和背景颜色(隐藏表头名)
+        tab.col_label_row.set_facecolor("white")
+        tab.col_label_row.set_fontcolor("white")
+        # 设置行标题文字和背景颜色
+        tab.columns["index"].set_facecolor("white")
+        tab.columns["index"].set_fontcolor("white")
+        tab.columns["index"].set_linewidth(0)
+        check_output()
+        plt.savefig('./output/details.png')
+        plt.show()
 # 时间起止（默认全部），是否显示细节,是否自定义输出图片名称，是否显示对数，是否显示超额
     def pnl(self, timerange=None, detail=True, filename=None, log=False, excess=False):
         plt, fig, ax = FB.display.matplot()
         # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
         if type(timerange) != type(None):
             # 时间段内净值与基准
             net = self.net.loc[timerange[0]:timerange[1]]
@@ -124,15 +166,15 @@
                 if excess:
                     ax.plot(np.exp(self.excess_lr.loc[timerange[0]:timerange[1]].cumsum()), 
                             c='C3', label='超额收益')
             else:
                 ax.text(0.7,0.05,'Sharpe:  {}'.format(round(sharpe,2)), transform=ax.transAxes)
             ax.plot(net/net[0], c='C0', label='p&l')
             # 如果基准是0就不绘制了
-            if not (self.benchmark==0).any().values[0]:
+            if not (self.benchmark==0).all().values[0]:
                 # benchmark 匹配回测时间段, 基准从0开始
                 benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
                 benchmark.loc[self.net.index[0]] = 0
                 # colors of benchmark
                 colors_list = ['C4','C5','C6','C7']
                 for i in range(len(benchmark.columns)):
                     ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), \
@@ -149,15 +191,15 @@
     #评价指标
             ax.text(0.7,0.05,'年化收益率: {}%\n夏普比率:   {}\n最大回撤:   {}%\n'.format(
             round(100*self.return_annual,2), round(self.sharpe,2), 
             round(100*max(self.drawdown),2)), transform=ax.transAxes)
         # 净值与基准
             ax.plot(self.net, c='C0', label=self.stratname)
             # 如果基准是0就不绘制了
-            if not (self.benchmark==0).any().values[0]:
+            if not (self.benchmark==0).all().values[0]:
                 # benchmark 匹配回测时间段, 基准从0开始
                 benchmark = self.benchmark.loc[self.net.index[0]:self.net.index[-1]].copy()
                 benchmark.loc[self.net.index[0]] = 0
                 # colors of benchmark
                 colors_list = ['C4','C5','C6','C7']
                 for i in range(len(benchmark.columns)):
                     ax.plot((benchmark[benchmark.columns[i]]+1).cumprod(), \
@@ -223,36 +265,41 @@
         plt, fig, ax = FB.display.matplot()
 
         len_years = len(yearly_returns)
         plot_x = range(len_years)
         plot_index = yearly_returns.index
         plot_height = yearly_returns['lr'].values
         plot_height1 = yearly_returns['bench'].values
+        max_height = max(np.hstack([plot_height, plot_height1]))
+        min_height = min(np.hstack([plot_height, plot_height1]))
+        height = max_height-min_height
         # 如果benchmark是0的话就不画对比了
         if not (self.benchmark==0).any().values[0]:
             ax.bar([i-0.225  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
             ax.bar([i+0.225  for i in plot_x], plot_height1, width=0.45, color='C4',\
                     label=self.benchmark.columns[0])
+            for x, contri in zip(plot_x, plot_height):
+                if contri>0:
+                    plt.text(x-0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
+                else:
+                    plt.text(x-0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
+            for x, contri in zip(plot_x, plot_height1):
+                if contri>0:
+                    plt.text(x+0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
+                else:
+                    plt.text(x+0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
         else:
             ax.bar([i  for i in plot_x], plot_height, width=0.45, color='C0', label='策略')
-        max_height = max(np.hstack([plot_height, plot_height1]))
-        min_height = min(np.hstack([plot_height, plot_height1]))
-        height = max_height-min_height
+            for x, contri in zip(plot_x, plot_height):
+                if contri>0:
+                    plt.text(x, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
+                else:
+                    plt.text(x, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
         plt.ylim(min_height-0.1*height, max_height+0.1*height)
 
-        for x, contri in zip(plot_x, plot_height):
-            if contri>0:
-                plt.text(x-0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
-            else:
-                plt.text(x-0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
-        for x, contri in zip(plot_x, plot_height1):
-            if contri>0:
-                plt.text(x+0.225, contri+height/30, round(contri,1), ha='center', color='C3', fontsize=8)
-            else:
-                plt.text(x+0.225, contri-height/20, round(contri,1), ha='center', color='C2', fontsize=8)
         plt.legend()
         plt.title('年度收益')
         plt.xticks(plot_x, labels=plot_index)
         check_output()
         plt.ylabel('(%)')
         plt.savefig('./output/pnl_yearly.png')
         plt.show()
@@ -276,19 +323,45 @@
 
 
 
 ############################################################################################
 ################################### 处理持仓表 ##############################################
 ############################################################################################
 class HoldPost(ReturnsPost):
-    def __init__(self, df_hold, market=None, \
+    # 持仓表、单边交易成本、market
+    def __init__(self, df_hold, comm=0/1e4, market=None, \
                  benchmark=0, stratname='策略'):
-        returns = df_hold.groupby('date')['next_returns'].mean()
-        super(HoldPost, self).__init__(returns, benchmark=benchmark, stratname=stratname) 
-
+        self.df_hold = df_hold
+        # 等权持仓
+        df_hold['weight'] = 1
+        df_hold['weight'] = df_hold['weight']/df_hold['weight'].groupby('date').sum()
+        # 初始状态全仓为现金,没有现金列则
+        pos_df = df_hold['weight'].unstack('code').fillna(0)
+        pos_df_shift = pos_df.shift().fillna(0).copy()
+        pos_df_shift.loc[pos_df.index[0], 'deposit'] = 1
+        pos_df_shift.fillna(0)
+        # 去掉现金列的绝对值增减之和即为换手率
+        self.turnover_ser = abs(pos_df-pos_df_shift).drop(columns=['deposit', ]).sum(axis=1)
+        # 收益率
+        returns = (df_hold.groupby('date')['next_returns'].mean()+1)*(1-self.turnover_ser*comm)-1
+        super(HoldPost, self).__init__(returns, benchmark=benchmark, stratname=stratname)
+        self.df_details.loc[0, 'col6'] = '年换手' 
+        self.df_details.loc[1, 'col6'] = round(self.turnover_ser.mean()*250,1)
+    def turnover(self):
+        plt, fig, ax = FB.display.matplot()
+        ax.plot(self.turnover_ser*250, alpha=0.2)
+        ax.plot(self.turnover_ser.rolling(20).mean()*250, label='20日滚动换手')
+        ax.plot(self.turnover_ser.rolling(250).mean()*250, label='250日滚动换手')
+        ax.legend()
+        check_output()
+        plt.savefig('./output/turnover.png')
+        plt.show()
+    def get_contribution(self):
+        real_returns = self.df_hold['next_returns']/self.df_hold.groupby('date')['next_returns'].count()
+        self.contribution = ((real_returns+1).groupby('code').prod()-1).sort_values()
 
 
 ########################################################################################################
 ####################################  barbybar.world  ##################################################
 ########################################################################################################
 
 # 传入barbybar运行完毕的world对象
```

### Comparing `FreeBack-4.1.3a0/FreeBack/strat.py` & `FreeBack-4.2.4a0/FreeBack/strat.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def add_deposit(market):
         deposit = pd.DataFrame(index=market.index.get_level_values(0).unique())
         deposit['code']  = 'deposit'
         deposit['next_returns'] = 0
         deposit = deposit.reset_index(['date', 'code'])
         return pd.concat([market, deposit]).sort_values('date')
     if type(strat0['in/exclude'])==list:
-        if strat0['in/exclude']==[]:
+        if (strat0['in/exclude']==[]) | (strat0['in/exclude'][0]==''):
             # 空仓
             deposit = pd.DataFrame(index=market.index.get_level_values(0).unique())
             deposit['code'] = 'deposit'
             deposit['next_returns'] = 0
             return deposit.reset_index().set_index(['date', 'code'])
         else:
             return market.loc[:, strat0['in/exclude'], :][['next_returns']]
```

### Comparing `FreeBack-4.1.3a0/FreeBack.egg-info/PKG-INFO` & `FreeBack-4.2.4a0/FreeBack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.1.3a0
+Version: 4.2.4a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.1.3a0/LICENSE` & `FreeBack-4.2.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/PKG-INFO` & `FreeBack-4.2.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.1.3a0
+Version: 4.2.4a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.1.3a0/README.md` & `FreeBack-4.2.4a0/README.md`

 * *Files identical despite different names*

### Comparing `FreeBack-4.1.3a0/setup.py` & `FreeBack-4.2.4a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 setup(
     name="FreeBack",
     # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
     # (每次高级别序号增加后,低级别序号归0)
     # alpha为调试版,beta为测试版,stable为稳定版 
-    version="4.1.3-alpha",
+    version="4.2.4-alpha",
     author="LH.Li,zzq",
     author_email="lh98lee@zju.edu.cn",  
     description='Package for backtest',
     long_description=long_description, 
     # 描述文件为md格式
     long_description_content_type="text/markdown",
     url="https://github.com/LHanLi/FreeBack",
```

