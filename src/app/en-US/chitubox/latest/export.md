# Export

## Export Models

The export feature allows you to save your 3D model in various 3D mesh formats (stl, obj, 3mf), making it compatible with different 3D software and services.

	If you want to save your CHITUBOX Project, go to `Main Menu > Save Project`
	instead.

## Slice Models for Printing

This is where you slice your 3D model into printable layers, and export the sliced file in a format compatible with your 3D printer.

Before exporting, select the slicing mode in the Parameter Panel. CHITUBOX offers 4 slicing modes:

-   Single Parameter Slice: This mode allows you to set a single slicing parameter (layer height, exposure time, etc.) for the entire model.
-   Slicing by Model: This mode allows you to set different slicing parameters for different objects, note that setting exposure time for each object individually is not supported currently, but you can set **Picture Grayscale** for each object as a workaround.
    -   In the **Grouping Parameter Configuration** panel, you define available individual configurations, then in **File Grouping Panel**, you assign configurations to each object.
-   Slicing by Height: This mode allows you to set different slicing parameters based on the height of the model.
-   Slicing by Cross-sectional Area: This mode allows you to set different slicing parameters based on the cross-sectional area (exposure area) of individual layers. You can define different cross-sectional area intervals, and layers that meet the specified area criteria will use the corresponding configuration.
