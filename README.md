# Simple File Maker in shell

This is a basic Bash script (`fileMaker.sh`) that helps you quickly create a new file with a custom name, extension, and content. It's useful for generating simple files like `.txt`, `.sh`, or other custom extensions directly from the terminal.

## 📜 Features

- Choose any file extension (e.g., `txt`, `sh`, `md`)
- Name your file
- Enter the content to be written into the file
- Automatically saves the file in the same directory as the script

## 🧠 How It Works

The script uses `tput` to color the terminal text and `read` to get user input for:

1. File extension  
2. File name  
3. File contents  

It then writes the provided content to a new file in the script's directory.

## 🛠️ Usage

1. Open your terminal.  
2. Navigate to the directory containing the script.  
3. Make the script executable:

   ```bash
   chmod +x fileMaker.sh
   ```

4. Run the script:

   ```bash
   ./fileMaker.sh
   ```

5. Follow the prompts:
   - Enter a file extension (e.g., `txt`, `sh`)
   - Enter the file name
   - Enter the content for the file

The new file will be created in the same folder as the script.

## 💡 Example

```
whats your files extension exampels are txt or sh
> txt

Hey what do you want to call your file
> hello

what do you want to write inside of this file
> Hello, world!
```

✅ A file called `hello.txt` will be created in the script's directory containing:

```
Hello, world!
```

## 🖥️ Requirements

- Bash shell  
- Unix-like OS (Linux, macOS, WSL)

## 🔐 Notes

- The script does not escape special characters, so be careful with quotes or code that could break the script.
- It writes to the current directory of the script, not where you're calling it from.
