# Printing Preparation Conditions

## Printing Environment

1. The indoor temperature of the printing validation room should be consistently maintained between 18~28°C.
1. The indoor ambient humidity should be controlled below 60%.
1. The printer needs to be kept away from heat sources, water sources and vibration sources.
1. Ensure regular air circulation in the room to minimize and avoid inhalation of resin fumes by personnel.
1. The room should be kept in darkness or low blue light conditions. It is recommended to use a low yellow light. During the entire printing process, ensure that the printer's light-shielding cover is fully closed.
1. The power supply should meet grounding requirements and should not share a circuit with high-current devices. Ensure the stability of the power supply voltage during the printing process.
1. Do not place water, alcohol, or other volatile solvents in the printing room to avoid interference with the print quality.
1. The supply voltage and current should strictly follow the printer's power requirements.

## Printer Setup

1. Install the printer on a hard, level surface.
1. Check and confirm that the FEP film is intact, clean, and properly tensioned.
1. Ensure the light source and display device are functioning correctly.
1. Verify that the light intensity values are appropriate when the light source and imaging area are fully illuminated during normal use.
1. Ensure the imaging work area and the FEP film are clean and free of impurities.
1. Verify that the printer platform is securely locked.
1. Ensure there are no residual objects on the printing platform.
1. Confirm that the printing platform is level.
1. Ensure the resin vat is correctly installed and locked.

It is necessary to conduct light intensity sampling test following item 4 above as part of the printer verification process.

The light intensity measurement device selected for the light intensity sampling test needs to strictly follow the devices' corresponding instructions in order to acquire accurate light intensity value.

	The light intensity measuring device should be calibrated according to the specific wavelength used by the printer.

For selected printer products, measure and record light intensity values at fixed intervals as illustrated. Ensure the light intensity measuring device is fully adhered to the imaging surface. Measure and record the light intensity values five times at each specified point and calculate the average value.

![](../../../../../../../public/images/docs/en-US/chitubox-printing-test/1.x.x/test-preparation/front-of-printer.svg)

	The above content is mainly for the preparation process of pull-up photocurable 3D printing, and does not include the preparation instructions of bottom-up printers.

## Printing Materials

1. Check and confirm that the printing material is normal and not expired.
1. Ensure the resin in the vat is well-mixed and free of impurities.
1. Verify that there is enough resin in the vat to avoid overflow during printing.Preparation of Printing Documents

## Preparation of Printing Documents

### Model Layout Preparation

#### Single Model Layout

	For repeated parameter adjustments and layout tests of a single model, ensure the model is positioned consistently relative to the same printer. Refer to the example position below.

![](../../../../../../../public/images/docs/en-US/chitubox-printing-test/1.x.x/test-preparation/single-model_001.png)

	You can select the model to trigger the move button and click on the model to view and confirm its position relative to the platform.

#### Multi-Model Layout

	For repeated printing tests of multiple models, ensure the models are consistently positioned relative to the same printer.

#### Adjustment Of Support Parameters

Some test models include CHITUBOX's coarse, medium, and fine support models. These effectively test the validity of support contact point spacing parameters. Other support structure parameters can be tested through secondary editing and setting of the model support structure.

### Printing Parameter Settings And Preparation

Detailed printing parameter setting instructions can be seen on 📖user manual.

The table below outlines how different printing parameter settings in CHITUBOX Pro software affect print files and outcomes. Use this as a guide to optimize printing parameters.

			Settings
			Parameters
			Print Effect Description

				Printer

			Mirror

				Mirror settings affect the symmetry of the print file. Click  📖 here  to learn more.

			Resolution

				The resolution must match the printer's hardware specifications to ensure proper file interpretation and identification. Resolution is the key parameter for achieving extreme precision. Higher resolution can significantly improve print precision.

			Size

				X/Y print size must match the printer's hardware specifications to avoid size errors and deformation. The Z size setting needs to be set according to the actual hardware of the printer.The Z size setting affects print height but not precision.

				Under the same resolution, a smaller print size will improve the limit of printing accuracy.

			Build Area Offset

				X/Y effective print boundary settings, based on X/Y print size values.

			Display Correction

				Applicable to some DLP printers for correcting optical installation deviations. Improper settings can cause size errors and deformation.

			Print
			Layer Height (mm)

				Thinner layers result in more detailed slices (X/Y/Z) but longer print times. Too thin layers may affect print quality due to material sensitivity to light.

				Slice files with layers that are too thick will not only reduce the quality of the printed surface, but also further increase the risk of printing errors and failures.

			Bottom Layer Count

				The combination of base layers and base exposure time affects model adhesion to the platform. Excessive base layers can lead to over-curing at the model's base, which will lead larger size at the bottom and increase in print time.

				The tolerance compensation setting can be used to mitigate the overcuring effect.

			Exposure Time (s)

				Adequate exposure time ensures complete resin curing and precise print dimensions. Short exposure increases the risk of print failure, while long exposure reduces detail. 

			Bottom Exposure Time (s)

				Combined with base layers, this affects adhesion. Excessive base exposure time leads to over-curing. Mitigate this with bottom tolerance compensation settings.

			Transition Layer Count

				Proper transition layers help manage sudden changes in exposure time, reducing print failure risks.

			Transition Type

			Transition Layer Interval Time Difference

			Wait Mode During Printing

				It is recommended to set the Wait Mode to Resting Time

				Excessive wait time increases print defects and failure risks. Proper delay increases print surface quality by improving resin flow and reducesurface rippling during print.

			Bottom Lift Distance (mm)

				Appropriate lift distances aid in layer separation, preventing print failures and optimizing print time.

			Lifting Distance (mm)

			Bottom Lift Speed (mm/min)

				Appropriate speeds ensure successful layer separation, preventing failures and optimizing print time.

			Lifting Speed (mm/min)

			Bottom Retract Speed (mm/min)

				Appropriate retract speeds ensure accurate repositioning of the platform and optimize print time. Slow retract speeds help to avoid resin overflow.

			Retract Speed (mm/min)

			Advanced
			Bottom Light PWM

				Appropriate light intensity ensures model precision and performance, while controlling print time. 

				Note: Light PWM adjustments may not apply to certain machines.

			Light PWM

			Image Grey

				Appropriate grayscale ensures model precision and performance and differentiates from support structures, enhancing support strength.

			Anti-aliasing

				Appropriate edge smoothing and pixel blurring reduce layer lines and jagged edges.

				Note: Anti-aliasing is compatible with *.cbddlp, not with *.ctb.

			Tolerance Compensation

				Proper compensation adjusts model boundary dimensions accurately.

			Odd-Even Layer Difference

				A suitable setting for the odd-even layer parameter can enhance the differentiation between odd and even layers. This helps achieve a layered structure printing effect, which can be widely applied in fields such as invisible orthodontics.

			Bottom Tolerance Compensation

				Proper compensation reduces over-curing of base layers.

			Print Time Compensation

				Suitable compensation aligns estimated and actual print times more accurately.

			Mask

				Using the correct mask file improves consistency in model dimensions and fine details across the entire print area.
