[English](readme.md) | **简体中文**

# Encrypt File（文件加密工具）

一个小巧的桌面工具，用你自己掌握的密钥加密和解密文件。选好文件，加载或生成密钥，点击**加密**或**解密**即可。所有操作都在你的电脑上完成，不会上传任何内容。

## 功能

- 可一次选择多个文件
- 生成新的密钥文件，或加载以前保存的密钥
- 自行选择每个加密或解密结果的保存位置
- 对称加密（使用 `cryptography` 库的 Fernet）

## 使用方法

1. 点击 **Generate Key** 生成密钥，把 `.key` 文件存放在安全的地方；或点击 **Load Key** 加载已有密钥。
2. 点击 **Load File**，选择一个或多个文件。
3. 点击 **Encrypt File** 或 **Decrypt File**，再为每个结果选择文件名和文件夹。

> ⚠️ **请妥善保管密钥。** 密钥丢失，加密文件就无法打开；任何拿到密钥的人都能打开它们。请先用不重要的文件试一遍。

如果解密失败（例如密钥不对），控制台会打印错误信息。

## 从源码运行

需要 Python 3 和 Tkinter（Windows 标准安装包已包含）。

```bash
pip install -r requirements.txt
python encrypt.py
```

## 许可证

MIT，见 [LICENSE](LICENSE)。
