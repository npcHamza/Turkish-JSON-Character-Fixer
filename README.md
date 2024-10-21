# Turkish JSON Character Fixer

This Python script automatically fixes issues with Turkish characters in JSON files that are incorrectly encoded in UTF-8. It specifically targets situations where Turkish characters are represented as Unicode escape sequences (e.g., `\uXXXX`) and converts them back to their original form.

## Features

- Reads all `.json` files from a specified directory and corrects Turkish character encoding issues.
- Saves the corrected files to a new directory, leaving the original files untouched.
- Writes the JSON files with indentation and new lines for improved readability.

## Requirements

- Python 3.x
- No additional libraries are required as the `json` and `os` modules are part of Python's standard library.

## Usage

1. Place the JSON files that need fixing in a folder named **json_files**.
2. The script will process the JSON files and save the corrected versions in a new folder named **corrected_json_files**.

### Steps

1. Clone the project or download the zip.
2. Activate your Python environment (if applicable).
3. Add your JSON files to the `json_files` directory.
4. Run the script in your terminal or command prompt:

   ```bash
   python turkish_json_fixer.py
   ```

5. Once the script finishes, you will find the corrected JSON files in the `corrected_json_files` folder.

## Example Folder Structure

```bash
project_folder/
│
├── turkish_json_fixer.py  # The Python script
├── json_files/            # Folder containing original JSON files
│   ├── file1.json
│   ├── file2.json
│   └── ...
├── corrected_json_files/   # Folder where fixed JSON files will be saved (created automatically)
└── README.md              # This README file
```

## Notes

- The script rewrites the JSON files in UTF-8 format, ensuring that all Turkish characters are displayed correctly.
- No changes are made to the original files in the `json_files` folder; all corrected files are saved in the `corrected_json_files` folder.
