# Setting Up Tesseract: A Step-by-Step Guide

Tesseract is a popular open-source Optical Character Recognition (OCR) engine that can extract text from images. This guide will walk you through the steps to install and set up Tesseract on your computer, whether you're using macOS, Windows, or Linux.

## Step 1: Installing Tesseract

### macOS

To install Tesseract on macOS, you’ll need to use Homebrew, a package manager for macOS.

1. **Install Homebrew (if not already installed)**:
   - You may need to install X-code command line tools first! This package will allow other packages (including Homebrew) to execute commands. Open Terminal and run:

   ```bash
   xcode-select --install
   ```

   - Then install [Homebrew](https://brew.sh/), which will act as a manager for a lot of other packages you need to install. Run the following command:

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Tesseract**:
   - Once Homebrew is installed, run the following command in Terminal:

     ```bash
     brew install tesseract
     ```

   - This will install Tesseract on your system.

### Windows

1. **Download the Installer**:
   - Go to the [Tesseract download page](https://tesseract-ocr.github.io/tessdoc/Installation.html) and download the latest Windows installer. Scroll down to the "Windows" section and follow the links to download from "Tesseract at UB Mannheim". Unless you have a very old computer, make sure to download the 64-bit installer.

2. **Run the Installer**

   - Once the installer is downloaded, run the package. Note the setup path that the package is installed to.

3. **Add Tesseract to the system PATH.**

    - Open the start search, type in "env," and choose "Edit the system environment variables"
    - Click the "Environment Variables..." on the dialog that opens up
    - Find the row under "System Variables" for "Path." Select "Path" and click "Edit..."
    - A new dialog will pop up. Click on "New" and paste in the path from the installer. It will look something like `C:\Program Files\Tesseract-OCR`
    - Click "Ok" to save the changes

4. **Verify Installation**:
   - Open Command Prompt and type:

     ```bash
     tesseract --version
     ```

   - If installed correctly, this command will display the version of Tesseract you have installed.

## Step 2: Running Tesseract

Now that Tesseract is installed, you can start using it to extract text from images.

### Basic Usage

**Run Tesseract on an Image**:
   - To extract text from an image called `image.png`, use:

     ```bash
     tesseract image.png output
     ```

   - This command creates a file called `output.txt` with the extracted text.

### Output to PDF

Tesseract can also generate searchable PDFs:

```bash
tesseract image.png output pdf
```

This command creates a file called `output.pdf`.
