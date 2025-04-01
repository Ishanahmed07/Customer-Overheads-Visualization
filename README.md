# Customer Overheads Visualization

This repository contains the code and documentation for **COMP1800 Data Visualisation Coursework**, a project focused on visualizing relationships between customer data, overhead costs, and company size using interactive scatter plots. The project leverages Python libraries such as Pandas, Holoviews, and Bokeh to create a bubble chart where the x-axis represents customers, the y-axis represents overheads, and bubble size reflects company size.

## Project Overview
The goal of this project is to explore and visualize a dataset containing customer-related metrics (`customer`, `overheads`, `size`, `staff`, `marketing`) using an interactive scatter plot. The visualization includes hover tooltips displaying all column values and supports undo/redo functionality for user interaction.

### Key Features
- **Data Preprocessing**: Loads and manipulates data using Pandas, adding a `BubbleSize` column scaled from `size`.
- **Visualization**: 
  - Interactive scatter plot built with Holoviews and Bokeh.
  - X-axis: `customer`, Y-axis: `overheads`, Bubble size: `size * 0.5`.
  - Hover tooltips show all columns: `customer`, `overheads`, `BubbleSize`, `index`, `marketing`, `size`, `staff`.
  - Tools: Undo, Redo, Pan, Zoom, Save.
- **Libraries**: Pandas, Numpy, Holoviews, Bokeh, hvPlot.

## Dataset
The dataset is embedded within the notebook as a `ColumnDataSource` object (from Bokeh). It includes 40 rows with columns: `customer`, `overheads`, `size`, `staff`, and `marketing`. The `BubbleSize` column is derived by scaling `size` by 0.5.

## Requirements
To run this project, install the required Python packages:
```bash
pip install pandas numpy holoviews hvplot bokeh
