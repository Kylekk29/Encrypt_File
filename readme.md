**English** | [简体中文](README.zh-CN.md)

# Encrypt File

A small desktop tool to encrypt and decrypt files with a key you control. Pick files, load or generate a key, click **Encrypt** or **Decrypt**. Nothing leaves your computer.

## Features

- Select several files at once
- Generate a new key file, or load one you saved before
- Choose where each encrypted or decrypted copy is saved
- Symmetric encryption (Fernet from the `cryptography` library)

## How to use

1. Click **Generate Key** and save the `.key` file somewhere safe, or **Load Key** to use an existing one.
2. Click **Load File** and pick one or more files.
3. Click **Encrypt File** or **Decrypt File**, then choose the name and folder for each result.

> ⚠️ **Keep your key safe.** Lose it and the encrypted files cannot be opened. Anyone with the key can open them. Test with a non-important file first.

If decryption fails (for example the wrong key), an error is printed in the console.

## Run from source

Python 3 with Tkinter (included in the standard Windows installer).

```bash
pip install -r requirements.txt
python encrypt.py
```

## License

MIT, see [LICENSE](LICENSE).
