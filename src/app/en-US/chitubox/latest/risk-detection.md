# Risk Detection

CHITUBOX offers various risk detection features to help you identify potential issues with your 3D models before printing. These features include:

## Overhang Detection

Overhang Detection is a feature that identifies areas of the model that may require support structures due to overhangs. It helps you to visualize where supports are needed in case auto support generation is not sufficient. Detected Overhangs are listed in the Parameters Panel and allow you to navigate camera through them automatically.  

Overhang detection offers three levels of accuracy: low, medium, and high. The higher the accuracy level, the more precise the detection results, but the longer the detection time.

## Island Detection

Islands detection is similar to overhang detection, but it can only be applied after slicing the models. It identifies overhangs
by detecting if there is a attachable point at the previous layer, islands are listed in the Parameters Panel grouped by layer number, and highlighted in red at pixel level in the layer preview area.

If islands are considered ignorable, you can simply delete them, corresponding areas in the layer will not be exposed during printing. Alternatively, you can go back and add supports to these islands.

For most scenarios we recommend using Overhang Detection, which happens before slicing and allows camera auto-navigation at the overhang areas, also avoids the back-and-forth workflow that you have to deal with when using Island Detection.

## Cavity Detection

Cavity Detection can help users identify any enclosed cavities within 3D models, such as closed pockets or holes. Users can add holes to models to avoid vacuum effects during printing.

## Collision Detection

Collision detection can help users highlight collisions among 3D models. Users can adjust models to avoid such collisions.
