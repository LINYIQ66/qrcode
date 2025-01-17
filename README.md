QR Code Generator

This project is a simple web-based QR code generator that allows users to create QR codes from URLs. It uses the QRious library for QR code generation and provides an option to download the generated QR code.
Features

Generate QR Codes: Enter any valid URL to create a QR code.
Download QR Codes: Save the generated QR code as an image file.
Responsive Design: The application is styled for both desktop and mobile use.
Technologies Used

HTML: Structure of the application.
CSS: Styling the interface.
JavaScript: Logic for QR code generation and download.
QRious Library: For generating QR codes.
Setup and Usage

Prerequisites
A modern web browser (Chrome, Firefox, Edge, etc.)
Internet connection (to load the QRious library)
Steps to Use
Clone or download the code from this repository.
Open the index.html file in your web browser.
Enter a URL in the input box.
Click the "Generate QR Code" button.
View the generated QR code.
Click the "Download QR Code" link to save the QR code as an image.
Example
Input URL: https://www.example.com
Click Generate QR Code.
Download the image by clicking the Download QR Code link.
File Structure

project-folder/
├── index.html      # Main HTML file
├── style.css       # Embedded CSS styles (within HTML)
└── script.js       # JavaScript for QR code generation (embedded within HTML)
External Libraries

QRious: Used for QR code generation. The library is loaded via a CDN:
<script src="https://cdn.jsdelivr.net/npm/qrious/dist/qrious.min.js"></script>
Customization

QR Code Size: Change the size of the QR code by modifying the size parameter in the script:
const qr = new QRious({
    element: document.getElementById('qrCanvas'),
    value: url,
    size: 250 // Adjust size here
});
Styling: Modify the styles in the <style> section of the HTML file to suit your design preferences.
Screenshots

Input URL:
Users can input a URL and click Generate QR Code.
Generated QR Code:
The QR code is displayed on a canvas element.
Download Link:
The "Download QR Code" link appears after generating a QR code.
License

This project is open-source and available under the MIT License.
