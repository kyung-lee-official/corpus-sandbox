# Support Your Model

In this section we will focus on the support features of CHITUBOX, which are essential for ensuring successful 3D printing. Proper support structures can help prevent print failures and improve the overall quality of your models.

## Support Classification

CHITUBOX offers various support types to cater to different printing needs. Let's break down all these concepts.

### Support Segments

A support can be divided into several segments, each serving a specific purpose:

-    **Top**: the top support structure directly contacts
    the model.

-    **Main**: the main support structure provides stability
    to the model.

-    **Base**: the base support structure provides a foundation
    for the model.

-    **Raft**: the raft support structure provides a base
    for the model to print on.

-    **Snug**: the snug support structure connects to the
    model both above and below. It's typically used to support overhangs in areas
    where it's difficult to attach supports directly to the build plate.

-    **Cross Bracing**: the cross bracing support
    structure provides additional stability to the model by creating scaffolding-like
    support between supports.

### Independent Support

Independent Support refers to supports that only have a single top segment without forks on the top, it includes:

-   **Adaptive Support**: this type of support adaptively adds supports based on the model's geometry and overhangs.

-   **Vertical Support**: the top of the support is perpendicular to the model's contact surface.

-   **Upright Support**: the top of the support is generated straight up on the Main segment, perpendicular to the build plate.

### Forked Support

Forked Support refers to supports that have a top segment with forks, it allows multiple connections to the model, significantly reduceding the amount of supports needed. It includes:

-   **Branch Support**: top segment composed of multiple branches that can be adjusted to fit the model's geometry.

-   **Joint Support**: top segment generated upon an extra forked segment of a Main segment, appearing two segments above the Main segment. One on another is allowed.

-   **Small Support**: top segment's Lower Diameter is set to be identical as Upper Diameter when generated, make the top segment thin-pillar-like, but remain editable.

-   **Tree Support**: top segment generated upon an extra forked segment of a Main segment, similar to Joint Support, but can only generated on the Main segment. One on another is not supported.

There are some Forked Support specific parameters:

-   **Automatic Attachment**: check this option to allow top segments to be generated upon a nearest Main segment automatically.
    -   Attachment Radius: the radius of the area around the Main segment where the top segment can be attached automatically.
    -   Branching Angle: the maximum angle between the top segment and the upward extension of the Main segment at which the branches of the support can grow.

## Enhanced Settings

-   **Max. Contact Point Offset**: the maximum allowable distance between contact point and the support's Main segment, limiting generation long-top supports that may cause print failures.
-   **Min. Effective Support Height**: the minimum height that a support structure must have to be considered effective. The parameter Lower Diameter of Supports' Main segment will be be applied to supports generated below this height.
-   **Spacing from Model**: the minimum distance between the model and the support structure, helping to prevent the support from fusing to the model during printing.

## Edit Support

**Edit Support** allows you to modify existing support structures. Some values take effect immediately, while others maked with  require re-generation of the support structures to apply changes.

To Edit a Support Structure, first, enter "Edit Support" mode. Then, click on a support to select it. If you want to select a specific segment of the support, click the segment. Once selected, the Parameters Panel will display the editable parameters for that segment.

Some parameters can only be applied during generation and will not be saved. These parameters are marked as "Editable" instead of showing a specific value.

### To Export and Apply a Custom Configuration

To export a custom support configuration:

-   Select a support structure and make your desired changes.

-   In the Parameters Panel, click the "Export" button.

-   This will save the current configuration as a file (\*.cfgx) that can be imported later.

To apply this custom configuration to other supports:

-   Click the import button to import the configuration file (if you haven't already).

-   Select the target supports.

-   Click the "Apply" button in the Parameters Panel.

## Manual Support

**Manual Support** allows you to add support structures manually. This is useful for complex models where automatic support generation may not provide the best results.

## Batch Support

Batch Support offers a way to apply support structures to specific areas of the model.

-   **Area Selection**: provides different selection tools for selecting areas for auto support generation.
-   **Countour Support**: select the contour of the model to generate support structures on it.
-   **Face Support**: select a flat face of the model to generate support structures on it.
-   **Boundary Support**: similar to Face Support, but applies to the edges of the model only.

## Auto Support

Auto Support automatically generates support structures based on the model's geometry. It can save you time and effort in preparing your models for printing.

In **Auto Support**, you can adjust the **Contact Point Spacing** to change the density of the supports. Decrease this value to increase the support density.

## Magic Support

If your model has intricate designs or varying overhang angles, typically you will need to supports with various parameters to ensure a successful print. **Magic Support** is a feature that allows you to add supports with different parameters to your model in individual steps.

## Support Center

Support Parameter Center for managing support profiles and customizing the parameters displayed in support functions.

## Mirror Support

Mirror Support checks your model's symmetry, any symmetrical plane found will be listed in the Parameters Panel.

	Checking model symmetry can be time-consuming, especially for complex
	models. If your model lacks symmetry, we recommend skipping this step.

## Raft

Raft is literally a flat surface that the model is printed on. It helps to improve adhesion and can make it easier to remove the model from the build plate.

### Raft Type
Raft Type is used to select the shape of the raft, including Skate, Cross grid, Hexagonal grid, Bottom Connected, and Protective case.
Selecting None applies only the Model Lift Height, without generating a raft.

## Cross Bracing

Cross Bracing is a feature that adds additional support structures between existing supports to improve stability and reduce the risk of print failures. It can be particularly useful for tall or complex models.

## Merge Supports

Merge Supports allows you to combine multiple support structures into a single one. This can help reduce the number of supports needed and save resin.
