girara - user interface library
===============================

girara is a library that implements a user interface that focuses on simplicity
and minimalism. It consists of three main components: The view is a widget that
represents the actual application (e.g.: a web site or a document). The input
bar is used to execute commands of the application, while the status bar
notifies the user with current information. It is designed to replace and the
enhance the user interface that is used by zathura.

Requirements
------------

The following dependencies are required:

* `gtk3` (>= 3.20)
* `glib` (>= 2.50)

The following dependencies are optional:

* `libnotify`: notification support
* `json-c`: configuration dumping support

For building girara, the following dependencies are also required:

* `meson` (>= 0.56)
* `gettext`

The following dependencies are optional build-time only dependencies:

* `check` (>= 0.11): for tests
* `doxygen`: HTML documentation

To disable the optional support for `libnotify` and `json-c`, configure the build
system with `-Dnotify=disabled` or `-Djson=disabled`.

Installation
------------

Run the following command to build and install girara to your system using
meson's ninja backend:

    meson build
    cd build
    ninja
    ninja install

Note that the default backend for meson might vary based on the platform. Please
refer to the meson documentation for platform specific dependencies.

Bugs
----

Please report bugs at https://git.pwmt.org/pwmt/girara.
