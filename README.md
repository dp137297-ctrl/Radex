# Radex Screen Data Agent

A browser-based OCR tool for screenshots and screen captures. Upload an image or capture a screen, extract text, review low-confidence words, edit the result, and export it as TXT, CSV, JSON, or Excel.

## Run locally

Open `index.html` from a local web server (for example, the VS Code Live Server extension), or deploy it to GitHub Pages. Screen capture requires a secure context such as `localhost` or HTTPS. OCR and Excel support load Tesseract.js and SheetJS from jsDelivr, so an internet connection is needed.

## Deploy on GitHub Pages

1. Create a GitHub repository and upload the contents of this folder to the repository root.
2. Push the files to the `main` branch.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **GitHub Actions**.
5. The included workflow deploys the site whenever you push to `main`. After the first run completes, open the URL shown in **Settings → Pages**.

The workflow is `.github/workflows/pages.yml`. It publishes the repository root as a static site; no build step is required.

## Privacy and OCR notes

The selected image is processed in the browser and is not uploaded by this app. The OCR engine and language data are fetched from jsDelivr on first use. OCR can misread small, blurry, or handwritten text, so verify the extracted results against the source image before using them.

##**Disclaimer:
Radex Screen Data Agent is provided as a tool to assist with screen-based text extraction. Users are responsible for ensuring they have appropriate authorization to access and process the content they submit and for complying with applicable laws and platform policies. The tool is provided subject to its actual capabilities and limitations, and reasonable efforts will be made to address security concerns and technical errors. This disclaimer does not exclude any liability that cannot legally be excluded.
