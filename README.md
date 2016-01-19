# mplewis' KiCad Libraries

I use these libraries in my personal projects. Use at your own risk.

# Design Guidelines

*Reminders to myself when designing PCBs with KiCad*

Vias should be at least 0.9 mm in diameter if you expect to fit a header pin into them. Vias with diameter 0.762 mm printed at Dirty PCBs could take a header if you really forced it—make them bigger.

KiCad projects default to adding clearance to the solder mask. This makes your pads look shitty. Change this inside pcbnew: **Dimensions** –> **Pads Mask Clearance** –> **Solder Paste Clearance:** change from -0.003 to 0.

Don't squish fonts. Set the width and height equal to each other.

Font thicknesses are based on the font size. If your height/width are 0.04", the thickest KiCad will allow is 0.01" (25%). Here are some guidelines for font thickness:

* 10%: Thin
* 15%: Normal
* 20%: Bold
* 25%: Black

Extend the sides of your fill polygons a few clicks past the edge cuts. Otherwise your fill stops early at the sides and leaves pointy fill corners in your rounded corners. It looks weird.

On rounded corners:

* 0.05" radius still feels pretty pointy.
* Bean+ uses a corner radius of 10mm.

Routing works differently in OpenGL canvas mode than Default. I think?

Dirty PCBs is pretty dirty. Their silk aligning is all over the place. Don't use them for awesome custom art.

Pad size: 0.0125" annular ring pads are fine (0.025" difference between inner and outer diameter). 0.0155" pads are nice and fat and friendly.
