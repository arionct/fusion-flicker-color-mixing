**Context**

To mix two or more rgb colors, one would typically take the arithmetic mean of the respective rgb values to create the new color. For example, to mix red (255, 0, 0) with blue (0, 0, 255), take the average of each component: $r=\frac{255 + 0}{2}$, $g=\frac{0+0}{2}$, and $b=\frac{0+255}{2}$. This results in the color purple (128, 0, 128) which is exactly what is expected when mixing red and blue.

The flicker fusion threshold is a term to describe the limit at which humans can distinguish between a flickering light and a stable light. In other words, it describes the point at which a rapidly flickering light appears constant. This point is usually between 60 and 90 Hz but can vary depending on certain circumstances.
For more details: https://en.wikipedia.org/wiki/Flicker_fusion_threshold#:~:text=For%20the%20purposes%20of%20presenting,by%20an%20order%20of%20magnitude.

**The Program**

This program combines these concepts to simulate the mixing of colors by rapidly alternating between different colors. The current implementation allows the user to choose up to 6 colors to mix using a color wheel. Once the user submits the order, the next screen iterates through each color, depicting what appears to be a new color. Note: the colors have a transition period to avoid harsh flickering, but some combinations of colors may still be disturbing to the eyes.