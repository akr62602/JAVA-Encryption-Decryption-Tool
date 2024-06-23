# Encryption/Decryption Application

This Java project provides a user-friendly graphical interface to encrypt and decrypt text using the Caesar Cipher algorithm. The application allows users to input text, specify a key, and choose between encryption and decryption operations.

## Features

- **User-Friendly Interface**: The application uses Java Swing to provide an intuitive GUI, making it easy for users to input text and select operations.
- **Caesar Cipher Algorithm**: Implements the Caesar Cipher technique for secure encryption and decryption of text based on a user-defined key.
- **Input Validation**: Ensures the key is within an acceptable range (1-25) and provides error handling to guide users through successful operations.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) 8 or higher
- Integrated Development Environment (IDE) like IntelliJ IDEA or Eclipse

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/encryption-decryption.git
   ```
2. Open the project in your preferred IDE.

3. Build and run the project.

## Usage

1. Launch the application.
2. Enter the text to be encrypted or decrypted in the input field.
3. Enter a key (between 1 and 25) in the key field.
4. Select either the "Encrypt" or "Decrypt" radio button.
5. Click the "Perform Selected Operation" button to see the result in the output area.

## Code Explanation

### Main Class: `EncryptionDecryption`

- **Attributes**:
  - `JTextField inputField`: Text field for user input.
  - `JTextField keyField`: Text field for the encryption/decryption key.
  - `JTextArea outputArea`: Text area for displaying output.
  - `JRadioButton encryptRadio`: Radio button for selecting encryption.
  - `JRadioButton decryptRadio`: Radio button for selecting decryption.
  - `ButtonGroup radioGroup`: Group for managing the radio buttons.

- **Methods**:
  - `EncryptionDecryption()`: Sets up the GUI, initializes components, and adds action listeners.
  - `encrypt(String input, int key)`: Encrypts the input text using the Caesar Cipher algorithm.
  - `decrypt(String input, int key)`: Decrypts the input text by reversing the encryption process.

### Example

```java
public class EncryptionDecryption extends JFrame {
    // GUI components and attributes

    public EncryptionDecryption() {
        // Setup GUI
    }

    private String encrypt(String input, int key) {
        // Encryption logic
    }

    private String decrypt(String input, int key) {
        // Decryption logic
    }

    public static void main(String[] args) {
        EncryptionDecryption ed = new EncryptionDecryption();
        ed.setVisible(true);
    }
}
```

## Future Scope

- **Advanced Algorithms**: Implement more sophisticated encryption algorithms such as AES or RSA.
- **User Management**: Add user authentication features to manage access to the application.
- **Web Application**: Develop a web-based version of the application for broader accessibility.
- **Mobile Application**: Create a mobile version for Android/iOS devices.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README as needed for your project.
