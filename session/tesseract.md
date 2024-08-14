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

   - Then install Homebrew, which will act as a manager for a lot of other packages you need to install. Run the following command:

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
   - Go to the [Tesseract download page](https://github.com/tesseract-ocr/tesseract/wiki) and download the latest Windows installer.

2. **Install Tesseract**:
   - Run the installer you downloaded.
   - During installation, make sure to select the option to add Tesseract to your system’s PATH. This will allow you to run Tesseract from the command line.

3. **Verify Installation**:
   - Open Command Prompt and type:

     ```bash
     tesseract -v
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
