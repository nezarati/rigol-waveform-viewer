# Advanced Rigol .wfm Waveform Viewer

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
![Maintained: Yes](https://img.shields.io/badge/Maintained%3F-yes-green.svg)

🌐 **Try it Live**: [**nezarati.github.io/rigol-waveform-viewer**](https://nezarati.github.io/rigol-waveform-viewer/index.html)

A powerful, self-contained HTML-based tool for viewing and analyzing binary waveform files (`.wfm`) from Rigol oscilloscopes. This viewer runs entirely in your web browser with zero installation, providing an immediate, cross-platform solution for engineers, students, and hobbyists.

It extends basic viewing with a rich set of features for in-depth analysis, professional-grade exporting, and easy annotation.

***

## Screenshot

![Screenshot of the Advanced Rigol .wfm Waveform Viewer](screenshot.png)

***

## Key Features

### 📂 File Handling
* **Load Files**: Open `.wfm` files via the "Load" button or by **dragging and dropping** them onto the page.
* **Multi-File Support**: Load multiple files simultaneously, each managed in a separate **tab**.
* **File Information**: The sidebar displays the current filename and total number of data points.

***

### 📈 Waveform Display & Interaction
* **Interactive Panning & Zooming**:
    * **Pan (Horizontal)**: `Shift` + `Mouse Wheel`
    * **Zoom Time (X-Axis)**: `Ctrl` + `Mouse Wheel`
    * **Zoom Voltage (Y-Axis)**: `Ctrl` + `Shift` + `Mouse Wheel`
    * **Area Zoom**: Click and drag to select and zoom into a specific region.
* **View Controls**:
    * **Reset View**: Double-click the plot or press `F` to fit the entire waveform into view.
    * **Snap to Scales**: Optionally snap zoom levels to standard oscilloscope time/voltage scales.
    * **Relative Time**: Set the start of the current view as $t=0$ for relative measurements.
* **Channel Management**:
    * Toggle channel visibility.
    * Swap the drawing order (bring a channel to the front).
    * Assign custom names and legends to each channel.

***

### 📏 Measurements & Analysis
* **Live Measurement Table**: An on-screen table displays key statistics for the *visible* portion of the waveform.
    * **Available Calculations**: **Max**, **Min**, **Average**, and **RMS** voltage.
    * **Customizable**: Toggle which measurements are displayed.
* **Cursor Measurements**:
    * Enable two horizontal and two vertical cursors for precise readouts.
    * Measures **$\Delta V$** (voltage difference), **$\Delta t$** (time difference), and frequency ($1/\Delta t$).
    * **Channel Tracking**: Cursors can "snap" to a selected channel's waveform.
    * **Quick Set**: Instantly move cursors to the max/min voltage points in the current view.

***

### ✒️ Annotations
* **Area Annotation**: Hold `Shift` + `Drag` to draw a persistent measurement box showing the region's $\Delta t$ and $\Delta V$.
* **Text Annotation**: Press `T` to enter text mode and click on the plot to add labels.
* **Manage Annotations**: Select annotations to move or resize them. Press `Delete` to remove a selected annotation.

***

### 📤 Exporting & Copying
* **Quick Copy**: Press `Ctrl` + `C` to copy the current view to the clipboard as a PNG image. A **"B&W Copy"** theme is available for high-contrast pastes.
* **Advanced Export Dialog**: Generate professional-grade output for reports or data processing.
    * **Formats**: **PNG**, **SVG** (vector), and **CSV** (raw data).
    * **Data Scope**: Export either the current zoomed-in view or the entire waveform dataset.
    * **Styling Options**:
        * **Black & White**: Creates a high-contrast, printer-friendly version.
        * **IEEE Style**: Formats the plot for academic publications (specific size, `10pt Times New Roman` font, simplified colors).
        * **Measurements Below Plot**: Option to place the measurement table neatly at the bottom.

***

## How to Use

1.  **Download**: Save the `index.html` file from this repository to your computer.
2.  **Open**: Open the file in a modern web browser (e.g., Google Chrome, Firefox, Edge).
3.  **Load**: Drag a `.wfm` file onto the page or use the "Load WFM File" button.

***

## Compatibility

This tool is designed to be compatible with `.wfm` files from a wide range of modern Rigol oscilloscopes. It has been tested with files from the following series:
* DS1000Z (e.g., DS1054Z)
* MSO5000

If your oscilloscope model is not listed, it is still likely to work. Please open an issue to confirm compatibility and help us update this list.

***

## Shortcuts

| Action | Shortcut |
| :--- | :--- |
| **View Control** | |
| Fit Waveform to View / Reset | `F` Key or `Double-Click` |
| Zoom to Area | `Mouse Drag` |
| Pan Horizontally | `Shift` + `Mouse Wheel` |
| Zoom Time (Horizontal) | `Ctrl` + `Mouse Wheel` |
| Zoom Voltage (Vertical) | `Ctrl` + `Shift` + `Mouse Wheel` |
| **Actions** | |
| Copy to Clipboard | `Ctrl` + `C` |
| Add Text Annotation | `T` Key |
| Create Area Annotation | `Shift` + `Mouse Drag` |
| Delete Selected Annotation | `Delete` Key |

***

## Contributing

Contributions are welcome! Please feel free to submit a pull request or create an issue for bugs, feature requests, or compatibility reports.

***

## License

This project is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

***

## Author

* **Ali NezaratiZadeh**
