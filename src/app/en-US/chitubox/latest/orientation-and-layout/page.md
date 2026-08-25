# Orientation and Layout

## Orientation

Set the orientation for the selected 3D model automatically before adding supports.
The line defined by two points with the longest distance on the surface of the model
will be considered as the vertical axis when applying auto orientation.

## Layout

Set the layout for the selected 3D model automatically before adding supports.
The layout defines how the model will be positioned and oriented on the build plate.

CHITUBOX supports multi-platform layouts, if your current build plate can't accommodate all objects, additional platforms will be automatically created to fit everything.

	If the size of a single model exceeds the build plate limits, CHITUBOX simply move it out of the build plate, and will not automatically create a new platform for it.

Options explained:

-   Loop Layout: whether to layout objects in line-by-line sequence or a looped sequence.

-   Layout Scope: this options sets offsets for the build plate limit auto-layout area.
