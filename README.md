# linux
tips &amp; tricks to remember for myself

(https://www.linuxbabe.com/desktop-linux/switch-intel-nvidia-graphics-card-ubuntu)
https://askubuntu.com/questions/1117153/how-enable-use-geforce-mx150

Alternatively, you can open your terminal and write the command

`prime-select query`
to check which of the cards is your system using, and the commands

`sudo prime-select nvidia`
or

`sudo prime-select intel`
to change between the two cards and then restart the session.

Note: this didn't turn disable the gpu. Use powertop to manually adjust afterwards




**gpg keyserver receive failed: server indicated a failure**
Add google dns server to resolv.conf (located at /etc/resolv.conf)
`nameserver 8.8.8.8 #google dns server`



**Jetbrains tools not working in tiling WM (e.g bspwm)**
https://github.com/swaywm/sway/issues/595
Solution:
`wmname LG3D`

**Bspwm: Super + Space to trig dmenu not working**
Solution:
If keyboard layout is changed, then it might not work. Changing back from norwegian to us-keyboard solved the issue.



**Volume adjust using terminal**
pactl set-sink-volume @DEFAULT_SINK@ -10% (decrease by 10%)
