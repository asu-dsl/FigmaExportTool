# Component Export Tool for Figma

A simple plugin to export Figma components with customizable prefixes and formats.

## Installation

1. Download the latest release from the GitHub releases section
2. Unzip the package to your preferred location
3. In Figma, go to Plugins > Development > Import plugin from manifest
4. Navigate to the unzipped folder and select the manifest.json file

<img src="https://i.imgur.com/17awNvf.png" width="50%" alt="Import Plugin">

## Usage

1. Select the component(s) you want to export in Figma
2. Open the plugin via Plugins > Component Export Tool

<img src="https://i.imgur.com/h6CReUM.png" width="50%" alt="Load Plugin">

3. Configure your export settings:
   - Prefix: Add a prefix to all exported files (defaults to 'ui_')
   - Custom filename: Available for single selection only
   - Format: Choose between PNG, JPG, SVG, or PDF
   - Scale: Set export scale (not applicable for SVG)

<img src="https://i.imgur.com/H2ZNmgV.png" width="50%" alt="Export UI">

4. Click "Export Selected" to start the export process

## Multiple Selection

When multiple components are selected:
- Custom filename is disabled
- Files are exported using the prefix + original component name
- Exports happen sequentially to ensure reliability

## Settings

Access the settings panel via the gear icon to:
- Set a default prefix for all exports
- Configure export path
- Settings are saved between sessions

## Notes

- The plugin handles one export at a time to ensure reliability
- Progress bar shows export status for multiple selections
- SVG exports automatically disable scale options
