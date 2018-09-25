# CMake GUI Here for Nemo

## Install

1. Add the following to `~/.config/Thunar/uca.xml`

    ```xml
    <action>
        <icon></icon>
        <name>CMake GUI Here</name>
        <!-- You might need to change this value -->
        <unique-id>1537910568312016-8</unique-id>
        <!-- Replace 'cmake-gui' with the path to cmake-gui if necessary -->
        <command>cmake-gui &quot;-H$(echo %f)&quot; &quot;-B$(echo %f)/build&quot;</command>
        <description></description>
        <patterns>*</patterns>
        <startup-notify/>
        <directories/>
    </action>
    ```

## Usage

1. Right-click on the "background" of a directory containing a `CMakeLists.txt` file
1. Choose `CMake GUI Here`

## Uninstall

1. Remove the added `<action>` node that contains `CMake GUI Here` from `~/.config/Thunar/uca.xml`

## Credit

* https://classicforum.manjaro.org/index.php?topic=17759.0
