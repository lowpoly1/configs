# set modifier to the meta key
set $mod Mod4

# hide window borders
new_window pixel 0
for_window [class="^.*"] border pixel 0
default_border none
default_floating_border none

# set gaps
gaps inner 8
gaps outer 2

# to move floating windows
floating_modifier $mod

# switch to workspace
bindsym $mod+1    workspace  $ws1
bindsym $mod+2    workspace  $ws2
bindsym $mod+3    workspace  $ws3
bindsym $mod+4    workspace  $ws4
bindsym $mod+5    workspace  $ws5
bindsym $mod+6    workspace  $ws6
bindsym $mod+7    workspace  $ws7
bindsym $mod+8    workspace  $ws8
bindsym $mod+9    workspace  $ws9
bindsym $mod+0    workspace  $ws10

# switch to workspace with numpad keys
bindcode $mod+87 workspace 1
bindcode $mod+88 workspace 2
bindcode $mod+89 workspace 3
bindcode $mod+83 workspace 4
bindcode $mod+84 workspace 5
bindcode $mod+85 workspace 6
bindcode $mod+79 workspace 7
bindcode $mod+80 workspace 8
bindcode $mod+81 workspace 9
bindcode $mod+90 workspace 10

# switch to workspace with numlock numpad keys
bindcode $mod+Mod2+87 workspace $ws1
bindcode $mod+Mod2+88 workspace $ws2
bindcode $mod+Mod2+89 workspace $ws3
bindcode $mod+Mod2+83 workspace $ws4
bindcode $mod+Mod2+84 workspace $ws5
bindcode $mod+Mod2+85 workspace $ws6
bindcode $mod+Mod2+79 workspace $ws7
bindcode $mod+Mod2+80 workspace $ws8
bindcode $mod+Mod2+81 workspace $ws9
bindcode $mod+Mod2+90 workspace $ws10

# move focused container to workspace
bindsym $mod+Shift+1    move container to workspace  $ws1
bindsym $mod+Shift+2    move container to workspace  $ws2
bindsym $mod+Shift+3    move container to workspace  $ws3
bindsym $mod+Shift+4    move container to workspace  $ws4
bindsym $mod+Shift+5    move container to workspace  $ws5
bindsym $mod+Shift+6    move container to workspace  $ws6
bindsym $mod+Shift+7    move container to workspace  $ws7
bindsym $mod+Shift+8    move container to workspace  $ws8
bindsym $mod+Shift+9    move container to workspace  $ws9
bindsym $mod+Shift+0    move container to workspace  $ws10

# move focused container to workspace with numpad keys
bindcode $mod+Shift+Mod2+87 	move container to workspace  $ws1
bindcode $mod+Shift+Mod2+88 	move container to workspace  $ws2
bindcode $mod+Shift+Mod2+89 	move container to workspace  $ws3
bindcode $mod+Shift+Mod2+83 	move container to workspace  $ws4
bindcode $mod+Shift+Mod2+84 	move container to workspace  $ws5
bindcode $mod+Shift+Mod2+85 	move container to workspace  $ws6
bindcode $mod+Shift+Mod2+79 	move container to workspace  $ws7
bindcode $mod+Shift+Mod2+80 	move container to workspace  $ws8
bindcode $mod+Shift+Mod2+81 	move container to workspace  $ws9
bindcode $mod+Shift+Mod2+90 	move container to workspace  $ws10

# move focused container to workspace with numpad keys
bindcode $mod+Shift+87 	 move container to workspace  $ws1
bindcode $mod+Shift+88 	 move container to workspace  $ws2
bindcode $mod+Shift+89 	 move container to workspace  $ws3
bindcode $mod+Shift+83 	 move container to workspace  $ws4
bindcode $mod+Shift+84 	 move container to workspace  $ws5
bindcode $mod+Shift+85 	 move container to workspace  $ws6
bindcode $mod+Shift+79 	 move container to workspace  $ws7
bindcode $mod+Shift+80 	 move container to workspace  $ws8
bindcode $mod+Shift+81 	 move container to workspace  $ws9
bindcode $mod+Shift+90 	 move container to workspace  $ws10

# change focus
bindsym $mod+j focus left
bindsym $mod+k focus down
bindsym $mod+b focus up
bindsym $mod+o focus right

# alternatively, you can use the cursor keys:
bindsym $mod+Left focus left
bindsym $mod+Down focus down
bindsym $mod+Up focus up
bindsym $mod+Right focus right

# move focused window
bindsym $mod+Shift+j move left
bindsym $mod+Shift+k move down
bindsym $mod+Shift+b move up
bindsym $mod+Shift+o move right

# alternatively, you can use the cursor keys:
bindsym $mod+Shift+Left move left
bindsym $mod+Shift+Down move down
bindsym $mod+Shift+Up move up
bindsym $mod+Shift+Right move right

# split in horizontal orientation
bindsym $mod+h split h

# split in vertical orientation
bindsym $mod+v split v

# enter fullscreen mode for the focused container
bindsym $mod+f fullscreen toggle

# change container layout (stacked, tabbed, toggle split)
bindsym $mod+s layout stacking
bindsym $mod+g layout tabbed
bindsym $mod+e layout toggle split

# toggle tiling / floating
bindsym $mod+Shift+space floating toggle

# change focus between tiling / floating windows
bindsym $mod+space focus mode_toggle

# focus the parent container
bindsym $mod+a focus parent

# for resizing windows
mode "resize" {

        bindsym j resize shrink width 10 px or 10 ppt
        bindsym k resize grow height 10 px or 10 ppt
        bindsym l resize shrink height 10 px or 10 ppt
        bindsym ntilde resize grow width 10 px or 10 ppt
        
    	  bindsym Left resize shrink width 10 px or 10 ppt
        bindsym Down resize grow height 10 px or 10 ppt
        bindsym Up resize shrink height 10 px or 10 ppt
        bindsym Right resize grow width 10 px or 10 ppt

	      bindsym Return mode "default"
        bindsym Escape mode "default"
}
bindsym $mod+r mode "resize"

# set floating (nontiling) for apps needing it
for_window [class="Yad" instance="yad"] floating enable
for_window [class="Galculator" instance="galculator"] floating enable
for_window [class="Blueberry.py" instance="blueberry.py"] floating enable

# set floating (nontiling) for special apps
for_window [class="Xsane" instance="xsane"] floating enable
for_window [class="Pavucontrol" instance="pavucontrol"] floating enable
for_window [class="qt5ct" instance="qt5ct"] floating enable
for_window [class="Blueberry.py" instance="blueberry.py"] floating enable
for_window [class="Bluetooth-sendto" instance="bluetooth-sendto"] floating enable
for_window [class="Pamac-manager"] floating enable
for_window [window_role="About"] floating enable

# start a terminal
bindsym $mod+Return exec kitty

# kill focused window
bindsym $mod+q kill

# reload the configuration file
bindsym $mod+Shift+c reload

# restart i3 inplace (preserves your layout/session, can be used to update i3)
bindsym $mod+Shift+r restart

# audio controls
bindsym $mod+Shift+p exec playerctl play-pause
bindsym $mod+Ctrl+Left exec playerctl previous
bindsym $mod+Ctrl+Right exec playerctl next

# lock by blurring the screen:
bindsym $mod+l exec ~/.config/i3/scripts/blur-lock

# power menu
bindsym $mod+Shift+e exec ~/.config/i3/scripts/powermenu

# keybinding in fancy rofi (automated):
bindsym F1 exec ~/.config/i3/scripts/keyhint-2

bindsym $mod+d exec rofi -modi drun -show drun \
		-config ~/.config/rofi/rofidmenu.rasi

bindsym $mod+t exec rofi -show window \
		-config ~/.config/rofi/rofidmenu.rasi

# set background with feh
exec --no-startup-id feh --bg-scale ~/Pictures/background.jpg

# notifications via dunst
exec --no-startup-id dbus-launch dunst --config ~/.config/dunst/dunstrc

# picom for transparency
exec --no-startup-id picom -b

# get authorization with polkit-gnome
exec --no-startup-id /usr/lib/polkit-gnome/polkit-gnome-authentication-agent-1

# autostart apps
exec --no-startup-id dex --autostart --environment i3

# set powersavings for display
exec --no-startup-id xset s 480 dpms 600 600 600

# autotiling
exec_always --no-startup-id autotiling

# volume control
exec --no-startup-id pasystray
