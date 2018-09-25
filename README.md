# CMake Context Menu Item

A collection of scripts that add context menu items for launching CMake from the OS file manager.

# Supported File Managers

* Linux
  * Dolphin
  * Nautilus
  * Nemo
  * Thunar
* Windows
  * Windows File Explorer

# Contributing

Bug fixes and pull requests (e.g. adding support to more file managers) are welcome :)

For the "CMake GUI Here" menu item, the main _trick_ is to launch  `cmake-gui` with the following arguments

  ```sh
  cmake-gui "-H<path to current folder>" "-B<path to current folder>/build"
  ```

Note that

* `"-H..."` and `"-B..."` are quoted
* There are **no spaces** after `-H` and `-B`
