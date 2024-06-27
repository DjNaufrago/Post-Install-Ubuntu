Type in terminal:
`sudo pluma /usr/share/glib-2.0/schemas/30_ubuntu-mate.gschema.override`

Edit line 2, replacing the path with the one to your wallpaper and save the changes.
For example, change this:
`background='/usr/share/backgrounds/ubuntu-mate-jammy/Jammy-Jellyfish_WP_4096x2304_Green.png'`
For this:
`background='/usr/share/backgrounds/ubuntu-mate-photos/gabriele-diwald-201135.jpg'`

Save and type:
`sudo glib-compile-schemas /usr/share/glib-2.0/schemas/`
