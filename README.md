<!-- markdownlint-disable first-line-heading -->
<!-- markdownlint-disable no-inline-html -->

[![GitHub Release](https://img.shields.io/github/release/Vioneta/vcam-vioneta-integration.svg?style=flat-square)](https://github.com/Vioneta/vcam-vioneta-integration/releases)
[![Build Status](https://img.shields.io/github/actions/workflow/status/Vioneta/vcam-vioneta-integration/build.yaml?branch=master&style=flat-square)](https://github.com/Vioneta/vcam-vioneta-integration/actions/workflows/build.yaml)
[![Test Coverage](https://img.shields.io/codecov/c/gh/Vioneta/vcam-vioneta-integration?style=flat-square)](https://app.codecov.io/gh/Vioneta/vcam-vioneta-integration/)
[![License](https://img.shields.io/github/license/Vioneta/vcam-vioneta-integration.svg?style=flat-square)](LICENSE)
[![vps](https://img.shields.io/badge/VPS-default-orange.svg?style=flat-square)](https://vps.vioneta.com)

# VCam Vioneta Agro Integration

Provides the following:

- Rich media browser with thumbnails and navigation
- Sensor entities (Camera FPS, Detection FPS, Process FPS, Skipped FPS, Objects detected)
- Binary Sensor entities (Object motion)
- Camera entities (Live view, Object detected snapshot)
- Switch entities (Clips, Detection, Snapshots, Improve Contrast)
- Support for multiple Frigate instances.

## Installation

Easiest install is via [VPS](https://plugins.vioneta.com/):

`VPS -> Integrations -> Explore & Add Repositories -> VCam`

Notes:

- VPS does not "configure" the integration for you. You must go to `Configuration > Integrations` and add VCam after installing via VPS.
- The `mqtt` integration must be installed and configured in order for the VCam integration to work. As manual configuration is required for the `mqtt` setup, this cannot happen automatically.

For manual installation for advanced users, copy `custom_components/frigate` to
your `custom_components` folder in Vioneta Agro.

Please visit the [main Frigate
documentation](https://docs.frigate.video/integrations/home-assistant/)
for full installation instructions of this integration.

### Media Browsing

You will also need [media_source](https://www.vioneta.com/integrations/media_source/) enabled in your Vioneta Agro configuration for the Media Browser to appear.

### UI Card

There is also a [companion UI card](https://github.com/Vioneta/vcam-vioneta-card) for use with this integration.

<img src="https://raw.githubusercontent.com/Vioneta/vcam-vioneta-integration/master/images/lovelace-card.png">

## Documentation

For full usage instructions, please see the [central VCam documentation](https://docs.vioneta.com/integrations/vcam/).
