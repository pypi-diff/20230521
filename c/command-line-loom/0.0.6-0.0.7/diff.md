# Comparing `tmp/command_line_loom-0.0.6.tar.gz` & `tmp/command_line_loom-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_line_loom-0.0.6.tar", max compression
+gzip compressed data, was "command_line_loom-0.0.7.tar", max compression
```

## Comparing `command_line_loom-0.0.6.tar` & `command_line_loom-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.6/LICENSE
--rw-r--r--   0        0        0     1815 2023-05-20 13:04:32.039784 command_line_loom-0.0.6/README.md
--rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.6/cll/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.6/cll/__main__.py
--rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.6/cll/app.py
--rw-r--r--   0        0        0     7379 2023-05-20 13:02:49.604384 command_line_loom-0.0.6/cll/config.py
--rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.6/cll/data_structs/__init__.py
--rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.6/cll/data_structs/data_structs.py
--rw-r--r--   0        0        0     9817 2023-05-19 21:14:40.199467 command_line_loom-0.0.6/cll/data_structs/loom_index.py
--rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.6/cll/data_structs/node.py
--rwxr-xr-x   0        0        0     4133 2023-05-20 12:28:46.515322 command_line_loom-0.0.6/cll/encoder.py
--rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.6/cll/io.py
--rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.6/cll/store.py
--rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.6/cll/templater.py
--rw-r--r--   0        0        0    15810 2023-05-20 12:56:46.502548 command_line_loom-0.0.6/cll/tree.py
--rw-r--r--   0        0        0     1052 2023-05-20 13:04:42.115725 command_line_loom-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 command_line_loom-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1899 2023-05-21 13:57:05.105476 command_line_loom-0.0.7/README.md
+-rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.7/cll/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/__main__.py
+-rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.7/cll/app.py
+-rw-r--r--   0        0        0     7381 2023-05-20 21:23:31.452227 command_line_loom-0.0.7/cll/config.py
+-rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/data_structs/__init__.py
+-rw-r--r--   0        0        0    13252 2023-05-21 13:07:37.864187 command_line_loom-0.0.7/cll/data_structs/data_structs.py
+-rw-r--r--   0        0        0    11176 2023-05-21 13:19:09.623216 command_line_loom-0.0.7/cll/data_structs/loom_index.py
+-rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.7/cll/data_structs/node.py
+-rwxr-xr-x   0        0        0     4162 2023-05-21 14:03:25.003785 command_line_loom-0.0.7/cll/encoder.py
+-rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.7/cll/io.py
+-rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.7/cll/store.py
+-rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.7/cll/templater.py
+-rw-r--r--   0        0        0    19070 2023-05-21 14:09:35.940621 command_line_loom-0.0.7/cll/tree.py
+-rw-r--r--   0        0        0     1052 2023-05-21 14:17:02.082261 command_line_loom-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 command_line_loom-0.0.7/PKG-INFO
```

### Comparing `command_line_loom-0.0.6/LICENSE` & `command_line_loom-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/README.md` & `command_line_loom-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 poetry install
 ```
 
 ## Usage
 
 Should be self-documenting in the interface. Just type 'help'.
 
+Some node manipulation: [vid](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)
+
 Watch this for more advanced usage: [vid](https://asciinema.org/a/tLpxm9FdW6gKdJztRnAPAOl7X).
 
 ## Configuration
 
 Before using Command Line Loom, you need to set up a configuration file. This should happen automatically when you run the `cll` command for the first time.
 
 This will create a configuration file in your home directory. See the documentation for each model to learn how to obtain an API key.
```

### Comparing `command_line_loom-0.0.6/cll/__main__.py` & `command_line_loom-0.0.7/cll/__main__.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/app.py` & `command_line_loom-0.0.7/cll/app.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/config.py` & `command_line_loom-0.0.7/cll/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         if default:
             config._dict["chat_name"] = default
 
         if toggle or config._dict["chat_name"]:
             config.save()
 
         if config._dict["file"]:
-            print(f"File mode is on. Using {config._dict['chat_name']} as the chat history file.")
+            print(f"File mode is on. Using '{config._dict['chat_name']}' as the chat history file.")
         else:
             print("File mode is off.")
 
 
 cli = make_typer_shell(
     prompt="📜: ",
     intro="Welcome to the Config! Type help or ? to list commands."
```

### Comparing `command_line_loom-0.0.6/cll/data_structs/data_structs.py` & `command_line_loom-0.0.7/cll/data_structs/data_structs.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,23 +109,51 @@
             self.add_node(node)
         if node.index in self.root_nodes:
             raise ValueError(
                 "Cannot add a new root node with the same index as an existing root node."
             )
         self._root_nodes.append(node.index)
 
+    def delete(self, node: Node, all: bool = False) -> None:
+        """Delete a node. If the node has children, reassign them to the parent, unless 'all' is set."""
+        parent = self.get_parent(node)
+        if not all:
+            self.foster(node, parent)
+        if node.index in self.root_nodes:
+            self._root_nodes.remove(node.index)
+        parent = self.get_parent(node)
+        if parent is not None:
+            parent.child_indices.remove(node.index)
+        if all:
+            for child in self.get_all_children(node).values():
+                del self.all_nodes[child.index]
+                print(f"Deleted node {child.index}.")
+        del self.all_nodes[node.index]
+        print(f"Deleted node {node.index}.")
+
+    def foster(self, parent: Node, new_parent: Optional[Node] = None) -> None:
+        """Foster the children of a node to a new parent. If no parent, make them root nodes."""
+        children = self.get_children(parent)
+        for child in children.values():
+            if new_parent is None:
+                self._root_nodes.append(child.index)
+            else:
+                new_parent.child_indices.add(child.index)
+        parent.child_indices = set()
+        print(f"Hoisted {[child.index for child in children.values()]} to {new_parent.index}")
+
     def get_children(self, parent_node: Optional[Node]) -> Dict[int, Node]:
         """Get nodes given indices."""
         if parent_node is None:
             return self.root_nodes
         else:
             return {i: self.all_nodes[i] for i in parent_node.child_indices}
 
     def get_all_children(self, parent_node: Optional[Node], all_children=None) -> Dict[int, Node]:
-        """Get all children."""
+        """Get all descendent nodes."""
         all_children = all_children or {}
         children = self.get_children(parent_node)
         for child_node in children.values():
             all_children[child_node.index] = child_node
             self.get_all_children(child_node, all_children)
         return all_children
 
@@ -202,44 +230,51 @@
         """Get path to root of the tree."""
         path = path.append(node) if path is not None else [node]
         parent_node = self.get_parent(node)
         if parent_node is None:
             return path
         return self.get_path_to_root(parent_node, path)
 
-    def _get_graph(self) -> None:
+    def _get_graph(self, node: Optional[Node] = None) -> None:
+        if node is None:
+            node = self.all_nodes[self.active_root]
         g = nx.Graph()
 
         # add nodes
-        for node in self.active_tree.values():
+        active_nodes = self.get_all_children(node)
+        active_nodes.update({node.index: node})
+        for node in active_nodes.values():
             g.add_node(node.index)
 
         # add edges
-        for node in self.active_tree.values():
+        for node in active_nodes.values():
             children = self.get_children(node)
             for _, child in children.items():
                 g.add_edge(child.index, node.index)
 
         self.graph = g
         return self.graph
 
-    def _get_distances(self) -> None:
-        self._get_graph()
+    def _get_distances(self, node: Optional[Node] = None) -> None:
+        self._get_graph(node)
         self.distances = {}
         for u in self.graph.nodes:
             for v in self.graph.nodes:
                 self.distances[tuple({u, v})] = nx.shortest_path_length(self.graph, u, v)
 
     def get_distance_from_path(self, query_index) -> int:
         distance = float('inf')
         for index in self.path_indices:
             distance = min(distance, self.distances[tuple({index, query_index})])
         return distance
 
-    def close_node(self, query_index, head_index) -> Tuple[int, bool]:
+    def close_node(self, query_index, head_index: Optional[int] = None) -> Tuple[int, bool]:
+        if head_index is None:
+            return 0, True
+
         # Close to path?
         distance = self.get_distance_from_path(query_index)
         if distance < self.path_neighborhood:
             return distance, True
 
         # Close to head?
         distance = self.distances[tuple({query_index, head_index})]
@@ -258,60 +293,61 @@
 
     # Print Representation
     def _root_info(self) -> str:
         _str = "\n# Root Node Index (branches:total_nodes)) #\n"
         for root in self.root_nodes.values():
             leaves = self.get_leaves(root)
             children = self.get_all_children(root)
-            _str += f"{root.index}; ({len(leaves)}:{len(children)}):\t\t{root.text.splitlines()[0]}"
+            _str += f"{root.index}:\t(branches:{len(leaves)}, nodes:{len(children)}):\t{root.text.splitlines()[0]}"
             if self.all_nodes[root.index].node_info.get("checked_out", False):
                 _str += "\t\t<-- CURRENT_ROOT"
-        print(Panel(_str, title="Root Nodes"))
+            _str += "\n"
+        print(Panel(_str, title="Root Nodes", style="bold blue"))
 
     def legend(self) -> str:
         txt = (
             "checked out nodes are in [bold red]bold red[/bold red]\n"
             "other nodes are in [dim blue]dim blue[/dim blue]\n"
             "navigate with [magenta]hjkl[/magenta]\n"
-            "show the current prompt with [magenta]p[/magenta]\n"
             "show the tree with [magenta]t[/magenta]\n"
-            "(this will be the checked out path plus template)"
         )
         print(Panel.fit(txt, title="Legend", border_style="bold magenta"))
 
     def get_full_repr(self, summaries=False) -> str:
         uber_root = Node(
             index=-1,
             text="(displaying all nodes)",
             child_indices=self._root_nodes,
             node_info={"checked_out": True},
         )
         self.legend()
         self._root_info()
         return self._get_repr(uber_root)
 
-    def _get_repr(self, node: Optional[Node] = None) -> str:
+    def _get_repr(self, node: Optional[Node] = None, full: bool = True) -> str:
         if node is None:
             if self.path_indices:
                 node = self.all_nodes[self.path_indices[0]]
             elif len(self.all_nodes):
                 node = self.all_nodes[min(self.all_nodes.keys())]
             else:
                 return
         tree = RichTree(self._text(node), style="bold red", guide_style="bold magenta")
-        self._get_distances()
+        self._get_distances(node)
         return self._get_repr_recursive(node, tree)
 
     def _get_repr_recursive(self, node: Optional[Node] = None, tree: Optional[RichTree] = None) -> str:
         nodes = self.get_children(node)
         for child_node in nodes.values():
-            distance, close = self.close_node(child_node.index, self.path_indices[-1])
+            distance, close = self.close_node(child_node.index, self.path_indices[-1] if len(self.path) else None)
             style = "dim blue" if distance else "bold red"
             if not close:
-                subtree = tree.add("...", style=style)
+                children = self.get_all_children(child_node)
+                no_children = len(children)
+                subtree = tree.add(f"... ({no_children})", style=style)
                 continue
             subtree = tree.add(self._text(child_node), style=style)
             self._get_repr_recursive(child_node, subtree)
         return tree
 
     def _text(self, node: Node) -> str:
         text_width = shutil.get_terminal_size().columns - 30
```

### Comparing `command_line_loom-0.0.6/cll/data_structs/loom_index.py` & `command_line_loom-0.0.7/cll/data_structs/loom_index.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import subprocess
-import datetime
+from copy import deepcopy
 import json
 from typing import Any, Dict, Optional, Sequence, List, Union
-from pathlib import Path
 
 from .data_structs import IndexGraph, Node
 from llama_index.schema import BaseDocument
 
 
 class LoomIndex:
     """Multiverse Index.
@@ -107,48 +105,87 @@
         """Cherry pick a list of nodes in the index."""
         nodes = []
         for identifier in identifiers:
             if identifier in self.tags.keys():
                 node = self.index_struct.all_nodes[self.tags[identifier]]
             else:
                 node = self.index_struct.get_node(identifier)
-            nodes.append(node)
+            nodes.append(deepcopy(node))
+
         for node in nodes:
+            node.child_indices = set()
+            node.node_info.pop("checked_out", None)
+            node.index = len(self.index_struct.all_nodes)
             self.extend(node)
 
-    def delete(self, identifiers: List[Union[int, str]]) -> None:
+    def hoist(self, identifier: Union[int, str], target: Optional[Union[int, str]]) -> None:
+        """Hoist a node in the index."""
+        branch = self.identify(identifier)
+        target = self.identify(target)
+
+        if branch is None:
+            return
+
+        # Now copy the node and all its children
+        if target is None:
+            self.clear_checkout()
+        else:
+            self.checkout_path(target)
+        self.rebuild(branch)
+
+    def identify(self, identifier: Optional[Union[int, str]]) -> None:
+        if identifier is None:
+            return
+        if identifier in self.tags.keys():
+            return self.index_struct.all_nodes[self.tags[identifier]]
+        else:
+            return self.index_struct.get_node(identifier)
+
+    def rebuild(self, node: Node) -> None:
+        """Rebuild the index from a list of nodes."""
+        node.node_info.pop("checked_out", None)
+        node = deepcopy(node)
+        node.index = len(self.index_struct.all_nodes)
+        child_indices = node.child_indices
+        node.child_indices = set()
+        self.extend(node)
+        for child_id in child_indices:
+            child = self.index_struct.all_nodes[child_id]
+            node.child_indices.add(self.rebuild(child))
+            self.checkout(node.index)
+        return node.index
+
+    def delete(self, identifiers: List[Union[int, str]], all: bool = False) -> None:
         """Delete a list of nodes in the index."""
         if not isinstance(identifiers, list):
             identifiers = [identifiers]
         nodes = []
         for identifier in identifiers:
             if identifier in self.tags.keys():
                 node = self.index_struct.all_nodes[self.tags[identifier]]
             else:
                 node = self.index_struct.get_node(identifier)
             nodes.append(node)
         for node in nodes:
-            del self.index_struct.all_nodes[node.index]
-            if node.index in self.index_struct._root_nodes:
-                self.index_struct._root_nodes.remove(node.index)
+            self.index_struct.delete(node, all=all)
 
     def clear_checkout(self) -> None:
         """Clear checkout."""
         for node in self.index_struct.all_nodes.values():
             node.node_info.pop("checked_out", None)
         for node in self.index_struct.root_nodes.values():
             node.node_info.pop("checked_out", None)
 
     def repr(self, node):
         if isinstance(node, int):
             node = self.index_struct.all_nodes[node]
         return self.index_struct._get_repr(node)
 
     def __repr__(self) -> str:
-        return self.__str__()
+        return self.__str__() or "No summary available."
 
     def __str__(self) -> str:
         self.path_formatted
 
     @property
     def path_formatted(self) -> List[Node]:
         return self.index_struct.path_formatted
```

### Comparing `command_line_loom-0.0.6/cll/data_structs/node.py` & `command_line_loom-0.0.7/cll/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/encoder.py` & `command_line_loom-0.0.7/cll/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,7 +117,9 @@
         elif string.startswith('rot') or string.startswith('caesar'):
             # Get the number from the string
             parts = re.split(r"(\d+)", string)
             # Get the number from the string
             number = int(parts[1])
             # Get the encoding function
             return lambda s: Encoder.caesar(s, -number)
+
+        return Encoder.none
```

### Comparing `command_line_loom-0.0.6/cll/io.py` & `command_line_loom-0.0.7/cll/io.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/store.py` & `command_line_loom-0.0.7/cll/store.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/templater.py` & `command_line_loom-0.0.7/cll/templater.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.6/cll/tree.py` & `command_line_loom-0.0.7/cll/tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from rich import print
 from rich.console import Console
 from rich.panel import Panel
 from typer import Argument, Context, get_app_dir
 from typing_extensions import Annotated
 
 from typer_shell import make_typer_shell
+from typer_shell.typer_shell import _update as update, save as save_config, _print as print_config
 from .encoder import Encoder
 
 
 @dataclass
 class DummyTree:
     params: Optional[dict] = None
     prompt: str = ""
@@ -109,15 +110,15 @@
         return
     path_str = ""
     if len(path) > 1:
         path_str += "".join([str(node) for node in path[:-1]])
     path_str += "[bold red]"
     path_str += str(path[-1])
     path_str += "[/bold red]"
-    print(Panel.fit(path_str, title="Prompt", border_style="bold magenta"))
+    print(Panel.fit(path_str, title="Prompt (unencoded, without template)", border_style="bold magenta"))
 
 
 def get_params(ctx):
     name = ctx.command.name
     if name not in ctx.obj.params_groups:
         if ctx.parent:
             name = ctx.parent.command.name
@@ -153,14 +154,22 @@
     params_path=Path(get_app_dir("cll")) / "tree.yaml"
 )
 
 
 @cli.command(hidden=True)
 def default(ctx: Context, line: str):
     """Default command"""
+    # # First, try splitting into different letters
+    # if len(line) < 5:
+    #     line = list(line)
+    #     if ctx.parent:
+    #         command = ctx.parent.command.get_command(ctx, line[0])
+    #         if command:
+    #             ctx.invoke(command, ctx=ctx, *line[1:])
+
     if len(line) < 20:
         print("Ill assume you didn't mean to send that. If you do, use 'send X'. (Below 20 chars.)")
         return
     ctx.invoke(send, ctx=ctx, msg=line.split(" "))
 
 
 @cli.command(hidden=True)
@@ -203,24 +212,67 @@
     "View may be rotated 90 degrees."
     for _ in range(count):
         ctx.obj.tree.index.step(direction)
     path_with_current(ctx)
 
 
 @cli.command()
+@cli.command(name="nb", hidden=True)
+def neighborhood(ctx: Context):
+    "The tree view is truncated for nodes that are far from the current path.\n"
+    "This command changes the size of the neighborhood.\n"
+    "There are two params: the path neighborhood and the head neighborhood.\n"
+    "The path neighborhood is the maximum distance a node can be from the current path.\n"
+    "The head neighborhood is the maximum distance a node can be from the head of the tree.\n"
+    params = get_params(ctx)
+    for key, value in params.items():
+        if key not in ["path_neighborhood", "head_neighborhood"]:
+            continue
+        value = input(f"{key} [{value}]: ")
+        if not value:
+            continue
+        update(key, value, params)
+    save_config(ctx)
+    path_with_current(ctx)
+    print(params)
+
+
+@cli.command()
 @cli.command(name="en", hidden=True)
 @cli.command(name="encoding", hidden=True)
-def encoder(ctx: Context, encoder: str):
+def encoder(
+        ctx: Context,
+        encoder: Annotated[Optional[str], Argument()] = None
+):
     '(en) Set the encoder to use. Text will be encoded and decoded before being sent.\n'
     'Available encoders:\n'
     '\t"none": no encoding\n'
     '\t"base64": base64 encoding\n'
     '\t"rot13": rot13 encoding\n'
     '\t"caesar X": caesar encoding, rot by X (rot13 == "ceaser 13")\n'
+    if not encoder:
+        click.echo(
+            "Ender a choice. I will tell you what I parse it as. "
+            "If you are happy, hit enter. "
+            "Lambdas are probably ceaser cypers correctly interpreted."
+        )
+        current_encoder = ctx.obj.tree.encoder.callback
+        last_encoder = "none"
+        while True:
+            new_encoder_name = current_encoder.__name__
+            new_encoder = input(f"encoder [{new_encoder_name}]: ")
+            if not new_encoder:
+                encoder = last_encoder
+                break
+            current_encoder = Encoder._get_encoder(new_encoder)
+            last_encoder = new_encoder
+
     set_encoder(ctx, encoder)
+    save_config(ctx)
+    print_config(ctx)
 
 
 @cli.command()
 @cli.command(name="re", hidden=True)
 def reencode(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
     "(re) Reencode the current node."
     if not index:
@@ -250,31 +302,31 @@
 
 
 @cli.command()
 @cli.command(name="d", hidden=True)
 @cli.command(name="p", hidden=True)
 def display(
     ctx: Context,
-    type: Annotated[Optional[str], Argument()] = "p",
+    type: Annotated[Optional[str], Argument()] = "t",
     index: Annotated[Optional[str], Argument()] = None,
 ):
-    """(d, p, t) Various display options (check helpgg).\n
+    """(d, p, t) Various display options (check 'help display').\n
     Types:\n
         \ttree/t: display the tree structure\n
         \tall/a: display the full tree including other roots\n
         \tpath/p: display the path to the current node\n
         \tprompt/pr: display the current prompt\n
         \ttemplated/tr: display the current prompt with templated values\n
         \tsummary/s: display the current context and latest summary\n
         \tnode/n: display the specific node(s) (pass the index of the node(s))
     """
     Console().clear()
     if type in ["t", "tree"]:
         ctx.obj.tree.index.index_struct.legend()
-        print(ctx.obj.tree._get_repr())
+        print(ctx.obj.tree.index.index_struct._get_repr())
 
     if type in ["a", "all"]:
         print(ctx.obj.tree.index.index_struct.get_full_repr())
         return
 
     if type in ["c", "context"]:
         print(ctx.obj.tree.index.context)
@@ -295,30 +347,33 @@
         return
 
     if type in ["n", "node"]:
         if index is None:
             print("Please provide an index")
             return
 
-        if "," in index:
-            indexes = index.split(",")
-        else:
-            indexes = [index]
-
-        for index in indexes:
-            if index.isdigit():
+        for index in parse_indexes(index):
+            if isinstance(index, int):
+                print(index)
                 print(ctx.obj.tree.index.index_struct.all_nodes[int(index)].text)
                 continue
 
 
-@cli.command(name="tree")
 @cli.command(name="t", hidden=True)
+@cli.command(name="dt", hidden=True)
 def display_tree(ctx: Context):
     """(t) Display the tree."""
-    path_with_current(ctx)
+    display(ctx, "t")
+
+
+@cli.command(name="a", hidden=True)
+@cli.command(name="da", hidden=True)
+def display_all(ctx: Context):
+    """(t) Display the tree."""
+    display(ctx, "a")
 
 
 def _append(ctx, msg):
     if isinstance(msg, tuple) or isinstance(msg, list):
         msg = " ".join(msg)
     node = ctx.obj.tree.index._create_node(msg)
     node = ctx.obj.templater.in_(node)
@@ -381,32 +436,35 @@
 
 
 @cli.command()
 @cli.command(name="n", hidden=True)
 def new(ctx: Context):
     """n[ew] starts a new chain (a new root)"""
     ctx.obj.tree.index.clear_checkout()
+    ctx.invoke(append, ctx=ctx, msg=None)
     ctx.obj.tree.save()
+    path_with_current(ctx)
 
 
 @cli.command()
 @cli.command(name="ap", hidden=True)
 def append(
     ctx: Context,
-    msg: Annotated[Optional[List[str]], Argument()],
+    msg: Annotated[Optional[List[str]], Argument()] = None,
 ):
     """(ap) adds a new node at the end of the chain. If MSG is empty, an editor will be opened."""
     if not msg:
         msg = click.edit()
     _append(ctx, msg)
 
 
 @cli.command()
+@cli.command("st", hidden=True)
 def save_tree(ctx: Context):
-    """Save the current tree"""
+    """(st) Save the current tree"""
     ctx.obj.tree.save()
 
 
 @cli.command()
 def tag(
     ctx: Context,
     tag: Annotated[Optional[str], Argument()],
@@ -415,27 +473,27 @@
     if tag:
         ctx.obj.tree.index.tag(tag)
     print(ctx.obj.tree.index.tags)
 
 
 @cli.command()
 @cli.command(name="c", hidden=True)
+@cli.command(name="co", hidden=True)
 def checkout(ctx: Context, tag: str):
-    "(c) checks out a tag or index"
+    "(c, co) checks out a tag or index"
     if tag.isdigit():
         tag = int(tag)
     ctx.obj.tree.index.checkout(tag)
     path_with_current(ctx)
 
 
 @cli.command()
 @cli.command(name="e", hidden=True)
 def edit(ctx: Context, index: Annotated[Optional[str], Argument()] = None):
     """(e) Edit a node (default is the current node).
-    Or pass "prompt" to export the full tree to an editor.
     """
     if not index:
         index = ctx.obj.tree.index.path[-1].index
     index = int(index)
 
     input = ctx.obj.tree.index.index_struct.all_nodes[index].text
     output = click.edit(input)
@@ -454,55 +512,84 @@
     prev_encoder = ctx.obj.tree.encoder
     ctx.obj.tree.encoder = Encoder.get_encoder("none")
     input = str(ctx.obj.tree.prompt)
     ctx.obj.tree.encoder = prev_encoder
     click.edit(input)
 
 
-# @cli.command()
-# @cli.command(name="del", hidden=True)
-# def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None):
-#     "(del) delete some nodes (space separated) (last one by default)"
-#     if not indexes:
-#         indexes = [ctx.obj.tree.index.path[-1].index]
-#     else:
-#         indexes = indexes.split(" ")
-#     ctx.obj.tree.index.delete(indexes)
+def parse_indexes(indexes):
+    if "," in indexes:
+        indexes = indexes.split(",")
+    elif ":" in indexes:
+        indexes = indexes.split(":")
+    else:
+        indexes = indexes.split(" ")
+    return [int(index) if index.isdigit() else index for index in indexes]
+
+
+@cli.command()
+@cli.command(name="del", hidden=True)
+def delete(ctx: Context, indexes: Annotated[Optional[str], Argument()] = None, all: bool = False):
+    "(del) delete some nodes (space separated) (last one by default)"
+    if not indexes:
+        indexes = [ctx.obj.tree.index.path[-1].index]
+    else:
+        indexes = parse_indexes(indexes)
+    ctx.obj.tree.index.delete(indexes, all=all)
 
 
 @cli.command()
 @cli.command(name="cp", hidden=True)
 def cherry_pick(ctx: Context, indexes: str):
     "(cp) Copy nodes onto the current branch (can be indexes or tags, space separated)"
-    indexes = [int(index) if index.isdigit() else index for index in indexes.split(" ")]
+    indexes = parse_indexes(indexes)
     ctx.obj.tree.index.cherry_pick(indexes)
+    path_with_current(ctx)
+
+
+@cli.command()
+@cli.command(name="hh", hidden=True)
+def hoist(ctx: Context, target: Annotated[Optional[str], Argument()] = None):
+    "Copies the node and all downstreams to a new root."
+    index = ctx.obj.tree.index.path[-1].index
+    ctx.obj.tree.index.hoist(index, target)
+    path_with_current(ctx)
 
 
 @cli.command()
 def dump(ctx: Context):
     "Dump nodes into a fuzzy finder"
     selection = iterfzf.iterfzf(ctx.obj.tree.index.index_struct.active_tree_with_index, multi=True)
     if selection is None:
         return
     ids = [int(index.split(":")[0]) for index in selection]
-    print("\n".join(selection))
+    text = "\n".join(selection)
+    print(Panel(
+        f"[bold magenta]Selected:[/bold magenta]\n{text}\n"
+        f"\n[bold magenta]What do you want to do with these nodes?[/bold magenta]\n"
+        "\t([bold red]edit, e[/bold red]) dump the nodes into one file and open it in an editor\n"
+        "\t([bold red]cherry pick, cp[/bold red]) copy the nodes onto the current branch\n"
+        "\t([bold red]delete, d[/bold red]) delete the nodes\n"
+        "\t([bold red]cancel, c[/bold red])",
+        title="Dump",
+        border_style="bold magenta",
+    ))
     choice = click.prompt(
-        f"You selected {ids}, what do you want to do?\n"
-        "\t(edit) dump the nodes into one file and open it in an editor\n"
-        "\t(cherry pick) copy the nodes onto the current branch\n"
-        "\t(delete) delete the nodes\n"
-        "\t(cancel)",
+        "Choice:",
         type=click.Choice(["edit", "cherry pick", "delete", "cancel", "e", "cp", "d", "c"]),
     )
     if choice in ["e", "edit"]:
         text = "\n".join([ctx.obj.tree.index.index_struct.all_nodes[id].text for id in ids])
         output = click.edit(text)
         if output is None:
             return
-        ctx.obj.tree.extend(output)
+        node_template = deepcopy(ctx.obj.tree.index.index_struct.all_nodes[ids[0]])
+        node_template.child_indices = set()
+        node_template.text = output
+        ctx.obj.tree.extend(node_template)
     elif choice in ["cp", "cherry pick"]:
         ctx.obj.tree.index.cherry_pick(ids)
     elif choice in ["d", "delete"]:
         ctx.obj.tree.index.delete(ids)
 
     path_with_current(ctx)
```

### Comparing `command_line_loom-0.0.6/pyproject.toml` & `command_line_loom-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "command-line-loom"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 homepage = "https://github.com/fergusfettes/command-line-loom"
 readme = "README.md"
 packages = [{include = "cll"}]
 
 [tool.poetry.dependencies]
```

### Comparing `command_line_loom-0.0.6/PKG-INFO` & `command_line_loom-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command-line-loom
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://github.com/fergusfettes/command-line-loom
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -47,14 +47,16 @@
 poetry install
 ```
 
 ## Usage
 
 Should be self-documenting in the interface. Just type 'help'.
 
+Some node manipulation: [vid](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)
+
 Watch this for more advanced usage: [vid](https://asciinema.org/a/tLpxm9FdW6gKdJztRnAPAOl7X).
 
 ## Configuration
 
 Before using Command Line Loom, you need to set up a configuration file. This should happen automatically when you run the `cll` command for the first time.
 
 This will create a configuration file in your home directory. See the documentation for each model to learn how to obtain an API key.
```

