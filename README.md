# Setting up a new device
I "Device configuration", legg til variabelen
`RESIN_HOST_CONFIG_lcd_rotate=2`

# Endre til lokale DNS-servere
sudo balena config write --type raspberrypi3 dnsServers '10.0.1.202 10.0.1.200'

# Andre prosjekter til inspirasjon:
https://github.com/futurice/chilipie-kiosk
https://github.com/balena-io-projects/balena-dash
https://github.com/balena-io-playground/x11-window-manager
https://github.com/balena-io-playground/balena-vnc-example
https://github.com/jayatvars/balena-chromium-kiosk
https://github.com/Aietes/docker-rpi3-kiosk

# Endre styrke på baklys
`echo 127 > /sys/class/backlight/rpi_backlight/brightness`

# Endre DNS-servere på host-os:
https://www.balena.io/docs/reference/cli/#config-read
add “dnsServers”: “XX.XX.XX.XX YY.YY.YY.YY” (space separated) in the config.json

# Test-URL'er for WPE
- https://www.khronos.org/registry/webgl/sdk/tests/webgl-conformance-tests.html
- http://www.bouncyballs.org
