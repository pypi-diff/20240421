# Comparing `tmp/darkgray_dev_tools-0.0.2.tar.gz` & `tmp/darkgray_dev_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darkgray_dev_tools-0.0.2.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "darkgray_dev_tools-0.1.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `darkgray_dev_tools-0.0.2.tar` & `darkgray_dev_tools-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1171 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      111 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/__init__.py
--rw-r--r--   0        0        0     1322 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/changelog.py
--rwxr-xr-x   0        0        0     3194 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/darkgray_bump_version.py
--rw-r--r--   0        0        0    17823 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/darkgray_update_contributors.py
--rw-r--r--   0        0        0     3138 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/exceptions.py
--rw-r--r--   0        0        0     2197 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/milestones.py
--rw-r--r--   0        0        0      787 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/package_metadata.py
--rw-r--r--   0        0        0    10046 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/version_replace.py
--rw-r--r--   0        0        0     1930 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/versions.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 darkgray_dev_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      111 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/__init__.py
+-rw-r--r--   0        0        0     1322 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/changelog.py
+-rwxr-xr-x   0        0        0     3194 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/darkgray_bump_version.py
+-rw-r--r--   0        0        0    18698 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/darkgray_update_contributors.py
+-rw-r--r--   0        0        0     1579 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/exceptions.py
+-rw-r--r--   0        0        0     2197 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/milestones.py
+-rw-r--r--   0        0        0      787 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/package_metadata.py
+-rw-r--r--   0        0        0    10046 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/version_replace.py
+-rw-r--r--   0        0        0     1930 1980-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/versions.py
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 darkgray_dev_tools-0.1.0/PKG-INFO
```

### Comparing `darkgray_dev_tools-0.0.2/pyproject.toml` & `darkgray_dev_tools-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 [project]
 name = "darkgray_dev_tools"
 authors = [{name = "Antti Kaihola", email = "13725+akaihola@users.noreply.github.com"}]
 dynamic = ["version", "description"]
 dependencies = [
     "airium>=0.2.3",
     "click>=8.0.0",
-    "defusedxml>=0.7.1",
     "pyproject-parser",
     "requests_cache>=0.7",
     "ruamel.yaml>=0.15.78",
     "setuptools>=61",
 ]
 
 [project.urls]
 Home = "https://github.com/akaihola/darkgray-dev-tools"
 
 [project.scripts]
 darkgray_bump_version = "darkgray_dev_tools.darkgray_bump_version:bump_version"
-darkgray_verify_contributors = "darkgray_dev_tools.darkgray_update_contributors:verify"
 darkgray_update_contributors = "darkgray_dev_tools.darkgray_update_contributors:update"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/changelog.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/changelog.py`

 * *Files identical despite different names*

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/darkgray_bump_version.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/darkgray_bump_version.py`

 * *Files identical despite different names*

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/darkgray_update_contributors.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/darkgray_update_contributors.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,100 +3,59 @@
 Usage::
 
     pip install darkgray-dev-tools
     darkgray-update-contributors \
         --token=<ghp_your_github_token> \
         --modify-readme \
         --modify-contributors
-    darkgray-verify-contributors
 
 """
 
 # pylint: disable=too-few-public-methods,abstract-method
 
 from __future__ import annotations
 
-import re
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from functools import lru_cache, total_ordering
 from itertools import groupby
 from pathlib import Path
 from subprocess import run
 from textwrap import dedent, indent
-from typing import TYPE_CHECKING, Any, Iterable, MutableMapping, TypedDict, cast
-from xml.etree import ElementTree  # nosec
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    MutableMapping,
+    Protocol,
+    TypedDict,
+    cast,
+)
+from urllib.parse import urlencode, urljoin
 
 import click
-import defusedxml.ElementTree
 from airium import Airium
 from requests import codes
 from requests_cache.session import CachedSession
 from ruamel.yaml import YAML
 
 from darkgray_dev_tools.exceptions import (
     GitHubApiError,
     GitHubApiNotFoundError,
     GitHubRepoNameError,
-    InvalidGitHubUrlError,
-    SectionNotFoundError,
-    WrongContributionTypeError,
 )
 
 if TYPE_CHECKING:
     from requests.models import Response
 
 
 @click.group()
 def cli() -> None:
     """Create the main command group for command line parsing."""
 
 
-def _load_contributor_table(path: Path) -> ElementTree.Element:
-    """Load and parse the HTML contributor table as seen in ``README.rst``.
-
-    :param path: Path to ``README.rst``
-    :return: The parsed HTML as an element tree
-
-    """
-    readme = Path(path).read_text(encoding="utf-8")
-    match = re.search(r"<table>.*</table>", readme, re.DOTALL)
-    if not match:
-        section = "contributors HTML table"
-        raise SectionNotFoundError(section, "README.rst")
-    contributor_table = match.group(0)
-    contributor_table = contributor_table.replace("&", "&amp;")
-    try:
-        return cast(
-            ElementTree.Element, defusedxml.ElementTree.fromstring(contributor_table)
-        )
-    except ElementTree.ParseError as exc_info:
-        linenum, column = exc_info.position
-        line = contributor_table.splitlines()[linenum - 1]
-        click.echo(line, err=True)
-        click.echo((column - 1) * " ", nl=False, err=True)
-        click.echo("^", err=True)
-        raise
-
-
-def verify_contribution_type(url: str, contribution_type: str, *args: str) -> None:
-    """Raise an exception if the contribution type for the URL isn't valid.
-
-    :param url: The URL of the search for the author's contributions
-    :param contribution_type: The name of the contribution type
-    :param args: Valid contribution types for this type of URL path
-    :raises RuntimeError: Raised if the contribution type isn't valid
-
-    """
-    valid_contribution_types = args
-    if contribution_type not in valid_contribution_types:
-        raise WrongContributionTypeError(
-            url, contribution_type, valid_contribution_types
-        )
-
-
 @lru_cache(maxsize=1)
 def get_github_repository() -> str:
     """Get the name of the GitHub repository from the current directory.
 
     :return: The name of the GitHub repository, including the owner
 
     """
@@ -131,77 +90,153 @@
         ["Code"],
         "conda-issues",
     ),
     "conda-forge/{repo_name}-feedstock/search?q=": (["Code"], "feedstock-issues"),
 }
 
 
-@cli.command()
-def verify() -> None:
-    """Verify generated contributor table HTML in ``README.rst``.
+@dataclass
+class FormatAndJoin:
+    """Format a delimited list from the given key in the keyword arguments.
+
+    >>> fmt = FormatAndJoin(" OR ", "repos", "repo:{}")
+    >>> print(fmt.format(repos=["me/repo1", "me.repo2"]))
+    repo:me/repo1 OR repo:me.repo2
+
+    """
+
+    sep: str
+    key: str
+    fmt: str
+
+    def format(self, **kwargs: list[SupportsFormat]) -> str:
+        """Emulate the `str.format` method.
+
+        :param kwargs: The keyword arguments, containing the key to get the list of
+                       items from
+        :return: A string with the formatted items joined by the separator
+
+        """
+        items = kwargs[self.key]
+        formatted_items = (self.fmt.format(item) for item in items)
+        return self.sep.join(formatted_items)
+
+
+class SupportsFormat(Protocol):
+    """Protocol for objects that support a `str.format` like formatting method.
+
+    This is used only for type checking with Mypy.
+
+    """
+
+    def format(self, **kwargs: Any) -> str:  # type: ignore[misc]  # noqa: ANN401
+        """Signature for the ``format`` method."""
+
+
+class UrlPath:
+    """A URL path with query parameters as lists of format strings.
 
-    Output the corresponding YAML source.
+    >>> p = UrlPath(
+    ...     "search",
+    ...     q=[FormatAndJoin(" ", "repos", "repo:{}"), " who:me"],
+    ...     type=["issues"]
+    ... )
+    >>> print(p.render("https://github.com", repos=["me/repo1", "me/repo2"]))
+    https://github.com/search?q=repo%3Ame%2Frepo1+repo%3Ame%2Frepo2+who%3Ame&type=issues
 
     """
-    repo = get_github_repository()
-    repo_name = repo.split("/")[1]
-    users = {}
-    for td_user in _load_contributor_table(Path("README.rst")).findall("tr/td"):
-        profile_link = td_user[0]
-        username = profile_link.attrib["href"].rsplit("/", 1)[-1]
-        avatar_alt = profile_link[0].attrib["alt"]
-        if username != avatar_alt[1:]:
-            click.echo(f"@{username} != {avatar_alt}")
-        contributions = []
-        for contribution_link in td_user.findall("a")[1:]:
-            url = contribution_link.attrib["href"]
-            if not url.startswith("https://github.com/"):
-                raise InvalidGitHubUrlError(url)
-            path = url[19:]
-            contribution_type = contribution_link.attrib["title"]
-            for path_pattern, (
-                valid_types,
-                link_type,
-            ) in CONTRIBUTION_TYPE_VERIFICATION.items():
-                if path.startswith(path_pattern.format(repo=repo, repo_name=repo_name)):
-                    verify_contribution_type(url, contribution_type, *valid_types)
-                    contributions.append(
-                        {"type": contribution_type, "link_type": link_type}
-                    )
-                    break
-            else:
-                raise AssertionError((username, path, contribution_type))
-        users[username] = contributions
-    yaml = YAML(typ="safe", pure=True)
-    click.echo(yaml.dump(users))
+
+    def __init__(self, path: str, **query_params: list[SupportsFormat]) -> None:
+        """Create a new URL path with query parameters.
+
+        :param path: The URL path, e.g. ``search``
+        :param query_params: Query parameters as lists of format strings
+
+        """
+        self.path = path
+        self.query_params = query_params
+
+    def render(  # type: ignore[misc]
+        self, base_url: str, **kwargs: Any  # noqa: ANN401
+    ) -> str:
+        """Render the URL path with the given keyword arguments.
+
+        :param base_url: The base URL path, e.g. ``https://github.com/``
+        :param kwargs: The keyword arguments to format the query parameters with
+        :return: The rendered URL path
+
+        """
+        path = urljoin(base_url, self.path)
+        query_params = [
+            (key, "".join(part.format(**kwargs) for part in fmt))
+            for key, fmt in self.query_params.items()
+        ]
+        encoded_query_params = urlencode(query_params)
+        return f"{path}?{encoded_query_params}"
 
 
 CONTRIBUTION_SYMBOLS = {
     "Bug reports": "🐛",
     "Code": "💻",
     "Documentation": "📖",
     "Reviewed Pull Requests": "👀",
     "Answering Questions": "💬",
     "Maintenance": "🚧",
 }
 CONTRIBUTION_LINKS = {
-    "issues": "{repo}/issues?q=author%3A{{username}}",
-    "commits": "{repo}/commits?author={{username}}",
-    "pulls-reviewed": "{repo}/pulls?q=is%3Apr+reviewed-by%3A{{username}}",
-    "pulls-author": "{repo}/pulls?q=is%3Apr+author%3A{{username}}",
-    "search": "{repo}/search?q={{username}}",
-    "search-comments": "{repo}/search?q=commenter%3A{{username}}&type=issues",
-    "search-discussions": "{repo}/discussions?discussions_q=author%3A{{username}}",
-    "conda-issues": (
-        "conda-forge/staged-recipes/search"
-        "?q={repo_name}&type=issues&author={{username}}"
-    ),
-    "feedstock-issues": (
-        "conda-forge/{repo_name}-feedstock/search"
-        "?q={repo_name}+author%3A{{username}}&type=issues"
+    "issues": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " author:{username}"],
+        type=["issues"],
+    ),
+    "commits": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " author:{username}"],
+        type=["commits"],
+    ),
+    "pulls-reviewed": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " reviewed-by:{username}"],
+        type=["pullrequests"],
+    ),
+    "pulls-author": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " author:{username}"],
+        type=["pullrequests"],
+    ),
+    "search": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " {username}"],
+    ),
+    "search-comments": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " commenter:{username}"],
+        type=["issues"],
+    ),
+    "search-discussions": UrlPath(
+        "search",
+        q=[FormatAndJoin(" ", "repos", "repo:{}"), " involves:{username}"],
+        type=["discussions"],
+    ),
+    "conda-issues": UrlPath(
+        "search",
+        q=[
+            "repo:conda-forge/staged-recipes ",
+            FormatAndJoin(" OR ", "repos", "{}"),
+            " involves:{username}",
+        ],
+        type=["pullrequests"],
+    ),
+    "feedstock-issues": UrlPath(
+        "search",
+        q=[
+            FormatAndJoin(" OR ", "repo_names", "repo:conda-forge/{}-feedstock"),
+            " involves:{username}",
+        ],
+        type=["issues"],
     ),
 }
 
 
 class GitHubSession(CachedSession):
     """Caching HTTP request session with useful defaults.
 
@@ -274,50 +309,74 @@
     These contributor lists are generated based on ``contributors.yaml``.
 
     :param token: The GitHub authorization token for avoiding throttling
 
     """
     with Path("contributors.yaml").open(encoding="utf-8") as yaml_file:
         yaml = YAML(typ="safe", pure=True)
+        *configs, contributors_src = yaml.load_all(yaml_file)
+        if len(configs) > 1:
+            message = "Too many YAML documents in contributors.yaml"
+            raise ValueError(message)
+        config = Configuration(**(configs[0] if configs else {}))
         users_and_contributions: dict[str, list[Contribution]] = {
             login: [Contribution(**c) for c in contributions]
-            for login, contributions in yaml.load(yaml_file).items()
+            for login, contributions in contributors_src.items()
         }
     session = GitHubSession(token)
     users = join_github_users_with_contributions(users_and_contributions, session)
-    doc = render_html(users)
+    doc = render_html(users, config)
     click.echo(doc)
     contributor_list = render_contributor_list(users)
     contributors_text = "\n".join(sorted(contributor_list, key=lambda s: s.lower()))
     click.echo(contributors_text)
     if modify_readme:
         write_readme(doc)
     if modify_contributors:
         write_contributors(contributors_text)
 
 
+def get_cwd_repository() -> list[str]:
+    """Get the GitHub repository name from the current working directory.
+
+    :return: The GitHub repository name
+
+    """
+    return [get_github_repository()]
+
+
+@dataclass
+class Configuration:
+    """Configuration for updating contributors."""
+
+    repositories: list[str] = field(default_factory=get_cwd_repository)
+
+
 @dataclass
 class Contribution:
     """A type of contribution from a user."""
 
     type: str
     link_type: str
 
-    def github_search_link(self, login: str) -> str:
+    def github_search_link(self, login: str, config: Configuration) -> str:
         """Return a link to a GitHub search for a user's contributions.
 
         :param login: The GitHub username for the user
+        :param config: Configuration for updating contributors
         :return: A URL link to a GitHub search
 
         """
-        link_template = CONTRIBUTION_LINKS[self.link_type].format(
-            repo=get_github_repository(),
-            repo_name=get_github_repository().split("/")[1],
+        contribution_link = CONTRIBUTION_LINKS[self.link_type]
+        return contribution_link.render(
+            "https://github.com/",
+            repos=config.repositories,
+            repo_names=[repo.split("/")[1] for repo in config.repositories],
+            username=login,
         )
-        return f"https://github.com/{link_template}".format(username=login)
 
 
 class GitHubUser(TypedDict):
     """User record as returned by GitHub API ``/users/`` endpoint."""
 
     id: int
     name: str | None
@@ -429,18 +488,19 @@
     )
     return [
         [user for _, user in rownum_and_users]
         for _, rownum_and_users in users_and_contributions_by_row
     ]
 
 
-def render_html(users: list[Contributor]) -> Airium:
+def render_html(users: list[Contributor], config: Configuration) -> Airium:
     """Convert users and contributions into an HTML table for ``README.rst``.
 
     :param users: GitHub user records and the users' contributions to the repository
+    :param config: Configuration for updating contributors
     :return: An Airium document describing the HTML table
 
     """
     doc = Airium()
     rows_of_users: list[list[Contributor]] = make_rows(users, columns=6)
     with doc.table():
         for row_of_users in rows_of_users:
@@ -454,15 +514,17 @@
                                 alt=f"@{user.login}",
                             )
                             doc.br()
                             doc.sub().b(_t=user.display_name)
                         doc.br()
                         for contribution in user.contributions:
                             doc.a(
-                                href=contribution.github_search_link(user.login),
+                                href=contribution.github_search_link(
+                                    user.login, config
+                                ),
                                 title=contribution.type,
                                 _t=CONTRIBUTION_SYMBOLS[contribution.type],
                             )
     return doc
 
 
 def render_contributor_list(users: Iterable[Contributor]) -> list[str]:
```

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/exceptions.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,50 +19,14 @@
         :param regex: The regular expression that couldn't be found
         :param path: The path of the file in which the regex couldn't be found
 
         """
         super().__init__(f"Can't find `{regex}` in `{path}`")
 
 
-class SectionNotFoundError(Exception):
-    """Raised if an expected text section can't be found in a text file."""
-
-    def __init__(self, section: str, filename: str) -> None:
-        """Initialize the exception.
-
-        :param section: The name of the section which was not found.
-        :param filename: The name of the file in which the section couldn't be found
-
-        """
-        super().__init__(f"No {section} could be found in `{filename}`")
-
-
-class WrongContributionTypeError(Exception):
-    """Raised if verification finds a mismatching URL and contribution type."""
-
-    def __init__(
-        self,
-        url: str,
-        contribution_type: str,
-        valid_contribution_types: tuple[str, ...],
-    ) -> None:
-        """Initialize the exception.
-
-        :param url: The link to a GitHub search
-        :param contribution_type: The type of contribution to be found in search results
-        :param valid_contribution_types: Contribution types which can appear in the
-                                         search results
-
-        """
-        super().__init__(
-            f"Contribution type for {url} was {contribution_type}, "
-            f"expected {valid_contribution_types}"
-        )
-
-
 class GitHubRepoNameError(Exception):
     """Raised if ``git remote get-url`` fails & repository name can't be determined."""
 
     def __init__(self, cwd: Path) -> None:
         """Initialize the exception.
 
         :param cwd: The directory in which Git was run
@@ -70,26 +34,14 @@
         """
         super().__init__(
             f"Could not run Git to determine the name of the GitHub repository for "
             f"the working directory in {cwd}"
         )
 
 
-class InvalidGitHubUrlError(Exception):
-    """Raised if a contribution link doesn't point to GitHub."""
-
-    def __init__(self, url: str) -> None:
-        """Initialize the exception.
-
-        :param url: A link to search results for contributions of a contributor
-
-        """
-        super().__init__(f"{url} is not a valid GitHub URL")
-
-
 class GitHubApiNotFoundError(Exception):
     """Raised when a GitHub API resource is not found."""
 
 
 class GitHubApiError(Exception):
     """Raised when a GitHub API resource returns a non-OK response."""
```

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/milestones.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/milestones.py`

 * *Files identical despite different names*

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/package_metadata.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/package_metadata.py`

 * *Files identical despite different names*

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/version_replace.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/version_replace.py`

 * *Files identical despite different names*

### Comparing `darkgray_dev_tools-0.0.2/src/darkgray_dev_tools/versions.py` & `darkgray_dev_tools-0.1.0/src/darkgray_dev_tools/versions.py`

 * *Files identical despite different names*

