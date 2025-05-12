# Number-Plate-Detection
NumberPlate_detectionOf_Vehicles
🚗 Number Plate Detection using OpenCV and EasyOCR
This project demonstrates a simple approach to detect vehicle number plates using OpenCV and read the text on the plates using EasyOCR.

📌 Features
Detects vehicle number plates using OpenCV Haar Cascades.
Extracts and reads the number plate text with EasyOCR.
Displays the image with bounding boxes around the detected plates and the extracted text.
🖼️ Example Output
Below is an example of how the detected number plate appears after running the script:

Example Output

🛠️ Requirements
To install the required Python libraries, use the following command:

pip install opencv-python easyocr
If you're using Google Colab, the cv2_imshow function will automatically work for image display.

🧠 How It Works
The image is loaded and converted to grayscale.

A Haar Cascade classifier (haarcascade_russian_plate_number.xml) detects the vehicle number plates in the image.

Detected plates are cropped and passed to EasyOCR for text extraction.

The detected text is drawn on the original image, and the image is displayed with the bounding box around the plate.

🚀 How to Use
Clone the repository or download the code to your local machine.

Make sure the image file (e.g., NUMPLATE.jpeg) is in the same directory as the script, or update the path in the code.

Run the script:


image_path = 'NUMPLATE.jpeg'  # Path to your image file
detect_number_plate(image_path)
Local Use (Optional): If you're running this locally, replace cv2_imshow with cv2.imshow and ensure you have GUI support enabled for OpenCV to display the images.

📂 File Structure

├── detect_number_plate.py   # Python script for number plate detection
├── NUMPLATE.jpeg            # Sample image (replace with your own)
└── README.md                # Project documentation
🔍 Dependencies
OpenCV: For image processing and Haar cascade-based object detection.

EasyOCR: For text extraction from the detected number plate.

NumPy: For array manipulation.

For Google Colab users, cv2_imshow will be used automatically for image display. For local use, replace cv2_imshow with cv2.imshow.

⚠️ Notes
Detection accuracy may vary based on factors like lighting, plate angle, and image clarity.

The default Haar Cascade used is designed for Russian-style number plates. For better detection of plates from other regions, you may need to fine-tune or use a different cascade classifier.

📄 License
This project is open-source and available under the MIT License.
Feel free to use, modify, and distribute it!

🙌 Acknowledgments
OpenCV: OpenCV for computer vision tasks.

EasyOCR: EasyOCR for optical character recognition.

Haar Cascade Classifier: Pre-trained classifier for number plate detection.
