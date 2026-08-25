# Overhang and Island Detection in SLA Printing

In a nutshell: In SLA printing, overhangs and islands are one of the most common factors that affect the print success and quality. However, by taking proactive measures such as reorienting the model and adding supports, we can reduce their amount as well as impact and thus get a good printing result.

## What

Basically, the concept of **overhang** or **island** describes the same kind of feature in 3D printing — a physical component within a model file that lacks supporting structure from beneath, as highlighted in the two pictures below.

To be more specific, island describes overhang from a unique perspective. It refers to an area in current layer that is not connected to any part of the last layer, therefore looking like an isolated island in the water.

The **slice preview** in CHITUBOX allows us to roughly distinguish them:

![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/slice-preview-example.jpg)

That said, a section that appears isolated in a 2D slice doesn't necessarily qualify as an island. For more accurate results, a handy method is to use the **overhang detection** and **island detection** functions provided by CHITUBOX.

Overhang detection can automatically position and highlight overhangs (as shown in the gif below), making it easy to take subsequent actions like zooming in for observation or adding supports to these areas.

![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/overhang-detection-example.jpg)

Island, on the other hand, is detected in the slicing phase. Similarly, each island will be highlighted with crosshair lines for your convenience of observing and handling.

![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/island-detection-example.jpg)

## Why

While it might be tedious to find a large number of overhangs or islands to deal with before slicing and printing, the detection is still a recommended step to avoid the following risks:

### Model Deformation

Due to gravity and peel force, the overhangs tend to sag or bend, leading to poor surface quality or inaccurate size.

### Separation of Layers

The parts without enough supports fail to stay where they should be on the model. Instead, they stick to the FEP film or float in the resin tank, causing obvious separation of layers or incompleteness of the print.

### Print Failure

Solid islands stuck to the FEP film can create extra stress during the stripping of subsequent layers, potentially leading to print failure or even scratching the film.

## How

Now that we understand the potential risks of overhangs and islands in SLA printing, how can we address them to avoid nightmares?

### Reorienting the Model

To decrease the number of overhangs and islands, a simple and effective method is to observe your model and adjust the orientation based on its features.

For example, the girl model in the left picture was initially oriented in a normal direction — head up and feet down — and had 68 overhangs detected. However, when the orientation was changed to head down and feet up, the number dropped to 22 as shown in the right picture.

Since the model is cured layer by layer, growing from the build plate upwards, the adjusted orientation allows her hair to be more naturally supported. Additionally, given that the girl's head and umbrella clearly make up the bulk of the model's weight, positioning these wider and heavier sections closer to the build plate significantly reduces the number of overhangs.

### Adding Support

Adding support is the most frequently used approach. Whether support is needed depends on various factors, and here we list two for your information:

    - **The angle between the overhang and the horizontal plane.** The necessity of adding support is largely influenced by this angle, but there's no fixed figure since resin performance, model structure and the printer are all part of the equation. Generally, the closer the angle is to horizontal, the more likely it is to require support. Conversely, a steeper, near-vertical angle can often be self-supporting, making additional support unnecessary.

    - **The length of the overhang.** If the overhang is too long, such as in some horizontal bridging structures, it is highly prone to bending, deformation, or fracture under the effect of the peeling force, even if the angle with the horizontal plane is 0°.

In CHTUBOX, we provide three default support settings: light, middle and heavy. Light supports are relatively thinner easy to remove. Middle supports are suitable for most islands and common overhangs. Heavy ones are set for load-bearing areas and large models, providing stronger support.

        ![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/support-light-example.png)

        ![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/support-middle-example.png)

        ![](../../../../../public/images/docs/en-US/academy/overhang-and-island-detection-in-sla-printing/support-heavy-example.png)

There are a lot more factors to be considered when adding support. If you want to learn more about this technique, just go to:

	A Complete Guide about Adding Supports in SLA/DLP/LCD 3D Printing

	Effects of Contact Shape on Model Surface Quality

### Optimizing the Model at Design Stage

If you are good at modelling, considering printability during the design stage can make your work much easier.

    - **Using a fillet or chamfer:** Designing sharp edges with a fillet or chamfer provides a larger surface area for new layers to adhere to.

    - **Dividing the model:** Splitting a complex model into smaller, detachable parts allows you to handle supports and print each part separately before assembling them later.

### Delete or Ignore Them

Unless the overhang or island is very small, and the surrounding structures can provide enough adhesion to lift it along with the build plate during the subsequent printing process, it's not recommended to delete or ignore them.
