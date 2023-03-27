# README

Welcome to this private Warp workflow files repository on GitHub. This repository contains several workflows that have been built using YAML syntax. Each workflow has a unique purpose and is available for non-commercial use under the Creative Commons License.

Here is a brief overview of the workflows to find in this repository:

## Worfklows

### macOS specific

* `homebrew.yml` - Upgrade Homebrew and cleanup old versions.

## File Format

A comprehensive official description from [Warp](https://github.com/warpdotdev/workflows).

```yaml
# The name of the workflow.
name: Uninstall a Homebrew package and all of its dependencies
# The corresponding command for the workflow. Any arguments should be surrounded with two curly braces. E.g `command {{arg}}`.
command: |-
    brew tap beeftornado/rmtree
    brew rmtree {{package_name}}
# Any tags that the workflow should be categorized with.
tags:
  - homebrew
# A description of the workflow.
description: Uses the external command rmtree to remove a Homebrew package and all of its dependencies
# List of arguments within the command.
arguments:
    # Name of the argument within the command. This must exactly match the name of the argument
    # within the command (without the curly braces).
  - name: package_name
    # The description of the argument.
    description: The name of the package that should be removed
    # The default value for the argument.
    default_value: ~
# The source URL for where the workflow was generated from, if any.
source_url: "https://stackoverflow.com/questions/7323261/uninstall-remove-a-homebrew-package-including-all-its-dependencies"
# The author of the workflow.
author: Ory Band
# The URL of original author of the Workflow. For example, if this workflow was generated from StackOverflow, the `author_url` would be the StackOverflow author's profile page.
author_url: "https://stackoverflow.com/users/207894"
# The valid shells where this workflow should be active. If valid for all shells, this can be left empty.
# See FORMAT.md for the full list of accepted values.
shells: []
```

The official documentation from Warp can be found [here](https://docs.warp.dev/features/entry/workflows#creating-custom-workflows).

All workflows in this repository are available under the Creative Commons License for Non-Commercial Use. This means that you are free to use, modify, and share these projects as long as it is for non-commercial purposes. If you wish to use these dotfiles for commercial purposes, please contact the owner of this repository for licensing information.

If you have any questions or feedback, please do not hesitate to reach out to the owner of this repository.

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">
    <img
        alt="Creative Commons License"
        style="border-width:0"
        src="https://i.creativecommons.org/l/by-nc/4.0/80x15.png"
    />
</a>
<br />
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
