# Effects of Contact Shape on Model Surface Quality

> GS-B11 Rigid Resin is used in this case.

In CHITUBOX, there is a related parameter about support tips called "contact shape". You can choose "none" shape or "sphere" shape as shown below. Now let's test the effect of these two shapes on the support removal and the surface quality of the object.

Close up of sphere contact shape vs. no contact shape:

## Effect of Contact Shape on Model Surface

By changing the contact shape between the support and the model surface, we can see that there is a certain difference between the spherical contact shape and the contactless shape support. Because the top of the contactless shape support will be exposed and strengthened on the contact surface during the printing process, and gradually thicken and expand from the connection, the support is well connected with the model, ensuring the stability of the connection, but also making it difficult to remove the support.

## Effect of Contact Shape on Support Strength

![](../../../../public/images/docs/en-US/academy/effects-of-contact-shape-on-model-surface-quality/support-params.png)

				Support Parameters

![](../../../../public/images/docs/en-US/academy/effects-of-contact-shape-on-model-surface-quality/with-contact-shape.png)

				With Contact Shape

![](../../../../public/images/docs/en-US/academy/effects-of-contact-shape-on-model-surface-quality/without-contact-shape.png)

				Without Contact Shape

## Effect of Contact Shape on Support Removal

When removing the supports, it becomes apparent that "Sphere" contact shape supports are easier to remove than "None" contact shape supports, but in other words, "None" contact shape supports are more stable than "Sphere" contact shape supports in terms of the strength of support structures. After the removal of the supports, the residues of the supports left on the surface of the model are more pronounced with "Sphere" contact shape than with "None" contact shape.

If the model is delicate, the contactless shape support is more likely to accidentally damage the model when it is removed than the spherical support.

The sanding was done with an electric sanding pen with switchable sanding heads, and here sanding with a wheel and polishing with a fine sandpaper roll were used.

![](../../../../public/images/docs/en-US/academy/effects-of-contact-shape-on-model-surface-quality/electric-sanding-pen.png)

Although the "Sphere" contact shape supports leave more residues, it is relatively better sanded because the residues are mostly bumps. After sanding, the surface quality of the "Sphere" contact will be better compared to "None" contact shape.

Besides, there are remarkable pot holes on the surface of "None" contact shape. Because the rigid resin is relatively brittle and cutting will easily leave pot holes. But with shperes on the surface, it's much easier to protect the surface when removing the supports.

## Conclusion

1. The support structures of “sphere" shape is easier to remove than that of "none" shape.
1. The support structures of “none " shape is stronger than that of "sphere" shape.
1. After removing the supports, the support residues left on “sphere" shape surface are more obvious than that of "none" shape. But as they are all raised residue,1. there are fewer pits and the surface quality is smoother after treatment than "none" shapes.
1. The surface quality of “sphere" shape is better than that of "none" shape.
