https://math.hws.edu/graphicsbook/demos/c2/SimplePaintDemo.html

About this demo...
Drag your mouse on the canvas to draw. (Or use your finger on a touch screen.) Use the "Sketch", "Line", "Rectangle", or "Oval" tool for drawing shapes. The "Drawing Color" and "Line Width" menus control properties of the shapes. (Line width applies only to the "Sketch" and "Line" tools.)

Be sure to try the "Smudge" tool! It smudges existing colors as if they were made of wet paint. (You have to draw some shape before you can smudge it.) The implementation of this tool is an example of pixel manipulation using the getImageData() and putImageData() functions in an HTML canvas graphics context.

This demo uses an "overlay" canvas for drawing with the "Line", "Oval" and "Rectangle" tools. As you drag with one of those tools, the shape is drawn in an extra canvas that exactly covers the main canvas, so the shape can be drawn without changing the picture in the main canvas. The shape is drawn to the main canvas when you release the mouse at the end of the drag action. The overlay canvas is completely transparent, except for the shape that is drawn during dragging with the "Line", "Oval" and "Rectangle" tool. The "Smudge", "Erase", and "Sketch" tools operate directly on the main canvas.
