# Shape Generator and Combiner for Exam Proctoring

An open-source, client-side web application designed for instructors and computer science professors to generate randomized page-margin watermarks. These unique geometric combinations and alphanumeric codes help maintain control, track variations, and prevent cheating during paper-based exams.

## Project Purpose

When managing multiple examination groups or shuffling test variations, keeping track of papers can become difficult. This tool automates the creation of distinct visual watermarks that fit into standard A4 page margins (top, middle, and bottom positions). 

By using randomized geometric shapes, background colors, and dynamic numbers, each exam variation gets a highly identifiable visual signature that can be recognized at a glance during proctoring.

## How to Apply the Margin Watermark in Word Processing Software

The generated composition is an elongated vertical PNG layout with a transparent background. It is tailored to align perfectly along the page margins. Here is how to insert it as a background watermark:

### Microsoft Word
1. **Open the Header:** Double-click the very top area of your page to edit the **Header**.
2. **Insert the Image:** Go to `Insert > Pictures > Picture from File` and select your downloaded `composition.png`.
3. **Change Text Wrapping:** Right-click the inserted image, choose `Wrap Text`, and select **Behind Text**. This ensures it acts as an unselectable background layer that won't disrupt your exam text alignment.
4. **Positioning:** Drag the image file over to either the left or right margin. Scale it vertically if needed to span across the page safely.
5. **Close Header:** Double-click the main document area to finish. The margin watermark will now automatically replicate on every page.

### Google Docs
1. **Open the Watermark Tool:** Go to `Insert > Watermark` from the top menu bar.
2. **Upload Image:** In the sidebar that appears on the right, ensure the **Image** tab is selected, then click **Select Image** to upload your `composition.png`.
3. **Adjust Formatting Options:** - Uncheck **Faded** if you want the full vibrant color of the shapes to remain visible.
   - Click on **More Image Options** (or right-click the image) to open sizing and position parameters. 
4. **Positioning:** Set text wrapping to **Behind Text**. Drag and place the watermark structure perfectly inside the page margins.
5. **Apply:** Click **Done**. The margin indicator is locked safely in the background across all document pages.

## Features

- **100% Client-Side:** No server, database, or backend installation required. Powered entirely by HTML5 Canvas and JavaScript.
- **Randomized Asset Generation:** Generates a custom amount of shapes (circles, triangles, pentagons, stars, etc.) with random backgrounds and high-contrast labels.
- **Dynamic Proportions:** Adapts calculations dynamically to match your required pixel sizing while keeping original canvas geometry.
- **Interactive Multi-Selection:** Select up to 3 generated assets to build a continuous vertical margin layout.
- **Instant Download:** Merges selections instantly onto a high-resolution transparent PNG layout ready to be imported into your LaTeX, Typst, MS Word, or Google Docs templates.

## Usage Instructions

1. **Generate Shapes:** Enter your desired batch amount and pixel size constraint, then click **1. Generate Shapes**.
2. **Select Margins:** Click on the generated boxes within the gallery layout (up to 3 items). Your selections will be highlighted.
3. **Render Composition:** Click **2. Combine Selected**. Your vertical sheet margin will immediately render in the right-side preview column.
4. **Export:** Click the green **3. Download Composition** button to export your final watermark sequence as a transparent `.png` file.
