# Comparing `tmp/ovoenergy-1.3.1.dev0.tar.gz` & `tmp/ovoenergy-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovoenergy-1.3.1.dev0.tar", last modified: Wed Feb  1 22:36:39 2023, max compression
+gzip compressed data, was "ovoenergy-2.0.0.dev0.tar", last modified: Sun Apr 21 11:17:59 2024, max compression
```

## Comparing `ovoenergy-1.3.1.dev0.tar` & `ovoenergy-2.0.0.dev0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/ovoenergy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/ovoenergy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/models/carbon_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/models/footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/ovoenergy/ovoenergy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-01 22:36:39.000000 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-01 22:36:39.000000 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 22:36:39.000000 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-01 22:36:39.000000 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-01 22:36:39.000000 ovoenergy-1.3.1.dev0/ovoenergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 22:36:39.457124 ovoenergy-1.3.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-01 22:36:10.000000 ovoenergy-1.3.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.958370 ovoenergy-2.0.0.dev0/ovoenergy/
+-rw-r--r--   0 runner    (1001) docker     (127)    21944 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/ovoenergy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/ovoenergy/models/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 11:17:59.000000 ovoenergy-2.0.0.dev0/ovoenergy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 11:17:59.962370 ovoenergy-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-21 11:17:38.000000 ovoenergy-2.0.0.dev0/setup.py
```

### Comparing `ovoenergy-1.3.1.dev0/ovoenergy/__main__.py` & `ovoenergy-2.0.0.dev0/ovoenergy/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,152 +1,169 @@
-"""OVO Energy: Main"""
-from __future__ import annotations
+"""Main."""
 
 import asyncio
 from datetime import datetime, timedelta
-from typing import Optional
 
+import aiohttp
 import typer
 
+from . import OVOEnergy
 from ._version import __version__
-from .models import OVODailyUsage, OVOHalfHourUsage
-from .models.carbon_intensity import OVOCarbonIntensity
-from .models.footprint import OVOFootprint
-from .models.plan import OVOPlan
-from .ovoenergy import OVOEnergy
 
 app = typer.Typer()
 loop = asyncio.new_event_loop()
 asyncio.set_event_loop(loop)
 
 
+async def _setup_client(
+    username: str,
+    password: str,
+    account: int | None = None,
+) -> tuple[OVOEnergy, aiohttp.ClientSession]:
+    """Set up OVO Energy client."""
+    client_session = aiohttp.ClientSession()
+    client = OVOEnergy(
+        client_session=client_session,
+    )
+
+    if not await client.authenticate(username, password):
+        typer.secho("Authentication failed", fg=typer.colors.RED)
+        raise typer.Abort()
+
+    await client.bootstrap_accounts()
+
+    if account is not None:
+        client.custom_account_id = account
+
+    return (client, client_session)
+
+
 @app.command(name="daily", short_help="Get daily usage from OVO Energy")
 def daily(
     username: str = typer.Option(..., help="OVO Energy username"),
     password: str = typer.Option(..., help="OVO Energy password"),
-    account: str = typer.Option(None, help="OVO Energy account number"),
-    date: str = typer.Option(None, help="Date to retrieve data for"),
+    account: int = typer.Option(
+        None, help="OVO Energy account number (default: first account)"
+    ),
+    date: str = typer.Option(
+        None, help="Date to retrieve data for (default: this month)"
+    ),
 ) -> None:
     """Get daily usage from OVO Energy."""
     if date is None:
         # Get this month
         date = datetime.now().strftime("%Y-%m")
 
-    ovo_usage: Optional[OVODailyUsage] = None
-
-    client = OVOEnergy()
-
-    authenticated = loop.run_until_complete(
-        client.authenticate(username, password, account)
+    [client, client_session] = loop.run_until_complete(
+        _setup_client(username, password, account)
     )
-    if authenticated:
-        ovo_usage = loop.run_until_complete(client.get_daily_usage(date))
+    ovo_usage = loop.run_until_complete(client.get_daily_usage(date))
 
     typer.secho(
-        ovo_usage.json() if ovo_usage is not None else '{"message": "No data"}',
+        ovo_usage if ovo_usage is not None else '{"message": "No data"}',
         fg=typer.colors.GREEN,
     )
+    loop.run_until_complete(client_session.close())
 
 
 @app.command(name="halfhourly", short_help="Get half hourly usage from OVO Energy")
 def half_hourly(
     username: str = typer.Option(..., help="OVO Energy username"),
     password: str = typer.Option(..., help="OVO Energy password"),
-    account: str = typer.Option(None, help="OVO Energy account number"),
-    date: str = typer.Option(None, help="Date to retrieve data for"),
+    account: int = typer.Option(
+        None, help="OVO Energy account number (default: first account)"
+    ),
+    date: str = typer.Option(
+        None, help="Date to retrieve data for (default: this month)"
+    ),
 ) -> None:
     """Get half hourly usage from OVO Energy."""
     if date is None:
         # Get yesterday's date
         date = (datetime.now() - timedelta(days=1)).strftime("%Y-%m-%d")
 
-    ovo_usage: Optional[OVOHalfHourUsage] = None
-
-    client = OVOEnergy()
-    authenticated = loop.run_until_complete(
-        client.authenticate(username, password, account)
+    [client, client_session] = loop.run_until_complete(
+        _setup_client(username, password, account)
     )
-    if authenticated:
-        ovo_usage = loop.run_until_complete(client.get_half_hourly_usage(date))
+    ovo_usage = loop.run_until_complete(client.get_half_hourly_usage(date))
 
     typer.secho(
-        ovo_usage.json() if ovo_usage is not None else '{"message": "No data"}',
+        ovo_usage if ovo_usage is not None else '{"message": "No data"}',
         fg=typer.colors.GREEN,
     )
+    loop.run_until_complete(client_session.close())
 
 
-@app.command(name="plan", short_help="Get plan from OVO Energy")
-def plan(
+@app.command(name="plans", short_help="Get plans from OVO Energy")
+def plans(
     username: str = typer.Option(..., help="OVO Energy username"),
     password: str = typer.Option(..., help="OVO Energy password"),
-    account: str = typer.Option(None, help="OVO Energy account number"),
+    account: int = typer.Option(
+        None, help="OVO Energy account number (default: first account)"
+    ),
 ) -> None:
     """Get rates from OVO Energy."""
-    ovo_plan: Optional[OVOPlan] = None
-
-    client = OVOEnergy()
-    authenticated = loop.run_until_complete(
-        client.authenticate(username, password, account)
+    [client, client_session] = loop.run_until_complete(
+        _setup_client(username, password, account)
     )
-    if authenticated:
-        ovo_plan = loop.run_until_complete(client.get_plan())
+
+    ovo_plans = loop.run_until_complete(client.get_plans())
 
     typer.secho(
-        ovo_plan.json() if ovo_plan is not None else '{"message": "No data"}',
+        ovo_plans if ovo_plans is not None else '{"message": "No data"}',
         fg=typer.colors.GREEN,
     )
+    loop.run_until_complete(client_session.close())
 
 
 @app.command(name="carbon-footprint", short_help="Get carbon footprint from OVO Energy")
 def carbon_footprint(
     username: str = typer.Option(..., help="OVO Energy username"),
     password: str = typer.Option(..., help="OVO Energy password"),
-    account: str = typer.Option(None, help="OVO Energy account number"),
+    account: int = typer.Option(
+        None, help="OVO Energy account number (default: first account)"
+    ),
 ) -> None:
     """Get carbon footprint from OVO Energy."""
-    ovo_footprint: Optional[OVOFootprint] = None
-
-    client = OVOEnergy()
-    authenticated = loop.run_until_complete(
-        client.authenticate(username, password, account)
+    [client, client_session] = loop.run_until_complete(
+        _setup_client(username, password, account)
     )
-    if authenticated:
-        ovo_footprint = loop.run_until_complete(client.get_footprint())
+    ovo_footprint = loop.run_until_complete(client.get_footprint())
 
     typer.secho(
-        ovo_footprint.json() if ovo_footprint is not None else '{"message": "No data"}',
+        ovo_footprint if ovo_footprint is not None else '{"message": "No data"}',
         fg=typer.colors.GREEN,
     )
+    loop.run_until_complete(client_session.close())
 
 
 @app.command(name="carbon-intensity", short_help="Get carbon intensity from OVO Energy")
 def carbon_intensity(
     username: str = typer.Option(..., help="OVO Energy username"),
     password: str = typer.Option(..., help="OVO Energy password"),
-    account: str = typer.Option(None, help="OVO Energy account number"),
+    account: int = typer.Option(
+        None, help="OVO Energy account number (default: first account)"
+    ),
 ) -> None:
     """Get carbon intensity from OVO Energy."""
-    ovo_carbon_intensity: Optional[OVOCarbonIntensity] = None
-
-    client = OVOEnergy()
-    authenticated = loop.run_until_complete(
-        client.authenticate(username, password, account)
+    [client, client_session] = loop.run_until_complete(
+        _setup_client(username, password, account)
     )
-    if authenticated:
-        ovo_carbon_intensity = loop.run_until_complete(client.get_carbon_intensity())
+    ovo_carbon_intensity = loop.run_until_complete(client.get_carbon_intensity())
 
     typer.secho(
-        ovo_carbon_intensity.json()
+        ovo_carbon_intensity
         if ovo_carbon_intensity is not None
         else '{"message": "No data"}',
         fg=typer.colors.GREEN,
     )
+    loop.run_until_complete(client_session.close())
 
 
 @app.command(name="version", short_help="Module Version")
 def version() -> None:
-    """Module Version"""
+    """Display module version."""
     typer.secho(__version__.public(), fg=typer.colors.CYAN)
 
 
 if __name__ == "__main__":
     app()
```

