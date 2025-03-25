# MediaCrypt

MediaCrypt is a Python-based tool that lets you hide text inside media files and pull it back out with a key.

## Features
- Hides text in media files (like `.wav`, `.mp3`, etc.).
- Creates a key file for decryption.

## Requirements
- Python 3.x (for source code, when it’s out)
- Nothing extra needed for the `.exe` files

## Installation
The source code isn’t up yet but will be on GitHub later:
   ```bash
   git clone https://github.com/ZailoxTT/MediaCrypt.git
   ```
For now, just grab the `encrypt.exe` and `decrypt.exe` files to use the tool.

## Usage

### Encryption
1. Run `encrypt.exe`:
   ```bash
   encrypt.exe
   ```
2. Enter these when asked:
   - `Text to encrypt`: The message you want to hide.
   - `Key file`: Where to save the key (e.g., `key.txt`).
   - `Original media file`: The media file to use (e.g., `song.wav`).
3. The text gets added to the media file, and the key is saved.

### Decryption
1. Run `decrypt.exe`:
   ```bash
   decrypt.exe
   ```
2. Enter these when asked:
   - `Media file`: The media file with hidden text.
   - `Key file`: The key file from encryption.
   - `Save decrypted to`: Where to save the text (e.g., `output.txt`).
3. The original text gets pulled out and saved.

## How It Works
- **Encryption**: The text is hidden in the media file, and a key file is made to unlock it later.
- **Decryption**: The tool reads the hidden text from the file and uses the key to reveal it.

## Limitations
- Only letters (A–Z, a–z, А-Я, а-я) get hidden; other characters stay as-is.
- Big texts might make the file size obviously larger.
- Works best with files like `.wav` that don’t mind extra data at the end.

## Example
### Encryption
```bash
Text to encrypt: Hello, World!
Key file: key.txt
Original media file: song.wav
```
Output: Text hidden in `song.wav`, key saved in `key.txt`.

### Decryption
```bash
Media file: song.wav
Key file: key.txt
Save decrypted to: output.txt
```
Output: `Hello, World!` saved to `output.txt`.

## License
This will be under lLicense - check the [LICENSE](LICENSE) file when the source code drops.
