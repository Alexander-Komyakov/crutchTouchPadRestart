## crutchTouchPadRestart
# Touch Pad Restart
This solves the problem of the laptop in the touchpad turning off.
## Bug i2c_hid_acpi
`modprobe -r i2c_hid_acpi`
`modprobe i2c_hid_acpi`

## enable response to touch
`synclient TapButton1=1`

`synclient TapButton2=3`

## disable touchpad while typing
`syndaemon -i 0.2 -d`

# Installing

`# cd crutchTouchPadRestart`

`# cp touchpadrestart /usr/local/bin`

`# cp tpadrestart.service /etc/systemd/system`

`# systemctl start tpadrestart.service`

`# systemctl enable tpadrestart.service`

# Created by Alexander Komyakov
For any kind of help, support, suggetion and request ask in me
## Follow on:
<p align="left">
<a href="https://github.com/Alexander-Komyakov"><img src="https://img.shields.io/badge/GitHub-Follow%20on%20GitHub-inactive.svg?logo=github"></a>
</p><p align="left">
<a href="https://vk.com/shurikkomyakov"><img src="https://img.shields.io/badge/VK-Follow%20on%20Vkontakte-blue?logo=vk&logoColor=white"></a>
</p><p align="left">
