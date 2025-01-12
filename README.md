
# Steganography and Encryption for Secure File Sharing

## Overview
This project showcases the integration of **encryption** and **steganography** techniques to securely share files. The process involves:  
1. Encrypting a file.  
2. Embedding the encrypted file inside a cover image (steganography).  
3. Securely extracting and decrypting the file.  

Using Python libraries, this project simplifies the process of securely hiding and sharing files.

---

## Files in This Repository

- **`Decryption.ipynb`**: A Jupyter Notebook demonstrating how to extract and decrypt a file hidden inside a cover image.  
- **`Encryption (1).ipynb`**: A Jupyter Notebook for encrypting a file and embedding it into a cover image using steganography.  
- **`carrier.png`**: A sample cover image used to hide the encrypted file.  
- **`extracted_file`**: The decrypted file after being extracted from the stego image.  
- **`key.key`**: The encryption key used for file encryption and decryption.  
- **`secret.docx`**: A sample document that is encrypted and hidden.  
- **`stego_image.png`**: The final image containing the hidden encrypted file.

---

## Technologies Used

- **Python**: Primary language for implementation.  
- **Cryptography**: For encrypting and decrypting files securely.  
- **Steganography**: For hiding encrypted files inside images.  
- **Jupyter Notebooks**: To demonstrate encryption and decryption interactively.  
- **Pillow**: Python Imaging Library (PIL) for handling images in the steganography process.

---

## Example Workflow

### **Encryption:**
1. The `secret.docx` file is encrypted using a generated encryption key (`key.key`).  
2. The encrypted file is embedded into the `carrier.png` image.  
3. The resulting `stego_image.png` contains the encrypted file hidden within it.

### **Decryption:**
1. Upload the `stego_image.png` into the decryption notebook.  
2. Use the `key.key` to extract and decrypt the original file.  
3. The original `secret.docx` file is restored as `extracted_file`.

---

## Getting Started

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/Varshitha2141/Stegnography-Based-Secure-File-Sharing.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Stegnography-Based-Secure-File-Sharing
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
