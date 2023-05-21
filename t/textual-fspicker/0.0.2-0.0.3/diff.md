# Comparing `tmp/textual_fspicker-0.0.2-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 10971 bytes, number of entries: 11
--rw-r--r--  2.0 unx      692 b- defN 23-May-19 09:53 textual_fspicker/__init__.py
--rw-r--r--  2.0 unx     1159 b- defN 23-May-18 19:46 textual_fspicker/__main__.py
--rw-r--r--  2.0 unx     6739 b- defN 23-May-19 09:53 textual_fspicker/file_open.py
+Zip file size: 13341 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      740 b- defN 23-May-21 08:58 textual_fspicker/__init__.py
+-rw-r--r--  2.0 unx     2305 b- defN 23-May-21 08:58 textual_fspicker/__main__.py
+-rw-r--r--  2.0 unx     7980 b- defN 23-May-21 08:58 textual_fspicker/file_open.py
+-rw-r--r--  2.0 unx     1822 b- defN 23-May-21 08:58 textual_fspicker/path_filters.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
 -rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
--rw-r--r--  2.0 unx    11908 b- defN 23-May-19 09:53 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     5250 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      949 b- defN 23-May-19 09:53 textual_fspicker-0.0.2.dist-info/RECORD
-11 files, 29369 bytes uncompressed, 9345 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx    15053 b- defN 23-May-21 08:58 textual_fspicker/parts/directory_navigation.py
+-rw-r--r--  2.0 unx     6396 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1038 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/RECORD
+12 files, 38006 bytes uncompressed, 11575 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,32 +3,35 @@
 
 Filename: textual_fspicker/__main__.py
 Comment: 
 
 Filename: textual_fspicker/file_open.py
 Comment: 
 
+Filename: textual_fspicker/path_filters.py
+Comment: 
+
 Filename: textual_fspicker/py.typed
 Comment: 
 
 Filename: textual_fspicker/safe_tests.py
 Comment: 
 
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.2.dist-info/METADATA
+Filename: textual_fspicker-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.2.dist-info/WHEEL
+Filename: textual_fspicker-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.2.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.2.dist-info/RECORD
+Filename: textual_fspicker-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_fspicker/__init__.py

```diff
@@ -3,19 +3,20 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.0.2"
+__version__    = "0.0.3"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
-from .file_open import FileOpen
+from .file_open    import FileOpen
+from .path_filters import Filters
 
 ##############################################################################
 # Export the imports.
-__all__ = [ "FileOpen" ]
+__all__ = [ "FileOpen", "Filters" ]
 
 ### __init__.py ends here
```

## textual_fspicker/__main__.py

```diff
@@ -2,33 +2,65 @@
 
 ##############################################################################
 # Python imports.
 from pathlib import Path
 
 ##############################################################################
 # Textual imports.
-from textual.app     import App, ComposeResult
-from textual.widgets import Label, Button
+from textual.app        import App, ComposeResult
+from textual.containers import Center
+from textual.widgets    import Label, Button
 
 ##############################################################################
 # Local imports.
-from textual_fspicker import FileOpen
+from textual_fspicker import FileOpen, Filters
 
 ##############################################################################
 class TestApp( App[ None ] ):
     """A simple test application."""
 
-    def compose( self ) -> ComposeResult:
-        yield Label( "Press the button to pick something" )
-        yield Button( "Select a file" )
+    CSS = """
+    Screen#_default {
+        align: center middle;
+    }
+
+    Screen#_default Button {
+        margin-bottom: 2;
+    }
+    """
 
-    def show_selected( self, to_open: Path ) -> None:
-        self.query_one( Label ).update( str( to_open ) )
+    def compose( self ) -> ComposeResult:
+        """Compose the layout of the test application."""
+        with Center():
+            yield Button( "Select a file" )
+        with Center():
+            yield Label( "Press the button to pick something" )
+
+    def show_selected( self, to_show: Path ) -> None:
+        """Show the file that was selected by the user.
+
+        Args:
+            to_show: The file to show.
+        """
+        self.query_one( Label ).update( str( to_show ) )
 
     def on_button_pressed( self ):
-        self.push_screen( FileOpen( "." ), callback=self.show_selected )
+        """Show the `FileOpen` dialog when the button is pushed."""
+        self.push_screen(
+            FileOpen( ".", filters=Filters(
+                ( "Any",     lambda _: True ),
+                ( "Emacs",   lambda p: p.suffix.lower() == ".el" ),
+                ( "Lisp",    lambda p: p.suffix.lower() in ( ".lisp", ".lsp", ".cl" ) ),
+                ( "Python",  lambda p: p.suffix.lower() == ".py" ),
+                ( "Pascal",  lambda p: p.suffix.lower() == ".pas" ),
+                ( "Clipper", lambda p: p.suffix.lower() in ( ".prg", ".ch" ) ),
+                ( "C",       lambda p: p.suffix.lower() in ( ".c", ".h" ) ),
+                ( "C++",     lambda p: p.suffix.lower() in ( ".cpp", ".cc", ".h" ) ),
+            ) ),
+            callback=self.show_selected
+        )
 
 ##############################################################################
 if __name__ == "__main__":
     TestApp().run()
 
 ### __main__.py ends here
```

## textual_fspicker/file_open.py

```diff
@@ -8,29 +8,34 @@
 ##############################################################################
 # Textual imports.
 from textual            import on
 from textual.app        import ComposeResult
 from textual.binding    import Binding
 from textual.containers import Horizontal, Vertical
 from textual.screen     import ModalScreen
-from textual.widgets    import Button, Input
+from textual.widgets    import Button, Input, Select
 
 ##############################################################################
 # Local imports.
-from .parts import DirectoryNavigation
+from .parts        import DirectoryNavigation
+from .path_filters import Filters
 
 ##############################################################################
 class Dialog( Vertical ):
     """Layout class for the main dialog area."""
 
 ##############################################################################
 class InputBar( Horizontal ):
     """The input bar area of the dialog."""
 
 ##############################################################################
+class FileFilter( Select[ int ] ):
+    """The file filter."""
+
+##############################################################################
 class FileOpen( ModalScreen[ Path ] ):
     """A file opening dialog."""
 
     DEFAULT_CSS = """
     FileOpen {
         align: center middle;
     }
@@ -55,51 +60,70 @@
     }
 
     FileOpen InputBar Button {
         margin-left: 1;
     }
 
     FileOpen InputBar Input {
+        width: 2fr;
+    }
+
+    FileOpen InputBar Select {
         width: 1fr;
     }
     """
 
     BINDINGS = [
         Binding( "escape", "dismiss" ),
         Binding( "full_stop", "hidden" )
     ]
     """The bindings for the dialog."""
 
-    def __init__( self, location: str | Path | None=None, title: str="Open", must_exist: bool=True ) -> None:
+    def __init__(
+            self,
+            location: str | Path | None = None,
+            title: str = "Open",
+            must_exist: bool = True,
+            filters: Filters | None = None
+        ) -> None:
         """Initialise the `FileOpen` dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
             must_exist: Flag to say if the file must exist.
         """
         super().__init__()
         self._location = location
         """The starting location."""
         self._title = title
         """The title for the dialog."""
         self._must_exist = must_exist
         """Must the file exist?"""
+        self._filters = filters
+        """The filters for the dialog."""
 
     def compose( self ) -> ComposeResult:
         """Compose the child widgets.
 
         Returns:
             The widgets to compose.
         """
         with Dialog() as dialog:
             dialog.border_title = self._title
             yield DirectoryNavigation(self._location)
             with InputBar():
                 yield Input()
+                if self._filters:
+                    yield FileFilter(
+                        self._filters.selections,
+                        prompt      = "File filter",
+                        value       = 0,
+                        allow_blank = False
+                    )
                 yield Button( "Open", id="open" )
                 yield Button( "Cancel", id="cancel" )
 
     def _set_error( self, message: str="" ) -> None:
         """Set or clear the error message.
 
         Args:
@@ -196,8 +220,23 @@
         """Clear any error that might be showing."""
         self._set_error()
 
     def action_hidden( self ) -> None:
         """Action for toggling the display of hidden files."""
         self.query_one( DirectoryNavigation ).toggle_hidden()
 
+    @on( Select.Changed )
+    def _change_filter( self, event: Select.Changed ) -> None:
+        """Handle a change in the filter.
+
+        Args:
+            event: The event to handle.
+        """
+        if self._filters is not None and isinstance( event.value, int ):
+            self.query_one( DirectoryNavigation ).file_filter = self._filters[
+                event.value
+            ]
+        else:
+            self.query_one( DirectoryNavigation ).file_filter = None
+        self.query_one( DirectoryNavigation ).focus()
+
 ### file_open.py ends here
```

## textual_fspicker/parts/directory_navigation.py

```diff
@@ -2,65 +2,85 @@
 
 ##############################################################################
 # Python imports.
 from __future__        import annotations
 from dataclasses       import dataclass
 from datetime          import datetime
 from pathlib           import Path
-from typing            import Iterable
+from typing            import ClassVar, Iterable, NamedTuple, Optional
 from typing_extensions import Final
 
 ##############################################################################
 # Rich imports.
 from rich.console import RenderableType
+from rich.style   import Style
 from rich.table   import Table
 from rich.text    import Text
 
 ##############################################################################
 # Textual imports.
 from textual                     import work
 from textual.reactive            import var
 from textual.message             import Message
 from textual.widgets             import OptionList
 from textual.widgets.option_list import Option
 from textual.worker              import get_current_worker
 
 ##############################################################################
 # Local imports.
-from ..safe_tests import is_dir, is_file, is_symlink
+from ..safe_tests   import is_dir, is_file, is_symlink
+from ..path_filters import Filter
+
+##############################################################################
+class DirectoryEntryStyling( NamedTuple ):
+    """Styling for directory entries."""
+
+    hidden: Style
+    """Styling for hidden entries."""
+
+    name: Style
+    """Styling for a name."""
+
+    size: Style
+    """Styling for a size."""
+
+    time: Style
+    """Styling for a time."""
 
 ##############################################################################
 class DirectoryEntry( Option ):
     """A directory entry for the `DirectoryNaviation` class."""
 
     FOLDER_ICON: Final[ Text ] = Text.from_markup( ":file_folder:" )
     """The icon to use for a folder."""
 
     FILE_ICON: Final[ Text ] = Text.from_markup( ":page_facing_up:" )
     """The icon to use for a file."""
 
     LINK_ICON: Final[ Text ] = Text.from_markup( ":link:" )
     """The icon to use for links."""
 
-    def __init__( self, location: Path ) -> None:
+    def __init__( self, location: Path, styles: DirectoryEntryStyling ) -> None:
         self.location: Path = location.absolute()
         """The location of this directory entry."""
+        self._styles = styles
         super().__init__( self._as_renderable( location ) )
 
-    def _name( self, location: Path ) -> Text:
+    @classmethod
+    def _name( cls, location: Path ) -> Text:
         """Get a formatted name for the given location.
 
         Args:
             location: The location to get the name for.
 
         Returns:
             The formatted name.
         """
         return Text.assemble(
-            location.name, " ", self.LINK_ICON if is_symlink( location ) else ""
+            location.name, " ", cls.LINK_ICON if is_symlink( location ) else ""
         )
 
     @staticmethod
     def _mtime( location: Path ) -> str:
         """Get a formatted modification time for the given location.
 
         Args:
@@ -88,29 +108,44 @@
         try:
             entry_size = location.stat().st_size
         except FileNotFoundError:
             entry_size = 0
         # TODO: format well for a file browser.
         return str( entry_size )
 
+    def _style( self, base: Style, location: Path ) -> Style:
+        """Decide the best style to use.
+
+        Args:
+            base: The base style to start with.
+            location: The location to decide the style for.
+        """
+        return base + Style(
+            color     = self._styles.hidden.color,
+            italic    = self._styles.hidden.italic,
+            bold      = self._styles.hidden.bold,
+            underline = self._styles.hidden.underline
+        ) if DirectoryNavigation.is_hidden( location ) else base
+
     def _as_renderable( self, location: Path ) -> RenderableType:
         """Create the renderable for this entry.
 
         Args:
             location: The location to turn into a renderable.
 
         Returns:
             The entry as a Rich renderable.
         """
+
         prompt = Table.grid( expand=True )
         prompt.add_column( no_wrap=True, width=1 )
         prompt.add_column( no_wrap=True, justify="left", width=3 )
-        prompt.add_column( no_wrap=True, justify="left", ratio=1 )
-        prompt.add_column( no_wrap=True, justify="right", width=10 )
-        prompt.add_column( no_wrap=True, justify="right", width=20 )
+        prompt.add_column( no_wrap=True, justify="left", ratio=1, style=self._style( self._styles.name, location ) )
+        prompt.add_column( no_wrap=True, justify="right", width=10, style=self._style( self._styles.size, location ) )
+        prompt.add_column( no_wrap=True, justify="right", width=20, style=self._style( self._styles.time, location ) )
         prompt.add_column( no_wrap=True, width=1 )
         prompt.add_row(
             "",
             self.FOLDER_ICON if is_dir( location ) else self.FILE_ICON,
             self._name( location ),
             self._size( location ),
             self._mtime( location ),
@@ -123,14 +158,42 @@
     """A directory navigation widget.
 
     Provides a single-pane widget that lets the user navigate their way
     through a filesystenm, changing in and out of directories, and selecting
     a file.
     """
 
+    COMPONENT_CLASSES: ClassVar[set[str]] = {
+        "directory-navigation--hidden",
+        "directory-navigation--name",
+        "directory-navigation--size",
+        "directory-navigation--time",
+    }
+    """Component styles for the directory navigation widget."""
+
+    DEFAULT_CSS = """
+    DirectoryNavigation > .directory-navigation--hidden {
+        color: $text-muted;
+        text-style: italic;
+    }
+
+    DirectoryNavigation > .directory-navigation--name {
+        color: $text;
+    }
+
+    DirectoryNavigation > .directory-navigation--size {
+        color: $text;
+    }
+
+    DirectoryNavigation > .directory-navigation--time {
+        color: $text;
+    }
+    """
+    """Default styling for the widget."""
+
     @dataclass
     class _BaseMessage( Message ):
         """Base class for directory navigation messages."""
 
         control: DirectoryNavigation
         """The directory navigation control sending the message."""
 
@@ -152,14 +215,17 @@
 
     class PermissionError( _PathMessage ):
         """Message sent when there's a permission problem with a path."""
 
     _location: var[ Path ] = var[ Path ]( Path( "." ).absolute(), init=False )
     """The current location for the directory."""
 
+    file_filter: var[ Filter | None ] = var[ Optional[ Filter ] ]( None )
+    """The active file filter."""
+
     show_files: var[ bool ] = var( True )
     """Should files be shown and be selectable?"""
 
     show_hidden: var[ bool ] = var( False )
     """Should hidden entries be shown?"""
 
     sort_display: var[ bool ] = var( True )
@@ -216,39 +282,56 @@
             `True` if the path appears to be hidden, `False` if not.
 
         Note:
             For the moment this simply checks for the 'dot hack'. Eventually
             I'll extend this to detect hidden files in the most appropriate
             way for the current operating system.
         """
-        return path.name.startswith( "." )
+        return path.name.startswith( "." ) and path.name != ".."
 
     def hide( self, path: Path ) -> bool:
         """Should we hide the given path?
 
         Args:
             path: The path to test.
 
         Returns:
             `True` if the path should be hidden, `False` if not.
         """
+        # If there's a custom filter in place, give that a go first...
+        if self.file_filter is not None and is_file( path ):
+            if not self.file_filter( path ):
+                return True
+        # Either there is no custom filter, or whatever we're looking at
+        # passed so far; not do final checks.
         return self.is_hidden( path ) and not self.show_hidden
 
     def _sort( self, entries: Iterable[ DirectoryEntry ] ) -> Iterable[ DirectoryEntry ]:
         """Sort the entries as per the value of `sort_display`."""
         if self.sort_display:
             return sorted( entries, key=lambda entry: ( not is_dir( entry.location ), entry.location.name ) )
         return entries
 
+    @property
+    def _styles( self ) -> DirectoryEntryStyling:
+        """The styles to use for a directory entry."""
+        return DirectoryEntryStyling(
+            self.get_component_rich_style( "directory-navigation--hidden" ),
+            self.get_component_rich_style( "directory-navigation--name", partial=True ),
+            self.get_component_rich_style( "directory-navigation--size", partial=True  ),
+            self.get_component_rich_style( "directory-navigation--time", partial=True  ),
+        )
+
     def _repopulate_display( self ) -> None:
         """Repopulate the display of directories."""
+        styles = self._styles
         with self.app.batch_update():
             self.clear_options()
             if not self.is_root:
-                self.add_option( DirectoryEntry( self._location / ".." ) )
+                self.add_option( DirectoryEntry( self._location / "..", styles ) )
             self.add_options( self._sort( entry for entry in self._entries if not self.hide( entry.location ) ) )
         self._settle_highlight()
 
     @work(exclusive=True)
     def _load( self ) -> None:
         """Load the current directory data."""
 
@@ -259,18 +342,19 @@
         # parallel copy of *all* possible options for the list and then
         # populate from that.
         self._entries = []
 
         # Now loop over the directory, looking for directories within and
         # streaming them into the list via the app thread.
         worker = get_current_worker()
+        styles = self._styles
         try:
             for entry in self._location.iterdir():
                 if is_dir( entry ) or ( is_file( entry ) and self.show_files ):
-                    self._entries.append( DirectoryEntry( self._location / entry.name ) )
+                    self._entries.append( DirectoryEntry( self._location / entry.name, styles ) )
                 if worker.is_cancelled:
                     return
         except PermissionError:
             self.post_message( self.PermissionError( self, self._location ) )
 
         # Now that we've loaded everything up, let's make the call to update
         # the display.
@@ -289,14 +373,18 @@
         """Reload the content if the show-files flag has changed."""
         self._load()
 
     def _watch_sort_display( self ) -> None:
         """Refresh the display if the sort option has been changed."""
         self._repopulate_display()
 
+    def _watch_file_filter( self ) -> None:
+        """Refresh the display when the file filter has been changed."""
+        self._repopulate_display()
+
     def toggle_hidden( self ) -> None:
         """Toggle the display of hidden filesystem entries."""
         self.show_hidden = not self.show_hidden
 
     def _on_option_list_option_highlighted( self, event: OptionList.OptionHighlighted ) -> None:
         """Handle an entry in the list being highlighted.
```

## Comparing `textual_fspicker-0.0.2.dist-info/METADATA` & `textual_fspicker-0.0.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-fspicker
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Textual filesystem picker dialog library.
 Home-page: https://github.com/davep/textual-fspicker
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -82,34 +82,66 @@
 
 ##############################################################################
 # Python imports.
 from pathlib import Path
 
 ##############################################################################
 # Textual imports.
-from textual.app     import App, ComposeResult
-from textual.widgets import Label, Button
+from textual.app        import App, ComposeResult
+from textual.containers import Center
+from textual.widgets    import Label, Button
 
 ##############################################################################
 # Local imports.
-from textual_fspicker import FileOpen
+from textual_fspicker import FileOpen, Filters
 
 ##############################################################################
 class TestApp( App[ None ] ):
     """A simple test application."""
 
-    def compose( self ) -> ComposeResult:
-        yield Label( "Press the button to pick something" )
-        yield Button( "Select a file" )
+    CSS = """
+    Screen#_default {
+        align: center middle;
+    }
+
+    Screen#_default Button {
+        margin-bottom: 2;
+    }
+    """
 
-    def show_selected( self, to_open: Path ) -> None:
-        self.query_one( Label ).update( str( to_open ) )
+    def compose( self ) -> ComposeResult:
+        """Compose the layout of the test application."""
+        with Center():
+            yield Button( "Select a file" )
+        with Center():
+            yield Label( "Press the button to pick something" )
+
+    def show_selected( self, to_show: Path ) -> None:
+        """Show the file that was selected by the user.
+
+        Args:
+            to_show: The file to show.
+        """
+        self.query_one( Label ).update( str( to_show ) )
 
     def on_button_pressed( self ):
-        self.push_screen( FileOpen( "." ), callback=self.show_selected )
+        """Show the `FileOpen` dialog when the button is pushed."""
+        self.push_screen(
+            FileOpen( ".", filters=Filters(
+                ( "Any",     lambda _: True ),
+                ( "Emacs",   lambda p: p.suffix.lower() == ".el" ),
+                ( "Lisp",    lambda p: p.suffix.lower() in ( ".lisp", ".lsp", ".cl" ) ),
+                ( "Python",  lambda p: p.suffix.lower() == ".py" ),
+                ( "Pascal",  lambda p: p.suffix.lower() == ".pas" ),
+                ( "Clipper", lambda p: p.suffix.lower() in ( ".prg", ".ch" ) ),
+                ( "C",       lambda p: p.suffix.lower() in ( ".c", ".h" ) ),
+                ( "C++",     lambda p: p.suffix.lower() in ( ".cpp", ".cc", ".h" ) ),
+            ) ),
+            callback=self.show_selected
+        )
 
 ##############################################################################
 if __name__ == "__main__":
     TestApp().run()
 
 ### __main__.py ends here
 ```
@@ -124,15 +156,15 @@
 ## TODO
 
 - [ ] Flesh out what's displayed for directory entries
 - [ ] Add lots of styling options for directory entries
 - [ ] Settle on a final set of default styles for the dialogs
 - [ ] Add a more file-save-oriented dialog
 - [ ] Add a directory picking dialog
-- [ ] Add file filtering (extensions using `Select`)
+- [X] Add file filtering (extensions using `Select`)
 - [ ] Expose the hidden show/hide facility of the navigator in the dialogs
 - [ ] Better documentation
 - [ ] Test on Windows
 - [ ] Add custom mtime formatting
 - [ ] Add support for showing different times
 
 [//]: # (README.md ends here)
```

## Comparing `textual_fspicker-0.0.2.dist-info/RECORD` & `textual_fspicker-0.0.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-textual_fspicker/__init__.py,sha256=XqT9vmErdUGFM5xvWQulcEXtly6pLvsYHJbvDtBYFVQ,692
-textual_fspicker/__main__.py,sha256=RH99m2IWJMk2P9kelzkPyPQsfh_Yr6NkDDPMSRxoRFs,1159
-textual_fspicker/file_open.py,sha256=mADAv59DgUcUxfaw2KS5sngB8bzoYYilwXvTooevtMw,6739
+textual_fspicker/__init__.py,sha256=FUz9CzbjP9eRy8ekM_TWOeS0aLrwWe3BfmgMaaRL2Dk,740
+textual_fspicker/__main__.py,sha256=P5L8aMAp_LloN1VpcxJTQBGb6iRTq-VuDYAXxWOq4ro,2305
+textual_fspicker/file_open.py,sha256=oAxxWgIBBSx1pNQIY9behjly7CWGsZBsi4nN0oAfhH0,7980
+textual_fspicker/path_filters.py,sha256=XpPrynKVI_p8Tf6tUuhEmU5lxAaf3TQlsjKsRwXC5nk,1822
 textual_fspicker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 textual_fspicker/safe_tests.py,sha256=U3gpqVRr7qcv7mqF-I_sFojtr9Pv5JyqFzAxGG7qofA,2174
 textual_fspicker/parts/__init__.py,sha256=vjP1jzd5ty4IhwUZnVFkOjzctZn22EbwWDHh_16x-GM,389
-textual_fspicker/parts/directory_navigation.py,sha256=yJGjP2dkSwTpNqP0sh3no1cE_wJ4WDiRmIwjxdc9rDg,11908
-textual_fspicker-0.0.2.dist-info/METADATA,sha256=GB7Agrqhtn7pIG9OxAiO5kkHimcvtR9mijDmvcoDMHs,5250
-textual_fspicker-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-textual_fspicker-0.0.2.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
-textual_fspicker-0.0.2.dist-info/RECORD,,
+textual_fspicker/parts/directory_navigation.py,sha256=6jg6mBcBbVsH7DcimhsF2XKpwXqWBaVb4f2xx5G9mm0,15053
+textual_fspicker-0.0.3.dist-info/METADATA,sha256=CoAX4O10T8ZJX64-0AN4QYYBVSgw0PWyLI5lupuUmpo,6396
+textual_fspicker-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+textual_fspicker-0.0.3.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
+textual_fspicker-0.0.3.dist-info/RECORD,,
```

