# ZMK Config

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/issmirnov/zmk-config)

Use https://nickcoutsos.github.io/keymap-editor/ to edit.

See [Actions output](https://github.com/issmirnov/zmk-config/actions) for firmware downloads.

## ZMK Version

This config uses **official ZMK v0.3.0** for stability and travel reliability.

### Display Optimization Note

The caksoylar/SethMilliken fork provides e-ink display optimizations (periodic full refresh, alternative refresh patterns, custom widgets) but is currently incompatible with ZMK v0.3.0 due to LVGL 9 API changes. The display optimization config options are commented out in `corneish_zen.conf` - uncomment them if switching to a compatible fork.

See [caksoylar's gist](https://gist.github.com/caksoylar/c411313990978e1903c244f03039187a) for details on display improvements.

### Upgrading ZMK

To upgrade to a newer version:
1. Update `config/west.yml`: change `revision: v0.3.0` to the new tag
2. Update `.github/workflows/build.yml`: change `@v0.3.0` to match
3. Push and verify the build succeeds

## Rendered Keymap

(using https://github.com/caksoylar/keymap-drawer)

![layout](keymap-drawer/corneish_zen.svg)
