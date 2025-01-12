# Stegnography-Based-Secure-File-Sharing

This project demonstrates the process of embedding a file securely within an image using steganography techniques, along with encryption and decryption. The process involves:
1)Encrypting a file.
2)Embedding the encrypted file into a cover image (steganography).
3)Decrypting the file after extraction from the image.

Files in the Repository:
1)Decryption.ipynb: Jupyter notebook that demonstrates how to decrypt the hidden file.
2)Encryption.ipynb: Jupyter notebook for encrypting a file and embedding it within an image.
3)carrier.png: A sample image that serves as the cover image for hiding the encrypted file.
4)extracted_file: The file that will be extracted after decryption from the stego image.
5)key.key: The encryption key file used for file encryption and decryption.
6)secret.docx: A sample document file that is being encrypted and embedded.
7)stego_image.png: The final image with the encrypted file hidden within it.

Requirements:
To run the notebooks and the script, you will need the following Python libraries:
1)cryptography
2)Pillow (for image manipulation)
3)numpy
4)matplotlib
5)steghide or custom steganography tools
You can install them using pip:
pip install cryptography pillow numpy matplotlib

How It Works:
Step 1: Encrypt the File
Use Encryption.ipynb to select the file (e.g., secret.docx) and encrypt it using a symmetric encryption algorithm.
The key is saved as key.key to be used for decryption.
Step 2: Embed the Encrypted File
The encrypted file is then embedded into the image carrier.png using a steganographic algorithm.
The result is a stego_image.png, which appears to be a regular image but contains hidden encrypted data.
Step 3: Extract and Decrypt the File
Use Decryption.ipynb to extract the hidden encrypted file from stego_image.png.
After extraction, the file is decrypted using the key stored in key.key.

Example Workflow:
Encrypt the file using Encryption.ipynb.
Embed the encrypted file into carrier.png to create stego_image.png.
Extract the encrypted file from stego_image.png using Decryption.ipynb.
Decrypt the file using the key key.key.

Notes:
The project demonstrates the combination of encryption and steganography for secure file sharing.
The file size of the embedded data should be smaller than the capacity of the image used for steganography. Larger files may result in perceptible changes to the cover image.
This project does not perform any advanced error handling or validation, so ensure that the image and file sizes are compatible.

Contributing:
Feel free to fork the repository and submit issues or pull requests for improvements.

License:
This project is licensed under the MIT License - see the LICENSE file for details.

