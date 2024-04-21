# Comparing `tmp/bosing-2.0.0b1.tar.gz` & `tmp/bosing-2.0.0b2.tar.gz`

## Comparing `bosing-2.0.0b1.tar` & `bosing-2.0.0b2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 bosing-2.0.0b1/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.github/dependabot.yml
--rw-r--r--   0     1001      127     6307 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-20 18:18:31.000000 bosing-2.0.0b1/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-20 18:18:31.000000 bosing-2.0.0b1/LICENSE.txt
--rw-r--r--   0     1001      127     1348 2024-04-20 18:18:31.000000 bosing-2.0.0b1/README.md
--rw-r--r--   0     1001      127    10174 2024-04-20 18:18:31.000000 bosing-2.0.0b1/bosing.pyi
--rw-r--r--   0     1001      127      634 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/conf.py
--rw-r--r--   0     1001      127     1262 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/index.rst
--rw-r--r--   0     1001      127     2259 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/quickstart.rst
--rw-r--r--   0     1001      127       16 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-20 18:18:31.000000 bosing-2.0.0b1/docs/schedule.rst
--rw-r--r--   0     1001      127     1138 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/flexible.py
--rw-r--r--   0     1001      127      521 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/hann.py
--rw-r--r--   0     1001      127      770 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/interp.py
--rw-r--r--   0     1001      127      682 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/overlap.py
--rw-r--r--   0     1001      127     2219 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/schedule.py
--rw-r--r--   0     1001      127     1879 2024-04-20 18:18:31.000000 bosing-2.0.0b1/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-20 18:18:31.000000 bosing-2.0.0b1/ruff_defaults.toml
--rw-r--r--   0     1001      127    48283 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/lib.rs
--rw-r--r--   0     1001      127     9860 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/sampler.rs
--rw-r--r--   0     1001      127     2479 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7387 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3311 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/play.rs
--rw-r--r--   0     1001      127     2349 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3944 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5741 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11082 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/schedule.rs
--rw-r--r--   0     1001      127     4160 2024-04-20 18:18:31.000000 bosing-2.0.0b1/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-04-20 18:18:31.000000 bosing-2.0.0b1/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-20 18:18:31.000000 bosing-2.0.0b1/tests/__init__.py
--rw-r--r--   0     1001      127     1171 2024-04-20 18:18:31.000000 bosing-2.0.0b1/tests/test_basic.py
--rw-r--r--   0     1001      127    13735 2024-04-20 18:18:40.000000 bosing-2.0.0b1/Cargo.lock
--rw-r--r--   0     1001      127     1879 2024-04-20 18:18:31.000000 bosing-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 bosing-2.0.0b2/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-21 14:56:40.000000 bosing-2.0.0b2/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6307 2024-04-21 14:56:40.000000 bosing-2.0.0b2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-21 14:56:40.000000 bosing-2.0.0b2/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-21 14:56:40.000000 bosing-2.0.0b2/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-21 14:56:40.000000 bosing-2.0.0b2/LICENSE.txt
+-rw-r--r--   0     1001      127     1348 2024-04-21 14:56:40.000000 bosing-2.0.0b2/README.md
+-rw-r--r--   0     1001      127    10174 2024-04-21 14:56:40.000000 bosing-2.0.0b2/bosing.pyi
+-rw-r--r--   0     1001      127      634 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/quickstart.rst
+-rw-r--r--   0     1001      127       16 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-21 14:56:40.000000 bosing-2.0.0b2/docs/schedule.rst
+-rw-r--r--   0     1001      127     1138 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/flexible.py
+-rw-r--r--   0     1001      127      521 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/hann.py
+-rw-r--r--   0     1001      127      770 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/interp.py
+-rw-r--r--   0     1001      127      682 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/overlap.py
+-rw-r--r--   0     1001      127     2219 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/schedule.py
+-rw-r--r--   0     1001      127     1879 2024-04-21 14:56:40.000000 bosing-2.0.0b2/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-21 14:56:40.000000 bosing-2.0.0b2/ruff_defaults.toml
+-rw-r--r--   0     1001      127    60730 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/lib.rs
+-rw-r--r--   0     1001      127     9860 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/sampler.rs
+-rw-r--r--   0     1001      127     2479 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7387 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3311 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2349 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3944 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5741 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11082 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/schedule.rs
+-rw-r--r--   0     1001      127     4160 2024-04-21 14:56:40.000000 bosing-2.0.0b2/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-21 14:56:40.000000 bosing-2.0.0b2/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-21 14:56:40.000000 bosing-2.0.0b2/tests/__init__.py
+-rw-r--r--   0     1001      127     1171 2024-04-21 14:56:40.000000 bosing-2.0.0b2/tests/test_basic.py
+-rw-r--r--   0     1001      127    13735 2024-04-21 14:56:58.000000 bosing-2.0.0b2/Cargo.lock
+-rw-r--r--   0     1001      127     1879 2024-04-21 14:56:40.000000 bosing-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b2/PKG-INFO
```

### Comparing `bosing-2.0.0b1/.github/workflows/ci.yml` & `bosing-2.0.0b2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/.gitignore` & `bosing-2.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/.readthedocs.yaml` & `bosing-2.0.0b2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/LICENSE.txt` & `bosing-2.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/README.md` & `bosing-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/bosing.pyi` & `bosing-2.0.0b2/bosing.pyi`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/docs/Makefile` & `bosing-2.0.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/docs/conf.py` & `bosing-2.0.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/docs/index.rst` & `bosing-2.0.0b2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,19 @@
 
 从源码安装
 ----------
 
 #. 安装 Rust toolchain 1.74+
 #. 安装 Python 3.8+
 #. Clone 本项目并安装
-
     .. code-block:: console
 
         $ git clone https://github.com/kahojyun/Bosing.git
         $ cd Bosing
-        $ pip install -e .
+        $ pip install .
 
 注意
 ----
 
 .. caution::
 
     项目中所有相位 (phase) 的单位均为周期数, 比如 :math:`1` 代表弧度制的
```

### Comparing `bosing-2.0.0b1/docs/instruction.rst` & `bosing-2.0.0b2/docs/instruction.rst`

 * *Files 16% similar despite different names*

```diff
@@ -28,61 +28,37 @@
 相位计算
 --------
 
 .. note::
 
     公式中的相位单位均为周期数, 即 :math:`2\pi` 的倍数.
 
-目前程序会记录三种频率: 通道的载波频率 :math:`f_c`, 由于频率偏置而产生的额外频率
-:math:`f_a`, 以及 :class:`Play` 指令中的附加频率 :math:`f_p`. 前两者相加得到全局
-频率 :math:`f`, 即 :math:`f = f_c + f_a`. 相位则记录两种: 通道的初相位
-:math:`\phi_0` 与 :class:`Play` 指令中的附加相位 :math:`\phi_p`. 利用这些信息可
-以计算出时刻 :math:`t` 的额外相位 :math:`\phi_a(t)`:
+对于每个通道，``bosing`` 记录了以下信息:
 
-.. math::
-
-    \phi_a(t) = f_a t + \phi_0
-
-载波相位 :math:`\phi_c(t)`:
-
-.. math::
-
-    \phi_c(t) = \phi_a(t) + f_c t = f t + \phi_0
-
-起始时刻为 :math:`\tau` 的波形中的相位 :math:`\phi_p(t)` 则为:
-
-.. math::
+- 通道的载波频率 :math:`f_0`
+- 由于频率偏置而产生的额外频率 :math:`\Delta f`
+- 通道的初相位 :math:`\phi_c`
 
-    \phi_p(t) = \phi_c(t) + f_p (t - \tau)
-
-目前 :class:`ShiftFreq` 指令与 :class:`SetFreq` 指令改变的是 :math:`f_a`, 并且会
-令额外相位 :math:`\phi_a(t)` 在给定时刻 :math:`\tau` 连续:
+而 :class:`Play` 指令中还可以指定额外频率 :math:`f_p` 与额外相位 :math:`\phi_p`.
+假设经过 DRAG 修正后的波形包络为 :math:`E_d(t)`, 波形起始时间为 :math:`t_0`, 则
+混频后的波形为
 
 .. math::
 
-    \phi_a(\tau) = f_a \tau + \phi_0 = \phi_a'(\tau) = f_a' \tau +
-    \phi_0'
-
-:class:`ShiftPhase` 指令直接改变 :math:`\phi_0`, 不受时间影响.
-:class:`SetPhase` 改变 :math:`\phi_0` 使得给定时刻 :math:`\tau` 的
-额外相位 :math:`\phi_a(\tau)` 变为给定值 :math:`\phi`:
+    P(t) = E_d(t) \exp \big[ i 2 \pi ((f_0 + \Delta f) t + f_p (t-t_0) + \phi_c + \phi_p) \big]
 
-.. math::
+涉及相位的指令还有
 
-    \phi_a'(\tau) = f_a \tau + \phi_0' = \phi
+- :class:`ShiftPhase`:
+    改变 :math:`\phi_c`, 与时间无关
 
-:class:`SwapPhase` 指令在给定时刻 :math:`\tau` 交换两个通道的
-载波相位 :math:`\phi_c^{(1)}(\tau)` 与 :math:`\phi_c^{(2)}(\tau)`:
-
-.. math::
-
-    \phi_c^{(1)'}(\tau) = \phi_c^{(2)}(\tau) \\
-    \phi_c^{(2)'}(\tau) = \phi_c^{(1)}(\tau)
-
-最后生成波形时, ``bosing`` 采用的 I, Q 通道混频公式为:
-
-.. math::
+- :class:`SetPhase`:
+    改变 :math:`\phi_c`, 使得在指定时间 :math:`t` 时相位为 :math:`\phi`. 计算相位时
+    只包括 :math:`\Delta f`
 
-    I(t) = E(t)\cos(2\pi\phi_p(t)) \\
-    Q(t) = E(t)\sin(2\pi\phi_p(t))
+- :class:`SwapPhase`:
+    改变两个通道的 :math:`\phi_c`, 使得在指定时间 :math:`t` 时两个通道的相位交换. 计算相位时
+    包括 :math:`f_0` 与 :math:`\Delta f`
 
-其中 :math:`E(t)` 为包络.
+- :class:`ShiftFreq` 与 :class:`SetFreq`:
+    改变 :math:`\Delta f`, 同时改变 :math:`\phi_c` 使得在指定时间 :math:`t` 时相位保持连续.
+    计算相位时只包括 :math:`\Delta f`
```

### Comparing `bosing-2.0.0b1/docs/make.bat` & `bosing-2.0.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/docs/schedule.rst` & `bosing-2.0.0b2/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/flexible.py` & `bosing-2.0.0b2/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/hann.py` & `bosing-2.0.0b2/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/interp.py` & `bosing-2.0.0b2/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/overlap.py` & `bosing-2.0.0b2/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/schedule.py` & `bosing-2.0.0b2/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/example/schedule_stress.py` & `bosing-2.0.0b2/example/schedule_stress.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/ruff_defaults.toml` & `bosing-2.0.0b2/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/lib.rs` & `bosing-2.0.0b2/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,26 @@
 mod schedule;
 mod shape;
 
 #[global_allocator]
 static GLOBAL: MiMalloc = MiMalloc;
 
 /// Channel configuration.
+///
+/// `align_level` is the time axis alignment granularity. With sampling interval
+/// :math:`\Delta t` and `align_level` :math:`n`, start of pulse is aligned to
+/// the nearest multiple of :math:`2^n \Delta t`.
+///
+/// Args:
+///     name (str): Name of the channel.
+///     base_freq (float): Base frequency of the channel.
+///     sample_rate (float): Sample rate of the channel.
+///     length (int): Length of the waveform.
+///     delay (float): Delay of the channel. Defaults to 0.0.
+///     align_level (int): Time axis alignment granularity. Defaults to -10.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Channel {
     name: String,
     base_freq: f64,
     sample_rate: f64,
     length: usize,
@@ -52,26 +64,49 @@
             delay,
             align_level,
         }
     }
 }
 
 /// Alignment of a schedule element.
+///
+/// The alignment of a schedule element is used to align the element within its
+/// parent element. The alignment can be one of the following:
+///
+/// - :attr:`Alignment.End`
+/// - :attr:`Alignment.Start`
+/// - :attr:`Alignment.Center`
+/// - :attr:`Alignment.Stretch`: Stretch the element to fill the parent.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 enum Alignment {
     End,
     Start,
     Center,
     Stretch,
 }
 
 #[pymethods]
 impl Alignment {
     /// Convert the value to Alignment.
+    ///
+    /// The value can be one of the following:
+    ///
+    /// - :class:`Alignment`
+    /// - "end"
+    /// - "start"
+    /// - "center"
+    /// - "stretch"
+    ///
+    /// Args:
+    ///     obj (str | Alignment): The value to convert.
+    /// Returns:
+    ///     Alignment: The converted value.
+    /// Raises:
+    ///     ValueError: If the value cannot be converted to Alignment.
     #[staticmethod]
     fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(s) = obj.extract() {
             let alignment = match s {
@@ -94,14 +129,24 @@
 }
 
 fn extract_alignment(obj: &Bound<'_, PyAny>) -> PyResult<Alignment> {
     Alignment::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
 /// Base class for shapes.
+///
+/// Shapes are used to define the envelope of a pulse. Internally, the shape is
+/// represented as a function :math:`f(t)` defined on the interval :math:`t \in
+/// [-0.5, 0.5]`. The shape should be normalized such that :math:`f(\pm 0.5) = 0`
+/// and :math:`f(0) = 1`.
+///
+/// Following shapes are supported:
+///
+/// - :class:`Hann`: Hann window.
+/// - :class:`Interp`: Interpolated shape.
 #[pyclass(subclass, frozen)]
 #[derive(Debug, Clone)]
 struct Shape;
 
 impl Shape {
     fn get_rust_shape(slf: &Bound<'_, Shape>) -> PyResult<shape::Shape> {
         if slf.downcast::<Hann>().is_ok() {
@@ -133,14 +178,23 @@
 }
 
 /// An interpolated shape.
 ///
 /// The interpolated shape use a B-spline. :func:`scipy.interpolate.make_interp_spline`
 /// can be used to calculate the parameters.
 ///
+/// .. caution::
+///
+///     It's user's responsibility to ensure the b-spline parameters are valid and
+///     the shape is normalized such that :math:`f(\pm 0.5) = 0` and :math:`f(0) = 1`.
+///
+/// Args:
+///     knots (Sequence[float]): Knots of the B-spline.
+///     controls (Sequence[float]): Control points of the B-spline.
+///     degree (int): Degree of the B-spline.
 /// Example:
 ///     .. code-block:: python
 ///
 ///         import numpy as np
 ///         from scipy.interpolate import make_interp_spline
 ///         from bosing import Interp
 ///         x = np.linspace(0, np.pi, 10)
@@ -174,67 +228,123 @@
 fn extract_margin(obj: &Bound<'_, PyAny>) -> PyResult<(f64, f64)> {
     if let Ok(v) = obj.extract() {
         return Ok((v, v));
     }
     if let Ok((v1, v2)) = obj.extract() {
         return Ok((v1, v2));
     }
-    let msg = "Failed to convert the value to (f64, f64).";
+    let msg = "Failed to convert the value to (float, float).";
     Err(PyValueError::new_err(msg))
 }
 
 /// Base class for schedule elements.
 ///
 /// A schedule element is a node in the tree structure of a schedule similar to
 /// HTML elements. The design is inspired by `XAML in WPF / WinUI
 /// <https://learn.microsoft.com/en-us/windows/apps/design/layout/layouts-with-xaml>`_
 ///
-/// When :attr:`duration`, :attr:`max_duration`, and :attr:`min_duration` are
-/// conflicting, the priority is as follows:
+/// Every element has the following properties:
 ///
-/// 1. :attr:`min_duration`
-/// 2. :attr:`max_duration`
-/// 3. :attr:`duration`
+/// - :attr:`margin`
+///     The margin of an element is a tuple of two floats representing the
+///     margin before and after the element. If :attr:`margin` is set to a
+///     single float, both sides use the same value.
+///
+///     Similar to margins in XAML, margins don't collapse. For example, if two
+///     elements have a margin of 10 and 20, the space between the two elements
+///     is 30, not 20.
+///
+/// - :attr:`alignment`
+///     The alignment of the element. Currently, this property takes effect only
+///     when the element is a child of a :class:`Grid` element.
+///
+/// - :attr:`phantom`
+///     Whether the element is a phantom element. Phantom elements are measured
+///     and arranged in the layout but do not add to the waveforms.
+///
+/// - :attr:`duration`, :attr:`max_duration`, and :attr:`min_duration`
+///     Constraints on the duration of the element. When :attr:`duration`,
+///     :attr:`max_duration`, and :attr:`min_duration` are conflicting, the
+///     priority is as follows:
+///
+///     1. :attr:`min_duration`
+///     2. :attr:`max_duration`
+///     3. :attr:`duration`
+///
+///     When :attr:`duration` is not set, the duration is calculated such that
+///     the element occupies the minimum duration.
+///
+/// There are two types of elements:
+///
+/// - Instruction elements:
+///     Elements that instruct the waveform generator to perform certain
+///     operations, such as playing a pulse or setting the phase of a channel.
+///
+///     - :class:`Play`: Play a pulse on a channel.
+///     - :class:`ShiftPhase`: Shift the phase of a channel.
+///     - :class:`SetPhase`: Set the phase of a channel.
+///     - :class:`ShiftFreq`: Shift the frequency of a channel.
+///     - :class:`SetFreq`: Set the frequency of a channel.
+///     - :class:`SwapPhase`: Swap the phase of two channels.
+///
+///     The timing information required by the waveform generator is calculated
+///     by the layout system.
+///
+/// - Layout elements:
+///     Elements that control the layout of child elements.
+///
+///     - :class:`Grid`: Grid layout.
+///     - :class:`Stack`: Stack layout.
+///     - :class:`Absolute`: Absolute layout.
+///     - :class:`Repeat`: Repeat element.
+///     - :class:`Barrier`: Barrier element.
+///
+/// Args:
+///     margin (float | tuple[float, float]): Margin of the element. Defaults to
+///         0.
+///     alignment (str | Alignment): Alignment of the element. The value can
+///         be :class:`Alignment` or one of 'end', 'start', 'center', 'stretch'.
+///         Defaults to :attr:`Alignment.End`.
+///     phantom (bool): Whether the element is a phantom element and should not
+///         add to waveforms. Defaults to ``False``.
+///     duration (float): Duration of the element. Defaults to ``None``.
+///     max_duration (float): Maximum duration of the element. Defaults to
+///         ``inf``.
+///     min_duration (float): Minimum duration of the element. Defaults to 0.
 #[pyclass(subclass, frozen)]
 #[derive(Debug, Clone)]
 struct Element(Arc<schedule::Element>);
 
 #[pymethods]
 impl Element {
-    /// tuple[float, float]: Margin of the element.
     #[getter]
     fn margin(&self) -> (f64, f64) {
         self.0.common().margin()
     }
 
-    /// Alignment: Alignment of the element.
     #[getter]
     fn alignment(&self) -> Alignment {
         self.0.common().alignment()
     }
 
-    /// bool: Whether the element is a phantom element and should not add to waveforms.
     #[getter]
     fn phantom(&self) -> bool {
         self.0.common().phantom()
     }
 
-    /// float | None: Duration of the element.
     #[getter]
     fn duration(&self) -> Option<f64> {
         self.0.common().duration()
     }
 
-    /// float: Maximum duration of the element.
     #[getter]
     fn max_duration(&self) -> f64 {
         self.0.common().max_duration()
     }
 
-    /// float: Minimum duration of the element.
     #[getter]
     fn min_duration(&self) -> f64 {
         self.0.common().min_duration()
     }
 }
 
 fn build_element(
@@ -262,17 +372,53 @@
         .build()
         .map_err(|e| PyValueError::new_err(e.to_string()))?;
     Ok(Element(Arc::new(schedule::Element::new(common, variant))))
 }
 
 /// A pulse play element.
 ///
-/// If :attr:`flexible` is set to ``True`` and :attr:`alignment` is set to
-/// :attr:`Alignment.Stretch`, the plateau of the pulse is stretched to fill the
-/// parent element.
+/// Given the pulse envelope :math:`E(t)`, channel total frequency :math:`f_c`,
+/// and channel phase :math:`\phi_c`, the the final pulse :math:`P(t)` starts at
+/// :math:`t_0` with sideband will be
+///
+/// .. math::
+///
+///     E_d(t) = \left( 1 + i \alpha \frac{d}{dt} \right) E(t)
+///
+///     P(t) = E_d(t) \exp \big[ i 2 \pi (f_c t + f_p (t-t_0) + \phi_c + \phi_p) \big]
+///
+/// where :math:`\alpha` is the `drag_coef` parameter, :math:`f_p` is the
+/// `frequency` parameter, and :math:`\phi_p` is the `phase` parameter. The
+/// derivative is calculated using the central difference method. An exceptional
+/// case is when the pulse is a rectangular pulse. In this case, the drag
+/// coefficient is ignored.
+///
+/// If `flexible` is set to ``True``, the `plateau` parameter is ignored and the
+/// actual plateau length is determined by the duration of the element.
+///
+/// .. caution::
+///
+///     The unit of phase is number of cycles, not radians. For example, a phase
+///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
+///
+/// Args:
+///     channel_id (int): Target channel ID.
+///     shape_id (int | None): Shape ID of the pulse. If ``None``, the pulse is
+///         a rectangular pulse.
+///     amplitude (float): Amplitude of the pulse.
+///     width (float): Width of the pulse.
+///     plateau (float): Plateau length of the pulse. Defaults to 0.
+///     drag_coef (float): Drag coefficient of the pulse. If the pulse is a
+///         rectangular pulse, the drag coefficient is ignored. Defaults to 0.
+///     frequency (float): Additional frequency of the pulse on top of channel
+///         base frequency and frequency shift. Defaults to 0.
+///     phase (float): Additional phase of the pulse in **cycles**. Defaults to
+///         0.
+///     flexible (bool): Whether the pulse has flexible plateau length. Defaults
+///         to ``False``.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct Play;
 
 #[pymethods]
 impl Play {
     #[new]
@@ -337,138 +483,126 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID.
     #[getter]
     fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .channel_id();
         Ok(ret)
     }
 
-    /// int | None: Shape ID of the pulse. If ``None``, the pulse is a
-    ///     rectangular pulse.
     #[getter]
     fn shape_id(slf: &Bound<'_, Self>) -> PyResult<Option<usize>> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .shape_id();
         Ok(ret)
     }
 
-    /// float: Amplitude of the pulse.
     #[getter]
     fn amplitude(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .amplitude();
         Ok(ret)
     }
 
-    /// float: Width of the pulse.
     #[getter]
     fn width(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .width();
         Ok(ret)
     }
 
-    /// float: Plateau of the pulse.
     #[getter]
     fn plateau(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .plateau();
         Ok(ret)
     }
 
-    /// float: Drag coefficient of the pulse. If the pulse is a rectangular pulse,
-    ///     the drag coefficient is ignored.
     #[getter]
     fn drag_coef(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .drag_coef();
         Ok(ret)
     }
 
-    /// float: Additional frequency of the pulse on top of channel base
-    ///     frequency and frequency shift.
     #[getter]
     fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .frequency();
         Ok(ret)
     }
 
-    /// float: Additional phase of the pulse in **cycles**.
     #[getter]
     fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .phase();
         Ok(ret)
     }
 
-    /// bool: Whether the pulse is flexible and should stretch to fill the parent.
     #[getter]
     fn flexible(slf: &Bound<'_, Self>) -> PyResult<bool> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
@@ -477,14 +611,26 @@
             ))?
             .flexible();
         Ok(ret)
     }
 }
 
 /// A phase shift element.
+///
+/// Phase shift will be added to the channel phase offset :math:`\phi_c` and is
+/// time-independent.
+///
+/// .. caution::
+///
+///     The unit of phase is number of cycles, not radians. For example, a phase
+///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
+///
+/// Args:
+///     channel_id (int): Target channel ID.
+///     phase (float): Phase shift in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftPhase;
 
 #[pymethods]
 impl ShiftPhase {
     #[new]
@@ -522,30 +668,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID.
     #[getter]
     fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the shift_phase variant from the element.",
             ))?
             .channel_id();
         Ok(ret)
     }
 
-    /// float: Phase shift in **cycles**.
     #[getter]
     fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_phase()
@@ -555,24 +699,33 @@
             .phase();
         Ok(ret)
     }
 }
 
 /// A phase set element.
 ///
-/// Given the base frequency :math:`f`, the frequency shift :math:`\\Delta f`,
-/// the time :math:`t`, and the phase offset :math:`\\phi_0`, the phase is
-/// defined as
+/// Waveform generator treats the base frequency :math:`f_0` and the channel
+/// frequency shift :math:`\Delta f` differently. :math:`f_0` is never changed
+/// during the execution of the schedule, while :math:`\Delta f` can be changed
+/// by :class:`ShiftFreq` and :class:`SetFreq`. :class:`SetPhase` only considers
+/// :math:`\Delta f` part of the frequency. The channel phase offset
+/// :math:`\phi_c` will be adjusted such that
 ///
-/// .. math::
+/// .. math:: \Delta f t + \phi_c = \phi
+///
+/// at the scheduled time point, where :math:`\phi` is the `phase` parameter.
+///
+/// .. caution::
 ///
-///     \\phi(t) = (f + \\Delta f) t + \\phi_0
+///     The unit of phase is number of cycles, not radians. For example, a phase
+///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 ///
-/// :class:`SetPhase` sets the phase offset :math:`\\phi_0` such that
-/// :math:`\\phi(t)` is equal to the given phase.
+/// Args:
+///     channel_id (int): Target channel ID.
+///     phase (float): Target phase value in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetPhase;
 
 #[pymethods]
 impl SetPhase {
     #[new]
@@ -610,30 +763,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID.
     #[getter]
     fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the set_phase variant from the element.",
             ))?
             .channel_id();
         Ok(ret)
     }
 
-    /// float: Target phase value in **cycles**.
     #[getter]
     fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_phase()
@@ -643,17 +794,21 @@
             .phase();
         Ok(ret)
     }
 }
 
 /// A frequency shift element.
 ///
-/// Additional frequency shift on top of the channel cumulative frequency shift.
-/// Phase offset will be adjusted accordingly such that the phase is continuous
-/// at the shift point.
+/// Frequency shift will be added to the channel frequency shift :math:`\Delta
+/// f` and the channel phase offset :math:`\phi_c` will be adjusted such that
+/// the phase is continuous at the scheduled time point.
+///
+/// Args:
+///     channel_id (int): Target channel ID.
+///     frequency (float): Delta frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftFreq;
 
 #[pymethods]
 impl ShiftFreq {
     #[new]
@@ -691,30 +846,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID.
     #[getter]
     fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_freq()
             .ok_or(PyValueError::new_err(
                 "Failed to get the shift_freq variant from the element.",
             ))?
             .channel_id();
         Ok(ret)
     }
 
-    /// float: Delta frequency.
     #[getter]
     fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_freq()
@@ -724,16 +877,22 @@
             .frequency();
         Ok(ret)
     }
 }
 
 /// A frequency set element.
 ///
-/// Set the channel frequency shift to the target frequency. Phase offset will
-/// be adjusted accordingly such that the phase is continuous at the shift point.
+/// The channel frequency shift :math:`\Delta f` will be set to the provided
+/// `frequency` parameter and the channel phase offset :math:`\phi_c` will be
+/// adjusted such that the phase is continuous at the scheduled time point.
+/// The channel base frequency :math:`f_0` will not be changed.
+///
+/// Args:
+///     channel_id (int): Target channel ID.
+///     frequency (float): Target frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetFreq;
 
 #[pymethods]
 impl SetFreq {
     #[new]
@@ -771,30 +930,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID.
     #[getter]
     fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_freq()
             .ok_or(PyValueError::new_err(
                 "Failed to get the set_freq variant from the element.",
             ))?
             .channel_id();
         Ok(ret)
     }
 
-    /// float: Target frequency.
     #[getter]
     fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_freq()
@@ -804,22 +961,24 @@
             .frequency();
         Ok(ret)
     }
 }
 
 /// A phase swap element.
 ///
-/// This instruction swaps carrier phases between two target channels at the
-/// scheduled time point. Carrier phase is defined as
+/// Different from :class:`SetPhase` and :class:`SetFreq`, both the channel
+/// base frequency :math:`f_0` and the channel frequency shift :math:`\Delta f`
+/// will be considered. At the scheduled time point, the phase to be swapped
+/// is calculated as
 ///
-/// .. math::
-///     \\phi(t) = (f + \\Delta f) t + \\phi_0
+/// .. math:: \phi(t) = (f_0 + \Delta f) t + \phi_c
 ///
-/// where :math:`f` is the base frequency, :math:`\\Delta f` is the frequency
-/// shift, :math:`t` is the time, and :math:`\\phi_0` is the phase offset.
+/// Args:
+///     channel_id1 (int): Target channel ID 1.
+///     channel_id2 (int): Target channel ID 2.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SwapPhase;
 
 #[pymethods]
 impl SwapPhase {
     #[new]
@@ -856,30 +1015,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Target channel ID 1.
     #[getter]
     fn channel_id1(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_swap_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the swap_phase variant from the element.",
             ))?
             .channel_id1();
         Ok(ret)
     }
 
-    /// int: Target channel ID 2.
     #[getter]
     fn channel_id2(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_swap_phase()
@@ -889,19 +1046,23 @@
             .channel_id2();
         Ok(ret)
     }
 }
 
 /// A barrier element.
 ///
-/// A barrier element is a zero-duration no-op element. Useful for aligning
-/// elements on different channels in :class:`Stack`.
+/// A barrier element is a no-op element. Useful for aligning elements on
+/// different channels and adding space between elements in a :class:`Stack`
+/// layout.
 ///
-/// If :attr:`channel_ids` is empty, the barrier is applied to
-/// all channels in its parent element.
+/// If no channel IDs are provided, the layout system will arrange the barrier
+/// element as if it occupies all channels in its parent.
+///
+/// Args:
+///     *channel_ids (int): Channel IDs. Defaults to empty.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct Barrier;
 
 #[pymethods]
 impl Barrier {
     #[new]
@@ -934,16 +1095,14 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// Sequence[int]: Target channel IDs. The returned value is a copy of the
-    ///     internal channel IDs.
     #[getter]
     fn channel_ids(slf: &Bound<'_, Self>) -> PyResult<Vec<usize>> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_barrier()
@@ -952,19 +1111,25 @@
             ))?
             .channel_ids()
             .to_vec();
         Ok(ret)
     }
 }
 
-/// A repeated schedule element.
+/// A repeat element.
+///
+/// Repeat the child element multiple times with a spacing between repetitions.
+///
+/// Args:
+///     child (Element): Child element to repeat.
+///     count (int): Number of repetitions.
+///     spacing (float): Spacing between repetitions. Defaults to 0.
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Repeat {
-    /// Element: Child element to repeat.
     child: Py<Element>,
 }
 
 #[pymethods]
 impl Repeat {
     #[new]
     #[pyo3(signature = (
@@ -1005,30 +1170,28 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
-    /// int: Number of repetitions.
     #[getter]
     fn count(slf: &Bound<'_, Self>) -> PyResult<usize> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_repeat()
             .ok_or(PyValueError::new_err(
                 "Failed to get the repeat variant from the element.",
             ))?
             .count();
         Ok(ret)
     }
 
-    /// float: Spacing between repetitions.
     #[getter]
     fn spacing(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_repeat()
@@ -1036,25 +1199,47 @@
                 "Failed to get the repeat variant from the element.",
             ))?
             .spacing();
         Ok(ret)
     }
 }
 
-/// Direction of arrangement.
+/// Layout order in a stack layout.
+///
+/// A stack layout has two possible children processing orders:
+///
+/// - :attr:`Direction.Backward`:
+///     Process children in reverse order and schedule them as late as possible.
+///     This is the default order.
+///
+/// - :attr:`Direction.Forward`:
+///     Process children in original order and schedule them as early as
+///     possible.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 enum Direction {
     Backward,
     Forward,
 }
 
 #[pymethods]
 impl Direction {
     /// Convert the value to Direction.
+    ///
+    /// The value can be:
+    ///
+    /// - :class:`Direction`
+    /// - str: 'backward' or 'forward'
+    ///
+    /// Args:
+    ///     obj (str | Direction): Value to convert.
+    /// Returns:
+    ///     Direction: Converted value.
+    /// Raises:
+    ///     ValueError: If the value cannot be converted.
     #[staticmethod]
     fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(s) = obj.extract() {
             let direction = match s {
@@ -1074,25 +1259,28 @@
     }
 }
 
 fn extract_direction(obj: &Bound<'_, PyAny>) -> PyResult<Direction> {
     Direction::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
-/// Layout child elements in one direction.
+/// A stack layout element.
 ///
-/// The child elements are arranged in one direction. The direction can be
-/// forwards or backwards.
+/// Each child element occupies some channels and has a duration. Stack layout
+/// will put children as close as possible without changing the order of
+/// children with common channels. Two layout orders are available:
+/// :attr:`Direction.Backward` and :attr:`Direction.Forward`. The default order
+/// is :attr:`Direction.Backward`.
 ///
-/// Child elements with no common channel are arranged in parallel.
-/// :class:`Barrier` can be used to synchronize multiple channels.
+/// Args:
+///     *children (Element): Child elements.
+///     direction (str | Direction): Layout order. Defaults to 'backward'.
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Stack {
-    /// Sequence[Element]: Child elements.
     children: Vec<Py<Element>>,
 }
 
 #[pymethods]
 impl Stack {
     #[new]
     #[pyo3(signature = (
@@ -1133,14 +1321,30 @@
                 duration,
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
+    /// Create a new stack layout with different children.
+    ///
+    /// Using this method may be more readable than specifying children in the
+    /// constructor.
+    ///
+    /// .. code-block:: python
+    ///
+    ///     stack = Stack(direction='forward').with_children(
+    ///         element1,
+    ///         element2,
+    ///     )
+    ///
+    /// Args:
+    ///     *children (Element): New child elements.
+    /// Returns:
+    ///     Stack: New stack layout.
     #[pyo3(signature=(*children))]
     fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<Element>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let rust_children = children.iter().map(|x| x.get().0.clone()).collect();
         let rust_base = &slf.downcast::<Element>()?.get().0;
         let common = rust_base.common().clone();
         let variant = rust_base
@@ -1155,15 +1359,14 @@
             (
                 Self { children },
                 Element(Arc::new(schedule::Element::new(common, variant))),
             ),
         )
     }
 
-    /// Direction: Direction of arrangement.
     #[getter]
     fn direction(slf: &Bound<'_, Self>) -> PyResult<Direction> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_stack()
@@ -1171,68 +1374,100 @@
                 "Failed to get the stack variant from the element.",
             ))?
             .direction();
         Ok(ret)
     }
 }
 
-/// A child element with an absolute time.
+/// A child element with an absolute time in a absolute layout.
+///
+/// The time of each child element is relative to the start of the absolute
+/// layout.
+///
+/// Args:
+///     time (float): Time relative to the start of the parent element.
+///     element (Element): Child element.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct AbsoluteEntry {
-    /// float: Time relative to the start of the parent element.
     time: f64,
-    /// Element: Child element.
     element: Py<Element>,
 }
 
 #[pymethods]
 impl AbsoluteEntry {
     #[new]
-    fn new(time: f64, element: Py<Element>) -> Self {
-        AbsoluteEntry { time, element }
+    fn new(time: f64, element: Py<Element>) -> PyResult<Self> {
+        if !time.is_finite() {
+            return Err(PyValueError::new_err("Time must be finite"));
+        }
+        Ok(AbsoluteEntry { time, element })
     }
 
     /// Convert the value to AbsoluteEntry.
     ///
     /// the value can be:
+    ///
     /// - AbsoluteEntry
     /// - Element
-    /// - tuple[float, Element]
+    /// - tuple[float, Element]: Time and element.
+    ///
+    /// Args:
+    ///     obj (AbsoluteEntry | Element | tuple[float, Element]): Value to convert.
+    /// Returns:
+    ///     AbsoluteEntry: Converted value.
+    /// Raises:
+    ///     ValueError: If the value cannot be converted.
     #[staticmethod]
     fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(element) = obj.extract() {
-            return Py::new(py, AbsoluteEntry::new(0.0, element));
+            return Py::new(py, AbsoluteEntry::new(0.0, element)?);
         }
         if let Ok((time, element)) = obj.extract() {
-            return Py::new(py, AbsoluteEntry::new(time, element));
+            return Py::new(py, AbsoluteEntry::new(time, element)?);
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to AbsoluteEntry",
         ))
     }
 }
 
 fn extract_absolute_entry(obj: &Bound<'_, PyAny>) -> PyResult<AbsoluteEntry> {
     AbsoluteEntry::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
-/// An absolute schedule element.
+/// An absolute layout element.
 ///
 /// The child elements are arranged in absolute time. The time of each child
 /// element is relative to the start of the absolute schedule. The duration of
 /// the absolute schedule is the maximum end time of the child elements.
+///
+/// The `children` argument can be:
+///
+/// - AbsoluteEntry
+/// - Element
+/// - tuple[float, Element]: Time and element.
+///
+/// Args:
+///     *children (AbsoluteEntry | Element | tuple[float, Element]): Child elements.
+/// Example:
+///     .. code-block:: python
+///
+///         absolute = Absolute(
+///             element1,
+///             (1.0, element2),
+///             AbsoluteEntry(2.0, element3),
+///         )
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Absolute {
-    /// Sequence[AbsoluteEntry]: Child elements.
     children: Vec<AbsoluteEntry>,
 }
 
 #[pymethods]
 impl Absolute {
     #[new]
     #[pyo3(signature = (
@@ -1280,14 +1515,30 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     /// Create a new absolute schedule with different children.
+    ///
+    /// Using this method may be more readable than specifying children in the
+    /// constructor.
+    ///
+    /// .. code-block:: python
+    ///
+    ///     absolute = Absolute(duration=50e-6).with_children(
+    ///         element1,
+    ///         (100e-9, element2),
+    ///     )
+    ///
+    /// Args:
+    ///     *children (AbsoluteEntry | Element | tuple[float, Element]): New
+    ///         child elements.
+    /// Returns:
+    ///     Absolute: New absolute schedule.
     #[pyo3(signature=(*children))]
     fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let children: Vec<_> = children
             .into_iter()
             .map(|x| extract_absolute_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
@@ -1318,66 +1569,75 @@
         )
     }
 }
 
 /// Unit of grid length.
 ///
 /// The unit can be:
+///
 /// - Seconds: Fixed length in seconds.
 /// - Auto: Auto length.
-/// - Star: Ratio of the remaining space.
+/// - Star: Ratio of the remaining duration.
 #[pyclass(frozen)]
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 enum GridLengthUnit {
     Seconds,
     Auto,
     Star,
 }
 
 /// Length of a grid column.
 ///
 /// :class:`GridLength` is used to specify the length of a grid column. The
-/// length can be specified in seconds, as a fraction of the remaining space,
+/// length can be specified in seconds, as a fraction of the remaining duration,
 /// or automatically.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct GridLength {
     value: f64,
     unit: GridLengthUnit,
 }
 
 #[pymethods]
 impl GridLength {
-    #[new]
-    fn new(value: f64, unit: GridLengthUnit) -> Self {
-        GridLength { value, unit }
-    }
-
     /// Create an automatic grid length.
+    ///
+    /// Returns:
+    ///     GridLength: Automatic grid length.
     #[staticmethod]
     fn auto() -> Self {
         GridLength {
             value: 0.0,
             unit: GridLengthUnit::Auto,
         }
     }
 
     /// Create a ratio based grid length.
+    ///
+    /// Args:
+    ///     value (float): Ratio of the remaining duration.
+    /// Returns:
+    ///     GridLength: Ratio based grid length.
     #[staticmethod]
     fn star(value: f64) -> PyResult<Self> {
         if !value.is_finite() || value <= 0.0 {
             return Err(PyValueError::new_err("The value must be greater than 0."));
         }
         Ok(GridLength {
             value,
             unit: GridLengthUnit::Star,
         })
     }
 
     /// Create a fixed grid length.
+    ///
+    /// Args:
+    ///     value (float): Fixed length in seconds.
+    /// Returns:
+    ///     GridLength: Fixed grid length.
     #[staticmethod]
     fn fixed(value: f64) -> PyResult<Self> {
         if !value.is_finite() || value < 0.0 {
             return Err(PyValueError::new_err(
                 "The value must be greater than or equal to 0.",
             ));
         }
@@ -1386,20 +1646,28 @@
             unit: GridLengthUnit::Seconds,
         })
     }
 
     /// Convert the value to GridLength.
     ///
     /// The value can be:
+    ///
     /// - GridLength
     /// - float: Fixed length in seconds.
     /// - 'auto': Auto length.
     /// - 'x*': x stars.
     /// - 'x': Fixed length in seconds.
     /// - '*': 1 star.
+    ///
+    /// Args:
+    ///     obj (GridLength | float | str): Value to convert.
+    /// Returns:
+    ///     GridLength: Converted value.
+    /// Raises:
+    ///     ValueError: If the value cannot be converted.
     #[staticmethod]
     fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(v) = obj.extract() {
@@ -1425,68 +1693,127 @@
     }
 }
 
 fn extract_grid_length(obj: &Bound<'_, PyAny>) -> PyResult<GridLength> {
     GridLength::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
-/// A child element in a grid.
+/// A child element in a grid layout.
+///
+/// Args:
+///     element (Element): Child element.
+///     column (int): Column index.
+///     span (int): Column span.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct GridEntry {
     element: Py<Element>,
     column: usize,
     span: usize,
 }
 
 #[pymethods]
 impl GridEntry {
     #[new]
     #[pyo3(signature = (element, column=0, span=1))]
-    fn new(element: Py<Element>, column: usize, span: usize) -> Self {
-        GridEntry {
+    fn new(element: Py<Element>, column: usize, span: usize) -> PyResult<Self> {
+        if span == 0 {
+            return Err(PyValueError::new_err("The span must be greater than 0."));
+        }
+        Ok(GridEntry {
             element,
             column,
             span,
-        }
+        })
     }
 
     /// Convert the value to GridEntry.
     ///
     /// The value can be:
+    ///
     /// - GridEntry
     /// - Element
     /// - tuple[Element, int]: Element and column.
     /// - tuple[Element, int, int]: Element, column, and span.
+    ///
+    /// Args:
+    ///     obj (GridEntry | Element | tuple[Element, int] | tuple[Element, int, int]): Value to convert.
+    /// Returns:
+    ///     GridEntry: Converted value.
+    /// Raises:
+    ///     ValueError: If the value cannot be converted.
     #[staticmethod]
     fn convert(obj: &Bound<'_, PyAny>) -> PyResult<Py<Self>> {
         let py = obj.py();
         if let Ok(slf) = obj.extract() {
             return Ok(slf);
         }
         if let Ok(element) = obj.extract() {
-            return Py::new(py, GridEntry::new(element, 0, 1));
+            return Py::new(py, GridEntry::new(element, 0, 1)?);
         }
         if let Ok((element, column)) = obj.extract() {
-            return Py::new(py, GridEntry::new(element, column, 1));
+            return Py::new(py, GridEntry::new(element, column, 1)?);
         }
         if let Ok((element, column, span)) = obj.extract() {
-            return Py::new(py, GridEntry::new(element, column, span));
+            return Py::new(py, GridEntry::new(element, column, span)?);
         }
         Err(PyValueError::new_err(
             "Failed to convert the value to GridEntry.",
         ))
     }
 }
 
 fn extract_grid_entry(obj: &Bound<'_, PyAny>) -> PyResult<GridEntry> {
     GridEntry::convert(obj).and_then(|x| x.extract(obj.py()))
 }
 
-/// A grid schedule element.
+/// A grid layout element.
+///
+/// A grid layout has multiple columns and each child element occupies some
+/// columns. The width of each column can be specified by :class:`GridLength`,
+/// which can be:
+///
+/// - Fixed length in seconds.
+/// - Auto length:
+///     The width is determined by the child element.
+///
+/// - Star length:
+///     The width id determined by remaining duration. For example, if there
+///     are two columns with 1* and 2* and the remaining duration is 300 ns,
+///     the width of the columns will be 100 ns and 200 ns.
+///
+/// Columns length can be specified with a simplified syntax:
+///
+/// - 'auto': Auto length.
+/// - 'x*': x stars.
+/// - 'x': Fixed length in seconds.
+/// - '*': 1 star.
+///
+/// If no columns are provided, the grid layout will have one column with '*'.
+///
+/// Children can be provided as:
+///
+/// - GridEntry
+/// - Element: The column index is 0 and the span is 1.
+/// - tuple[Element, int]: Element and column. The span is 1.
+/// - tuple[Element, int, int]: Element, column, and span.
+///
+/// Args:
+///     *children (GridEntry | Element | tuple[Element, int] | tuple[Element, int, int]): Child elements.
+///     columns (Iterable[GridLength | float | str]): Column lengths. Defaults to ['*'].
+/// Example:
+///     .. code-block:: python
+///
+///         grid = Grid(
+///             GridEntry(element1, 0, 1),
+///             (element2, 1),
+///             (element3, 2, 2),
+///             element4,
+///             columns=['auto', '1*', '2'],
+///         )
 #[pyclass(extends=Element, get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Grid {
     children: Vec<GridEntry>,
 }
 
 #[pymethods]
@@ -1545,14 +1872,30 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     /// Create a new grid schedule with different children.
+    ///
+    /// Using this method may be more readable than specifying children in the
+    /// constructor.
+    ///
+    /// .. code-block:: python
+    ///
+    ///     grid = Grid(columns=['auto', '*', 'auto']).with_children(
+    ///         element1,
+    ///         (element2, 2),
+    ///         (element3, 0, 3),
+    ///     )
+    ///
+    /// Args:
+    ///     *children (GridEntry | Element | tuple[Element, int] | tuple[Element, int, int]): New child elements.
+    /// Returns:
+    ///     Grid: New grid schedule.
     #[pyo3(signature=(*children))]
     fn with_children(slf: &Bound<'_, Self>, children: Vec<Py<PyAny>>) -> PyResult<Py<Self>> {
         let py = slf.py();
         let children: Vec<_> = children
             .into_iter()
             .map(|x| extract_grid_entry(&x.into_bound(py)))
             .collect::<PyResult<_>>()?;
@@ -1579,15 +1922,14 @@
             (
                 Self { children },
                 Element(Arc::new(schedule::Element::new(common, variant))),
             ),
         )
     }
 
-    /// Sequence[GridLength]: Column lengths.
     #[getter]
     fn columns(slf: &Bound<'_, Self>) -> PyResult<Vec<GridLength>> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_grid()
@@ -1601,28 +1943,28 @@
 }
 
 /// Generate waveforms from a schedule.
 ///
 /// Args:
 ///     channels (Iterable[Channel]): Information of the channels.
 ///     shapes (Iterable[Shape]): Shapes used in the schedule.
-///     schedule (Element): Schedule to execute.
+///     schedule (Element): Root element of the schedule.
 ///     time_tolerance (float): Tolerance for time comparison. Default is 1e-12.
-///     amp_tolerance (float): Tolerance for amplitude comparison. Default is 0.1 / 2^16.
-///     phase_tolerance (float): Tolerance for phase comparison. Default is 1e-4.
+///     amp_tolerance (float): Tolerance for amplitude comparison. Default is
+///         0.1 / 2^16.
+///     phase_tolerance (float): Tolerance for phase comparison. Default is
+///         1e-4.
 ///     allow_oversize (bool): Allow oversize elements. Default is ``False``.
-///
 /// Returns:
-///     Dict[str, numpy.ndarray]: Waveforms of the channels.
-///
+///     Dict[str, numpy.ndarray]: Waveforms of the channels. The key is the
+///         channel name and the value is the waveform.
 /// Raises:
 ///     ValueError: If some input is invalid.
 ///     TypeError: If some input has an invalid type.
 ///     RuntimeError: If waveform generation fails.
-///
 /// Example:
 ///     .. code-block:: python
 ///
 ///         from bosing import Barrier, Channel, Hann, Play, Stack, generate_waveforms
 ///         channels = [Channel("xy", 30e6, 2e9, 1000)]
 ///         shapes = [Hann()]
 ///         schedule = Stack(duration=500e-9).with_children(
@@ -1682,20 +2024,21 @@
         .into_iter()
         .zip(results)
         .map(|(c, w)| (c.name, PyArray1::from_vec_bound(py, w).unbind()))
         .collect();
     Ok(dict)
 }
 
-/// Generates microwave pulses for superconducting quantum computing experiments.
+/// Generates microwave pulses for superconducting quantum computing
+/// experiments.
 ///
 /// .. caution::
 ///
-///     All phase values are in number of cycles. For example, a phase of
-///     :math:`0.25` means :math:`\\pi/2` radians.
+///     The unit of phase is number of cycles, not radians. For example, a phase
+///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 #[pymodule]
 fn bosing(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<Absolute>()?;
     m.add_class::<AbsoluteEntry>()?;
     m.add_class::<Alignment>()?;
     m.add_class::<Barrier>()?;
     m.add_class::<Channel>()?;
```

### Comparing `bosing-2.0.0b1/src/sampler.rs` & `bosing-2.0.0b2/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/absolute.rs` & `bosing-2.0.0b2/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/grid.rs` & `bosing-2.0.0b2/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/play.rs` & `bosing-2.0.0b2/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/repeat.rs` & `bosing-2.0.0b2/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/simple.rs` & `bosing-2.0.0b2/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule/stack.rs` & `bosing-2.0.0b2/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/schedule.rs` & `bosing-2.0.0b2/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/src/shape.rs` & `bosing-2.0.0b2/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/tests/test_basic.py` & `bosing-2.0.0b2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/Cargo.lock` & `bosing-2.0.0b2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.1"
+version = "2.0.0-beta.2"
 dependencies = [
  "anyhow",
  "bspline",
  "enum_dispatch",
  "float-cmp",
  "itertools",
  "mimalloc",
```

### Comparing `bosing-2.0.0b1/pyproject.toml` & `bosing-2.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b1/PKG-INFO` & `bosing-2.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b1
+Version: 2.0.0b2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

