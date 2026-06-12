# wayboard

`wayboard` is a libinput-based keyboard input display for Wayland.

# Building

The following dependencies are required only at build time:

- `wayland-protocols`

The following dependencies are required for both building and running:

- `fcft`
- `libconfig`
- `libinput`
- `libudev`
- `pixman`
- `wayland-client`

To build and install wayboard, clone the repository and run 
mkdir build && cd build && meson setup --prefix=/usr . .. && meson compile && meson install


> [!IMPORTANT]
> wayboard requires additional privileges to read keyboard input. If your user
> is not a member of the `input` group, you can set the setuid bit on the
> `wayboard` binary.
>
> ```
> # chmod u+s $(which wayboard)
> ```

# Configuration

Added razer_keypad.cfg for The Razer Tartarus Pro.
Added razer_keypad.cfg for the Razer Naga Trinity.

# Running
wayboard razer_keypad.cfg
