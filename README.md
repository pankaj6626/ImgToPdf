# imgToPdf

Here are some screenshots from the project

![Screenshot (151)](https://user-images.githubusercontent.com/68517660/138468465-34a300cb-b882-45a3-8aea-e578a5f04888.png)



![Screenshot (152)](https://user-images.githubusercontent.com/68517660/138468550-67f642cd-48f2-47e8-b61e-f6f892b5f688.png)


# Image to PDF Converter

## Project Description
This project allows users to upload multiple images (JPG/PNG) and convert them into a single PDF file. Users can adjust the order of images, preview the final PDF, and download it.

## Features
- Upload multiple images (JPG/PNG).
- Adjust image order before conversion.
- Preview the PDF before downloading.
- Convert images into a single PDF.
- User-friendly interface.

## Technologies Used
- HTML
- CSS
- JavaScript
- PDF-Lib (for PDF generation)
- jsPDF (for PDF manipulation)
- Download.js (for downloading files)
- Font Awesome (for icons)

## Project Structure
```
image-to-pdf-converter/
│── index.html    # Main HTML file
│── index.css     # Styling file
│── index.js      # JavaScript logic for handling images and PDF conversion
```

## Installation & Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/image-to-pdf-converter.git
   ```
2. Navigate to the project directory:
   ```sh
   cd image-to-pdf-converter
   ```
3. Open `index.html` in a browser.
4. Click on "CHOOSE FILES" to upload images.
5. Preview uploaded images and arrange them as needed.
6. Click on "DOWNLOAD" to generate and download the PDF.

## JavaScript Functions
### `encodeImageFileAsURL(element)`
- Reads the selected image files and stores them in an array.
- Updates the UI to show uploaded images.
- Triggers PDF generation after a short delay.

### `saveAsPDF()`
- Displays the "SAVE AS PDF" button after images are uploaded.

### `handleDelete(e)`
- Removes an image from the list before conversion.
- If no images remain, reloads the page.

### `embedImages()`
- Converts images into a PDF using PDF-Lib.
- Embeds each image onto a new PDF page.
- Downloads the final PDF file.

### `convertToPDF()`
- Displays uploaded images in the UI.
- Allows users to delete images before conversion.

### `calcPdfSize()`
- Uses jsPDF to create a PDF document.
- Iterates through uploaded images and scales them to fit the PDF.
- Saves the final PDF as `combined_images.pdf`.

### `backToHomepage()`
- Reloads the page to reset the application.

## Deployment
- The project can be hosted on GitHub Pages or any static hosting provider.
- No backend is required; it runs entirely on the client-side.

## Future Enhancements
- Drag-and-drop functionality for reordering images.
- Add support for more image formats.
- Improve UI with better styling and animations.

## License
This project is open-source and available under the [MIT License](LICENSE).


