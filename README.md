# ContactManager14

ContactManager14 is a simple command-line application written in Java that allows users to manage their contacts. The application supports adding, displaying, and deleting contacts, with an additional feature of encrypting and decrypting the contact data using AES encryption.

## Features

- **Add Contact**: Add a contact with a name and phone number. The contact is encrypted before being saved.
- **Display Contacts**: Display all the saved contacts by decrypting the contact information.
- **Delete Contact**: (To be implemented) Remove a contact from the list after decrypting the stored data.
- **Encryption**: All contact information is stored in an encrypted format using AES encryption for enhanced security.

## Technologies Used

- **Java**: Core programming language.
- **Java Cryptography Extension (JCE)**: Used for AES encryption and decryption of contact data.
- **Serialization**: Used for storing and retrieving contact objects from a file.

## Prerequisites

Before running the ContactManager14 application, make sure you have the following:

- **Java Development Kit (JDK)** version 8 or later installed.
- A terminal or command-line interface (CLI) for running the program.

## How to Run

### 1. Clone the repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/Kabilash01/ContactManager.git
cd ContactManager
### ## How to Run

### 2. Compile the Java files

Navigate to the directory where the `ContactManager14.java` file is located and compile it using the following command:

```bash
javac ContactManager14.java
### 3.Run the application
After compiling the code, you can run the application with:
```bash
java ContactManager14

###Project Structure
ContactManager/
│
├── ContactManager14.java     # Main class with logic for managing contacts
├── Contact.java              # Contact class representing contact information
├── contacts.ser              # File where encrypted contacts are stored (generated after adding contacts)
├── README.md                 # Project documentation
└── .gitignore                # Ignore compiled class files and serialized data

###Encryption
The application uses AES (Advanced Encryption Standard) for encrypting and decrypting contact information before saving it to and retrieving it from the file contacts.ser. The encryption key is hardcoded in the program as *"secretKey1234567"*, but in a real-world application, you would use more secure key management practices.

###To-Do
Implement the Delete Contact functionality.
Improve file handling to support multiple contacts in a single file.
Enhance encryption key management to use secure and dynamic key generation.

