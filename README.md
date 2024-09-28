# PRODIGY_CS_02
IMAGE ENCRYPTION
Overview
This project provides a tool to encrypt and decrypt images using a secure encryption algorithm, powered by the Pillow library for image manipulation. The project ensures the confidentiality of image data, converting them into a format that is unreadable without the correct decryption key.
The project requires a Pillow libary. To install Pillow, use pip install Pillow
Once Pillow is installed, you can verify the installation by opening a Python shell and importing the library using python on the Commmand Line shell.
Then, in the Python shell, try import PIL, then print(PIL.__version__)
If Pillow was installed correctly, it should print out the version number of Pillow.
In your project’s Python script, you can now use Pillow like this:
from PIL import Image

# Example: Open an image file
image = Image.open('example.png')
image.show()

Encrypt an Image
To encrypt an image using Pillow for image processing and AES for encryption, use the following command:
python encrypt.py --input your_image.png --output encrypted_image.enc --key your_key

To decrypt an encrypted image and restore it to its original form,use:
python decrypt.py --input encrypted_image.enc --output decrypted_image.png --key

Thanks to the Pillow library, the following image formats are supported:
PNG
JPEG
BMP
TIFF
GIF

Installation
Clone the repository:

git clone https://github.com/DarkHorse06-dev/PRODIGY_CS_02.git
cd image-encryption

Limitations
The encryption key must be kept secure. Without the key, the encrypted image cannot be decrypted.
Large images may require more memory and processing time during encryption and decryption.
The image file size may increase slightly due to the encryption overhead.
