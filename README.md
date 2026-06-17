# DS5Settings

A free Windows app for configuring and testing a **[DS5Dongle](https://github.com/awalol/DS5Dongle)** —
the RP2350 / Pico 2 W adapter that bridges a Sony DualSense controller over Bluetooth to USB.

## Download

Grab the latest **`ds5settings.exe`** from the [**Releases**](../../releases) page. It's a
single file — no installer, no Python, nothing to set up. Just run it.

> **First run:** Windows SmartScreen may say *"Windows protected your PC"* because the app
> isn't code-signed. Click **More info → Run anyway**. (It's a small, unsigned hobby app —
> that warning is expected.)

## What it does

- **Settings** — change every dongle setting over USB: speaker/headset volume (applied live),
  gains, mic/speaker enable, polling rate, controller mode, and more; save to the dongle's flash.
- **Input Test** — see your controller live: buttons, sticks, d-pad, touchpad, triggers,
  gyro/accel, and factory motion-sensor calibration. Test rumble and adaptive triggers.
- **Firmware** — drag a `.uf2` onto the window to flash the dongle (once it's in BOOTSEL).
- **Troubleshooting** — clear stale Windows DualSense audio/HID entries; enable wake-on-PS.

## Requirements

- Windows 10/11 (64-bit)
- A [DS5Dongle](https://github.com/awalol/DS5Dongle) running firmware **v0.7.1** or newer,
  connected over USB

No admin rights for normal use (a couple of Troubleshooting actions prompt for UAC).

## Known issues

- **Rumble / adaptive-trigger test needs the speaker idle (firmware v0.7.1).** While Windows is
  using the dongle's speaker as the active playback device — or streaming audio to it — the
  controller ignores the rumble and trigger tests. Switch your Windows output to another device
  (or stop audio playback), then run the test.

## Found a bug?

Please open an [issue](../../issues) — include your Windows version, the dongle firmware
version, and what you were doing when it happened. Screenshots help.

## Support

If this is useful: [☕ Ko-fi](https://ko-fi.com/up2urheadlights)

## License

Free to use — see [LICENSE](LICENSE). Redistribution, modification, and reverse-engineering
are not permitted. Provided as-is, with no warranty.
