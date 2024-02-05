## Context

### RGB Color Mixing

To mix two or more rgb colors, one would typically take the arithmetic mean of the respective rgb values to create the new color. For example, to mix red (255, 0, 0) with blue (0, 0, 255), take the average of each component: $r=\frac{255 + 0}{2}$, $g=\frac{0+0}{2}$, $b=\frac{0+255}{2}$. This results in the color purple (128, 0, 128) which is exactly what is expected when mixing red and blue.

Sometimes, RGB color mixing is done using the root mean square (RMS) instead of the arithmetic mean. This method involves summing the square of each element, dividing by the number of elements, then finally taking the squareroot. Using the previous example with red and blue, we get: $r=\sqrt{\frac{255^2+0^2}{2}}$, $g=\sqrt{\frac{0^2+0^2}{2}}$, $b=\sqrt{\frac{0^2+255^2}{2}}$. Instead, this results in (180, 0, 180), also purple but not as dark as the previous one, highlighting this method's use: creating brighter mixed colors.

### Flicker Fusion Threshold

The flicker fusion threshold is  the limit at which humans can distinguish between a flickering light and a stable light. In other words, it describes the frequency at which a rapidly flickering light appears constant. This point is usually between 60 and 90 Hz but can vary depending on certain circumstances.

For more details: https://en.wikipedia.org/wiki/Flicker_fusion_threshold

## The Program

This program combines these concepts to simulate the mixing of colors by rapidly alternating between different colors. The current implementation allows the user to choose up to 6 colors to mix using a color wheel. Once the user clicks the "Begin" button, the next screen starts the simulation, depicting what appears to be a single new color.

Note: the colors have a transition period to avoid harsh flickering, but some combinations of colors may still be disturbing to the eyes.