# Model Editing

CHITUBOX provides a variety of common tools for editing 3D models to prepare them for printing.

## Hollow

Hollowing a model can reduce the amount of material used during printing.

Options explained:

-   **Wall Thickness**: Adjust the thickness of the walls.
-   **Precision**: Density of the generated triangles.
-   **Mode**: there are 3 modes available: Inner, Outer, and Bottom through. Inner mode will hollow out the model from the inside, Outer mode will peel off a designated thickness of wall from the model, and Bottom through is similar to Inner mode but also hollows out the bottom of the model.
    -   Infill: adding infill to the hollowed area can improve strength and model stability. There are three infill types (Scaffold, Hive, and Grid).
    -   Keep the Main Cavity: generates one single cavity during the hollowing operation.

## Drill

Drill holes in the model, typically used to allow resin to escape during printing.

## Duplicate

Duplicate allows you to create copies of the selected model, with designated number, spacing and layout.

## Mirror

Mirror selected model along the specified axis.

## Split

Split the selected model into multiple objects by checking geometry integrity and intersections. If your model is geometrically composed of multiple isolated parts, this feature can help you separate them for easier manipulation.

Let's create a geometrically intersected model for better clarity.

Open any 3D modeling software that you're familiar with, I will use Blender as an example, create 3 cubes that intersect with each other.

![Intersected cubes](../../../../../public/images/docs/en-US/chitubox/1.x.x/model-editing-000.png)

Once done, export them as a single STL file, and import it into CHITUBOX, apply the Split operation, and you will see the separated cubes.

![Separated cubes](../../../../../public/images/docs/en-US/chitubox/1.x.x/model-editing-001.png)

## Cut

### Plane Cut

**Options and Functions:**

* Add Cut Plane:

  Generate a cut plane by drawing a line crossing model(s). A new cut plane is generated perpendicular to the current view and through the line.

* Delete:

  Remove the cut plane.

* Cut Plane Transform: 

  Move of Change the Cut Plane by user inputs. Here  is used to switch between global coordinate system and local coodinate system.

* Align to Surface:

  Quickly align the cut plane to a selected model surface.

  You can also modify the location, angle and size of the cut plane in the model space.

**Apply Cutting:**

By clicking on apply, CHITUBOX will attempt to cut all **selected models**. At least one model needs to be selected for the cut to be applied.

![cut not allowed](../../../../../public/images/docs/en-US/chitubox/latest/model-editing/cut-not-allowed.png)

	A red cut surface means that the cut surface cannot be generated. This may due to the cut plane not fully crossing the entire model. Modify the cut plane before apply the cut.

**Connector Settings:**

* Connector

  By checking the connector box, you can generate connectors on the cut surfaces.

* Type

  Set the shape of the connecting key, including Pyramid Shaped or Connical Shaped.

* H 

  Set the overall height of the connectors.

* D1 

  Set the bottom width (Pyramid Shaped) or diameter (Connical Shaped) of the connectors.

* Geometry Definition

  There are two ways to define the overall geometry of the connecting key.

	* A 

	Define the geometry by inputing the angle between the side wall and the cut surface.

	* A 

	Define the geometry by inputing the width or geometry of the top surface of the connector key.

* T 

  Set the tolerance between the key and hole. This defines the spacing between sides walls of the key and sides walls of the hole. Input this number based on actual material requirement. Please note that the value may needs to be negative for some materials with high shrinkage rate when cured. We recommend starting with the default value of 0.1mm for general tough resin applications.

* I 

  Set the minimum distance between the axis of each key generated.

* Q 

  Set the maximum number of keys generated on the surface. Note that the cut surface may not be large enough to generate desired number of keys.

* Flip

  Reverse the direction of the key and hole generated. 

* Delete All

  Delete all connectors generated.

* Refresh

  Regenerate connectors after modifying connector parameters.

**Modify Connectors:**

Preview of connectors will be generated on the cut surface with the connector option checked.

You can modify any connector parameters and click on Refresh to regenerate all connectors.

By Selecting any connector, you can move the individual connector on the cut surface or modify the parameter of the selected connector alone. Parameter modifications of selected connectors will take effect immediately. 

Resulting connectors will be generated when the cut is applied.
### Free Cut
The free-cutting function allows you to precisely define the cutting plane and freely position the anchor points, enabling flexible model splitting based on actual printing and assembly requirements.

Step 1：
Please draw the cutting path at the intended location.

Step 2：
Drag anchor points of the cutting path on the model suface to adjust the cutting suface. You can also add extra points and
adjust them.

## Boolean

Boolean operations allow you to apply boolean logic to two models, such as union, difference, and intersection.

## Text Label

The Text Label tool allows you to add text labels to your model, which can be useful for identification or annotation purposes.

## Combine Models

The Combine Models feature allows you to merge multiple models into a single model after adding supports, and add an overall protective case for them.

## Align

The Align feature allows you to align separated parts. You can also freely combine different parts according to actual printing needs.

## Fill Cavity

The Fill Cavity feature allows you to select one or more cavities and fill them to create a solid model.

## Part  

The Part feature allows you to split a model into multiple independent parts.