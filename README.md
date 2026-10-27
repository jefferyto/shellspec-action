# ShellSpec action

A GitHub Action to run [ShellSpec].

[ShellSpec]: https://github.com/shellspec/shellspec

## Usage

Almost all of the available options correspond to ShellSpec's
[command-line options].

```yaml
- uses: jefferyto/shellspec-action@v1
  with:
    # The branch, tag or SHA of ShellSpec to use
    # Default: f2d13f9 (latest development version)
    shellspec-ref: ""

    # Relative path under $GITHUB_WORKSPACE for the root of the project
    # directory, i.e. where the ".shellspec" file is located
    project-root: ""

    # Specfile paths, directories, and/or patterns (relative to project
    # root, comma and/or newline separated) to pass to ShellSpec
    spec-paths: ""

    # Shell to run ShellSpec with
    # Default: "sh"
    shellspec-shell: ""

    # Prefix for names of artifacts uploaded by this action
    artifact-prefix: ""

    # Suffix for names of artifacts uploaded by this action
    artifact-suffix: ""

    # Shell to test with
    shell: ""

    # Modules (comma and/or newline separated) to require
    require: ""

    # Additional options file (relative to project root) to use
    options: ""

    # Paths (relative to project root, comma and/or newline separated)
    # to add to $SHELLSPEC_LOAD_PATH
    load-path: ""

    # Directory (relative to project root) to load helper files
    helperdir: ""

    # PATH environment variable to set at startup
    path-env-var: ""

    # Set to "true" to force the use of mocks instead of actual
    # commands, "false" to disable
    sandbox: ""

    # Sandbox path to set
    sandbox-path: ""

    # Execution directory of each specfile
    execdir: ""

    # List of environment variables (NAME=VALUE, comma and/or newline
    # separated) to set
    env-vars: ""

    # Shell script file (relative to project root) to use to set
    # environment variables
    env-from: ""

    # Set to "true" to treat warning as failure, "false" to disable
    warning-as-failure: ""

    # Abort the run after this number of failures, set to "0" to disable
    fail-fast: ""

    # Set to "true" to fail if no examples found, "false" to disable
    fail-no-examples: ""

    # Set to "true" to fail on low coverage, "false" to disable
    fail-low-coverage: ""

    # Run examples by this random type
    random: ""

    # Set to "true" to run examples with trace output of evaluation
    xtrace: ""

    # Set to "true" to run examples with trace output only
    xtrace-only: ""

    # Set to "true" to run focused groups/examples only
    focus: ""

    # Load files matching this pattern
    pattern: ""

    # Run examples whose names include this pattern
    example: ""

    # Run examples with this tag
    tag: ""

    # Default path to look for examples
    default-path: ""

    # Set to "true" to dereference all symlinks in specfile patterns
    dereference: ""

    # Set to "true" to enable coverage using kcov, "false" to disable
    kcov: ""

    # Additional kcov options (comma and/or newline separated)
    kcov-options: ""

    # Set to "true" to count the number of specfiles and examples
    count: ""

    # List these specfiles/examples
    list: ""

    # Set to "true" to check the syntax of specfiles
    syntax-check: ""

    # Set to "true" to output translated specfiles
    translate: ""

    # Set to "true" to show the task list
    task-list: ""

    # Run this task
    task: ""
```

[command-line options]: https://github.com/shellspec/shellspec#shellspec-cli

## License

MIT License

Copyright (c) 2026 Jeffery To

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
