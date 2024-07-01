This isn't yet finished, but it is a decent work in progress.



Basic physical properties:

The rail itself is a `16mm` by `20mm` by `5mm` + the connecting slant (approx. `23mm`). The light channel is `13mm` wide (`23mm - 2 * 5mm`) and has a groove that is `15mm` wide `~0.8mm` below the surface.

So far, what has worked for locking into the rail are these small two-layer locking pins. It's fine to print them very tight as long as they are PETG, so a little flexible. You can also print them without supports if you let the gradually emerge from the model (see the `-b` version).

### Printing notes

I've tried this in clear PETG. On a textured print surface, the adhesion is quite bad. For all the delicate parts, brim is essentially mandatory. For the corner piece, you might be able to print it without a brim, but it is probably going to at least lift off at the edges. So for the best possible fit, I would recommend just doing a brim everywhere.

Supports should not be needed with version B, but version A requires them and they do tend to either fail or be very hard to remove. That is why version A was ultimately scrapped.

##### A version

This is the initial version that basically does not work in any way, shape or form. The basic clips (just for testing) are not tight enough (they are `5.5mm` instead of exactly `5mm` from the edges, so they don't actually lock into the channels). The corner piece might work, but it is basically unprintable.

##### B version

This one seems to be actually working. The corner joint consists of three interlocking pieces. The two "side" pieces (L and R) lock into the rail, while the corner piece just sits there and is connected to the side pieces by a square peg. You can slide the side pieces inside the rail, so you don't have to lock everything into place at once. Note that the side pieces have a region where there are no clips. This is for hiding the seam with the original diffusion strip.

Here, the corner piece is intended to be printed on the obvious, most "flat" side, such that supports are not necessary. The side pieces should be printed in a way that layer lines run perpendicular to the clips (so they won't snap off and don't need supports). That is, the part is placed on the edge where it will meet/overlay with the original diffusion strip. The shape should be printable without supports as well.

#### Current issues

- The whole thing is slightly more "bulky" than what is actually necessary. Both the corner piece and the side pieces could be shorter. Just trim all the areas a bit. 
  - The interlocking peg could be shorter on both sides and can be moved closed to the actual corner. 
  - The clip area for latching on to the rail could be shorter (they are quite strong i the current design). 
  - The overlap area for the existing diffuser is also probably unnecessarily long.
- Currently, the parts have a very different texture because they are printed in different orientations. Furthermore, they are quite thin (often just two layers).
  - Make the "bulk" of the part thicker. Currently it is `1.2mm`, which means we can actually see through it and observe all the imperfections of the corner joint. We can probably double the thickness to make it less transparent. I would probably just use 100% infill here.
  - We can add fuzzy skin to the slant portion of the rail cover. We can't add it to the straight edge, because that one is sitting on the build plate when printing the corner piece. But this could be enough to make the texture of the part sufficiently random in order to make it less noticeable that there are printed with different settings.
  - Alternatively, we could try to create our own pattern instead of using fuzzy skin, but that seems to be a bit overcomplicated for now.

### Other tasks

* We eventually want some "stoppers" for the bottom of the rail so that the diffuser fits tightly and there is no gap between the rail and the table top. These can just be clips, because the cable will have to go down from the rail behind the cabinet.
* We also need a connecting center piece. This also needs to be clip on because we need a place in the middle from where we can load the diffuser. For that, we will probably need to align the two rails in the center better, but that's just the general issue of the middle cabinets not being very well aligned.

### Lessons learned

* We probably should have just cut the LED rails at 90 degrees and use only the plastic to join them. Would be easier to cut/measure and we would have less of a need to cover the joint in a nice way.
* Small clips do work, but they really need to be printed in the correct orientation.
* Bed adhesion with small PETG parts is rather poor, even with a brim. I would like to consider a smooth bed without interface material for this. 
* The transparent PETG is really easy to see through, but has imperfections due to layer lines. We'll see how the fuzzy skin helps to smooth out those imperfections.

