# Quick Start

This section will guide you through the basic usage of CHITUBOX, helping you to get started quickly. We will start by loading a model, and then add supports, slice the model, and finally export the printable file to your printer.

## Create Project

When you first launch CHITUBOX, you should see the **New Project** Button at the top of the main window. Click it to create a new project.

## Add a printer

In the **Print Information Panel**, add a printer. Here we use ELEGOO Jupiter as an example.

![Add Printer](../../../../../public/images/docs/en-US/chitubox/1.x.x/quick-start-000.png)

Click "Next". Here you can change the configurations of the printer. We will use the default settings for convenience. Click "Apply".

	Never change the **Resolution** and **Size** of a preset printer
	configuration as it may cause the printer to report an error when reading
	the file.

## Load Files

To load a 3D mesh file (stl, obj, 3mf, etc.):

If you wanna load a CHITUBOX Project file:

Alternatively, you can use drag and drop to load your files, both 3D mesh files and CHITUBOX project files.

Here we import _Grozhul, Warchief of the Iron Maw_, crafted by [Mojibake Collectibles](https://www.instagram.com/mojibake_collectibles).

![Grozhul, Warchief of the Iron Maw](../../../../../public/images/docs/en-US/chitubox/1.x.x/quick-start-001.png)

## Add Supports

Without supports, all overhangs will have nothing to pull them up during printing, causing the model to fail.

Typically, auto-support is our first choice for model support generation, but before applying auto-support, there are some parameters we need to tweak.

The model we used for demonstration has a large flat base, which is not recommended to be supported parallel to the build plate. We recommended either tilting the model or attaching the base flat on the build plate.

Prevent the support base from merging with the model's base, set **Platform Contact Shape** to `None`,

Then we modify **Model Lift Height** to `0` to ensure the model is attached flat on the build plate, and turn off **Automatically Add Raft** so raft doesn't merge with the model's base as well.

Change **Mode** to `+Platform` so the bottoms of supports will be generated on the platform only, not on the model.

We're all set now, click **Apply**. It may takes a few minutes to generate the supports, depending on the size and the complexity of the model.

![Grozhul, Warchief of the Iron Maw, supported](../../../../../public/images/docs/en-US/chitubox/1.x.x/quick-start-002.png)

You can also add manual supports if you want to have more control over the support placement.

Great! Now we can go ahead to slice the file.

## Slice and Save

Click the **Slice and Save** button, save the file to your USB drive.

Congratulations, you have completed the CHITUBOX basic tutorial. Have fun printing! 🎉🎉🎉
