# Change Log

### 0.3.7
* Add `lint` configuration to control the behaviors of syntax checking
* Fix error with run godot editor when the editor contains spaces
* Disable semicolons and brackets checks as default can be enabled with project settings
* Fix bugs in syntax valiadating
* Sync documentations with godot 3.0.4
```json
{
    "lint": {
        "semicolon": true,
        "conditionBrackets": true
    }
}
```

### 0.3.6
* Fix project configuration file path

### 0.3.5
* Add option to disable syntax checking for GDScript
* Improved inline if else statement syntax checking
* More resource type supported for syntax highglight
* Bump default godot version to 3.0
* Sync the documentations from godot 3.0

### 0.3.4
* Fix bug with builtin symbols parsing for godot 2.1
* Improved hover documentation
* Show window progress when parsing workspace symbols

### 0.3.3
* Fix some syntax checking errors.
* Fix problems with hover documentation with latest VSCode.
* Improved builtin class documentation page.
* Update the documentation data with latest godot version.

### 0.3.2
* Fix syntax checking error with match statement.
* Improved documentation for builtin code blocks.
* Start using MarkdonwString to keep links valid.

### 0.3.1
* Update documentations with latest godot.
* Fix errors with run script and run project.
* Improve code completion with opening script file and constants.
* Some improvements for documentations.

### 0.3.0
* Add project root configuration settings as `GodotTools.godotProjectRoot` thanks Konstantin Zaitcev
* Add auto indent support for gdscript language
* More friendly with godot 3.0 alpha
* Updated script snippets
* Fix highglight error with gdscript language
* Limited code completions

### 0.2.9
* Add configuration `GodotTools.completeNodePath` to switch is complete node paths
* Enhanced syntax highlight with GDScript
* Enhanced code completion with GDScript

### 0.2.8
* Add godot 3.0 project support with configuration `GodotTools.parseTextScene` >= 3
* Add configuration `GodotTools.parseTextScene` to allow disable node path parsing
* Remove `GodotTools.editorServerPort` configuration

### 0.2.7

* Fix some error with syntax checking
* Add symbol support for enumerations
* Remove key bindings for `F5`~`F8` as it might be conflict with other functionalities of VSCode
    * You can bind the key bindings back by add following configurations
    ```json
    {
        "command": "godot.runWorkspace",
        "key": "F5"
    },
    {
        "command": "godot.runCurrentScene",
        "key": "F6"
    },
    {
        "command": "godot.openWithEditor",
        "key": "F7"
    },
    {
        "command": "godot.updateWorkspaceSymbols",
        "key": "F8"
    }
    ```
    For more references please ready [keybindings](https://code.visualstudio.com/docs/getstarted/keybindings)

### 0.2.6

* Add shorthand if else expression support
* Add `enum` and `match` expression support
* Fix bugs with syntax checking
* Updated documentation data with godot 2.1.3
* Add syntax checking for end of expression
* The pulugin is compiled with latest VSCode thanks @arrkiin
* Add key bindings for open workspace with godot editor with `F7` and update workspace symbols with `F8`

### 0.2.5

* Run games within VSCode terminals
* Add key bindings for `F5 to run the workspace` and `F6 to run the edting scene`
* Fix a lot of bugs with unused variable checking
* Move workspace symbols state notice to status bar

### 0.2.4

* Add code checking for asignments and comparisons
* Improved builtin documentation preview page
* Fix bugs with unused variable checking

### 0.2.3
* Fix known errors with code syntax checking
* Add configuration `ignoreIndentedVars` to allow ignore indented variables in scripts
* Enhanced hover tip documentation rendering with code examples
* Add launch configurations to launch game with F5(expiremental)

### 0.2.2
* Better Syntax validating for code blocks
* More warning for non-python liked expression

### 0.2.1
* Support markdown render in hover tips for documentations in workspace symbols
* Add configuration `GodotTools.workspaceDocumentWithMarkdown` to control workspace documentation rendering

### 0.2.0

* Show autoloads information in hover tips and go to autoloads' definitions are supported now
* Fix the bug that workspace symbols resoved twice on Windows

### 0.1.9

* Show workspace constant value in hover tips and completion items
* More readable style for links in documentation preview page
* Improve code completion sort order and auto insert `()` for functions without parameters
* Fix bugs with workspace documentation parsing

### 0.1.8

* Show signatures on completion label
* More reliable unused variable and constant checking in documente
* Show workspace documentations and function signatures in completions

### 0.1.7

* Show documentations parsed from GDScripts in hover tips

### 0.1.6

* Reorder mouse hover tips, builtin methods are at top of workspace methods
* Show callabel signatures with documente symbols and workspace symbols
* Syntax highlight support for signal parameters

### 0.1.5

* Add function signature hint support
* Better syntax grammar checking
* Better hover hint message for workspace methods and signals

### 0.1.4

* Add documentation support for builtin Symbols.
* Improve speed of syntax parsing and other actions

### 0.1.3

* Better syntax highlight for GDScript
* Add mouse hover information support
* Add definition provider for GDScript

### 0.1.2
* Multiline string and `StringName` highlight support
* Builtin classes, properties, functions and constants highlight support
* Fix errors in code snipt

### 0.1.1
* Better syntax highlight with GDScript

### 0.1.0
* Initial release
