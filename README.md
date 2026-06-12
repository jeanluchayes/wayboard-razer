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
- `mkdir build && cd build && meson setup --prefix=/usr . .. && meson compile && meson install`


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
- `wayboard razer_keypad.cfg`

# Image:
<img width="1106" height="560" alt="image" src="https://github.com/user-attachments/assets/61a0caa3-23a1-4724-8f9c-42baa5681fa4" />
I colored the background green so it could key the background out in OBS.

I can't take a picture of the red timing text on the keys as it is too fast, but you can see when a key is pressed down quickly vs when its held down.
Held-down keys stay grey; quickly pressed keys get red text on them.

Video Demo:
https://youtu.be/1soldt7AIXs?si=4RFlUyZqXvnFlfyE
