Secure-Data-Hiding-in-Images-Using-Steganography-


Overview
This project implements an image-based steganography tool that allows users to securely hide and retrieve messages within images. The encryption mechanism ensures data confidentiality by using AES encryption, making it a robust solution for secure communication.



Features
🔐 AES Encryption: Messages are encrypted using AES-256 encryption before being hidden in an image.
📷 LSB Steganography: Uses Least Significant Bit (LSB) technique to embed encrypted messages within images.
📂 User-Friendly Interface: Built with Streamlit for an interactive and intuitive UI.
🖼️ Image Support: Supports PNG images for encoding and decoding messages.
🔑 Password Protection: Requires a password for both encryption and decryption, ensuring security.


Technologies Used


Python: Core programming language.
Streamlit: Web-based UI for seamless interaction.
OpenCV: Image processing library for reading and modifying images.
NumPy: Used for efficient array manipulations.
PyCryptodome: AES encryption library for securing messages.
Installation
Ensure you have Python installed, then install the required dependencies:

pip install streamlit opencv-python numpy pycryptodome
Usage
Run the Streamlit application with the following command:

streamlit run app.py
Encoding a Message
Upload a PNG image.
Enter the secret message.
Provide a passcode for encryption.
Click "Encode & Save Image" to generate an encrypted image.
Download the encrypted image for later use.
Decoding a Message
Upload the previously encoded image.
Enter the correct passcode.
Click "Decode Message" to reveal the hidden message.
Security Considerations
The encryption key is derived from the user's password using SHA-256 hashing.
Messages are padded and encrypted using AES in CBC mode.
A delimiter (%%) is used to mark the end of the message in LSB encoding.
Limitations
The size of the message is constrained by the image's pixel capacity.
Only PNG images are supported to maintain lossless encoding.
Future Enhancements
🔄 Support for additional image formats (JPEG, BMP, etc.).
📊 Improve encoding efficiency for larger messages.
🌐 Deploy as a web-based service for broader accessibility.
License
This project is open-source and licensed under the MIT License.

Acknowledgments
Special thanks to all open-source contributors and libraries that made this project possible.
