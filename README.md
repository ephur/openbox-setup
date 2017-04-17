# OpenBox Config & Tools

Collection of Scripts / Configs to make openbox behave how I want it in 2017...

I am not a fan of all the heavyweight desktops. Modern window managers/desktop environments provide a lot of functionality but 

### Requirements

Currently requires the following packages (ubuntu)
* openbox of course
* tint2
* suckless-tools

Currently requires the following python modules:
* requests (for weather API service)
* xlib (for wall paper swapping)

### Scripts
##### ob-lock

Just locks the screen, and after a small sleep puts the monitor to sleep. 

##### wp-switcher

Python script that is bound to all mouse/keyboard actions that swap virtual desktops. Allows a per virtual desktop background with openbox. Requires python xlib module. The script adds about two hundreths of a second to however long nitrogen (or whatever tool it's configured to use) takes to set the background. This makes for faster background swapping than any other method or tool I've tried

##### ob-weather (openbox pipe menu)

I know some people like weather widgets, but don't want that running all the time, so I just put it on a pipe menu, easy to get to this way and not using resources when not needed.

A python script that requires only requests python module. Metric units are not fully supported at the moment. It uses openweathermap.com for the source of data. You need to sign up and get an API key, only free functions are used. There's a cool python module for interacting with OWM, but for the operations I wanted it was a little heavy weight.

##### ob-cal (openbox pipe menu)

This was a text snipped I found somewhere via a google, fixed the cal output and saved it.

## Key Bindings

There are several key bindings setup for managing windows/desktops with this configuration. I find it very handy to be able to manage window positions in a 4x4 grid with the Win + Arrow keys. 

`WIN + r  : run dmenu, a text based 'run' menu`

`WIN + 1  :  switch to virtual desktop 1`
`WIN + 2  :  switch to virtual desktop 2`
`WIN + 3  :  switch to virtual desktop 3`

`CTRL + ALT + RIGHT   :  Move to the next desktop`
`CTRL + ALT + LEFT    :  Move to the previous desktop`
`SHIFT + WIN + RIGHT  :  Move current window to the next desktop, follow + focus`
`SHIFT + WIN + LEFT   :  Move current window to the previous desktop, follow + focus`

`WIN + d          :  minimize all / show desktop`
`SHIFT + WIN + d  :  minimize / iconify window`
`CTRL + ALT + l   :  lock the desktop & sleep monitor (5 seconds before sleep)`

`ALT + TAB          :  switch next window`
`ALT + SHIFT + TAB  :  switch previous window`
`ALT + F4           :  close window `
`WIN + SPACE        :  show window menu`

`WIN + RIGHT  :  move current window to right half of screen, 100% height, 50% width`
`WIN + LEFT   :  move current window to left half of screen 100% height, 50% width`
`WIN + UP     :  move current window to top of screen, 50% height, width unchanged`
`WIN + DOWN   :  move current window to bottom half of screen, 50% height, width unchanged`

