# Advanced Encryption Standard (AES) Implementation

A robust, pure-Python implementation of the **Advanced Encryption Standard (AES)**. This project provides a transparent look into the inner workings of symmetric-key cryptography, supporting multiple key lengths and operating modes.



## 🚀 Features

* **Variable Key Lengths:** Full support for **AES-128, AES-192, and AES-256**.
* **Operating Modes:**
    * **ECB (Electronic Codebook):** Standard block-by-block encryption.
    * **CBC (Cipher Block Chaining):** Enhanced security using an Initialization Vector (IV) to prevent pattern recognition.
* **Zero Dependencies:** Built using standard Python libraries—no external installations required.
* **Educational Design:** Clean code structure following the official FIPS 197 specification.

---

## 🛠 How It Works

The implementation handles the four main stages of the AES round transformation:

1.  **SubBytes:** A non-linear substitution step using a lookup table (S-box).
2.  **ShiftRows:** A transposition step where rows of the state are shifted cyclically.
3.  **MixColumns:** A mixing operation that operates on the columns of the state.
4.  **AddRoundKey:** The state is combined with a round key using bitwise XOR.



---

## 💻 Getting Started

### Prerequisites
* Python 3.6 or higher.

### Installation
Clone the repository to your local machine:
```bash
git clone [https://github.com/4rn4vk/Advanced-Encryption-Standard-AES-.git](https://github.com/4rn4vk/Advanced-Encryption-Standard-AES-.git)

cd Advanced-Encryption-Standard-AES-
```

## 🚀 How to Use

Follow these steps to encrypt or decrypt your data using the script:

1.  **Locate the "Code Compiler" Section:** Open `AES_Final.py` and scroll to the bottom of the file.
2.  **Configure Your Inputs:**
    * Find the **Encryption** or **Decryption** print statements.
    * Input your **Plain text** (for encryption) or **Cipher text** (for decryption) as a string.
    * Input your **Key** as a string (ensure it is 16, 24, or 32 bytes long).
3.  **Toggle CBC Mode:** * Do **not** modify the arguments inside the print statements.
    * Instead, change the boolean flags directly under the `Code Compiler` heading:
      
    ```python
    # Set to True for CBC mode, False for ECB mode
    CBC_encryption = True
    CBC_decryption = True
    ```
4.  **Run the Script:** Execute the file in your terminal:
    ```bash
    python AES_Final.py
    ```
5.  **View Results:** The encrypted or decrypted value will be printed directly to your console.

> **Note:** The script automatically handles the key expansion and round calculations based on the key string length you provide.
