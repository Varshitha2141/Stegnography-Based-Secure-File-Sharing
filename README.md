#Steganography and Encryption for Secure File Sharing

Overview
This project demonstrates the use of encryption and steganography to securely share files. The process involves encrypting a file, embedding it inside a cover image (steganography), and then securely extracting and decrypting it. The project uses Python libraries to handle both encryption and steganography, allowing users to send and receive encrypted files hidden inside an image.

Files in this Repository:
Decryption.ipynb: Jupyter Notebook that demonstrates how to extract and decrypt a file hidden inside a cover image.
Encryption (1).ipynb: Jupyter Notebook to encrypt a file and embed it into a cover image using steganography.
carrier.png: A sample cover image used to hide the encrypted file.
extracted_file: The decrypted file after extraction from the stego image.
key.key: The encryption key used for file encryption and decryption.
secret.docx: A sample document file that is encrypted and hidden.
stego_image.png: The final image with the hidden encrypted file embedded in it.

Technologies Used
Python: The primary language used for the implementation.
Cryptography: For encrypting and decrypting files.
Steganography: For hiding encrypted files inside images.
Jupyter Notebooks: For demonstrating the encryption and decryption process interactively.
Pillow: Python Imaging Library (PIL) for working with images in the steganography process.

Example Workflow:
Encrypt the file:
The secret.docx file is encrypted using the provided key and embedded into the carrier.png image.
The resulting stego_image.png contains the encrypted file, hidden in plain sight.
Decrypt the file:
The stego_image.png is uploaded into the decryption notebook, and the key.key is used to decrypt and extract the original file.
The original secret.docx file is restored.

File Structure:
steganography-secure-file-sharing/
│
├── Decryption.ipynb         # Jupyter notebook for extracting and decrypting files
├── Encryption (1).ipynb     # Jupyter notebook for encrypting and hiding files
├── carrier.png              # Cover image used to hide the encrypted file
├── extracted_file           # The decrypted file after extraction
├── key.key                  # Encryption key used for file encryption and decryption
├── secret.docx              # Sample document file to be encrypted and hidden
├── stego_image.png          # Image with the hidden encrypted file
├── requirements.txt         # Python dependencies
├── README.md                # Documentation
└── LICENSE                  # License information

Contributing:
Feel free to fork the repository and submit issues or pull requests for improvements.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

