# Change Log

## 0.2

### 0.2.4

- Improved error reporting for exceptions in DaCe.
- Allows multi-selection of elements (nodes / edges) in the graph view via
  Ctrl. + Click or box-select.
- Now grouping applicable transformations for relevance to the selected
  elements.

### 0.2.3

- Improved error reporting and recovery.
- Allows for a retry when the startup of the DaCe backend failed.
- Clears transformations when the document is changed.

### 0.2.2

- Fixes missing info contents in the info bar.

### 0.2.1

- Switched the renderer to a separate submodule with the DaCe webclient.
- Implemented a way to start and connect to a DaCe Python daemon running in the
  background.
- Give the user an option to download and install DaCe if it's missing on the
  system.
- Provide a list of appicable transformations when viewing an SDFG.
  - Auto sort the list with relevance to the current viewport, whenever a zoom
    or pan action is detected in the viewer.
  - Provide a means to manually update the list.
  - Provide a means to preview transformations on the graph by clicking them.
  - Provide a means of applying transformations by clicking the dedicated apply
    button next to a transformation.
  - List the transformation's description in the tooltip.
  - Provide a list of previously applied transformations to the SDFG.
  - Provide a means to preview previous states of the SDFG by clicking a
    transformation in the history.
  - Provide a means to jump back in time by clicking the apply button next to a
    transformation in the history.

## 0.1

### 0.1.11

- Updated the renderer with a new version as found in upstream DaCe.
- A number of improvements to the `Go to source` functionality:
  - `Go to source` buttons now show a tooltip on hovering, indicating what file
    and line the code is located at.
  - If the `Go to source` button fails to find the file referenced, it will now
    display an error notification as well as the expected file path.
  - The `Go to source` button can now handle absolute paths.

### 0.1.10

- Added back language support to automatically suggest the extension for SDFG
  files.

### 0.1.9

- Added jump to (Python) source functionality for tasklets.

### 0.1.8

- Made canvas resize correctly when VSCode window or editor is resized.

### 0.1.7

- Inherit SDFV button styles from VSCode
- Inter-State edges are now color friendlier
- Added DaCe to the plugin name for visibility and discoverability

### 0.1.6

- Translation and zoom is retained upon external reloading of the SDFG
- Draggable splitter behavior improvements w.r.t. snapping, minimum
  sizes, and dragging out of bounds

### 0.1.5

- Added draggable separator bar to resize canvas/info-box
- Removed obsolete scrollbars and changed layout to flexbox layout

### 0.1.4

- Added dark mode support (no canvas background)
- Added SDFG file (`.sdfg`) icons

### 0.1.0

Initial release of SDFV for VS Code