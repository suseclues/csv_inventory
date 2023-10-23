# File Inventory Generator

This Python script generates a CSV file containing information about files in a folder. The CSV includes columns for relative path, file name, file extension, file size, last modified time, and file integrity information (md5 checksum).

## Usage

1. **Install Dependencies**

   If you're not using a Python editor such as Visual Studio Code, make sure you have Python installed on your system. The script uses standard Python libraries and should not require installing any additional packages. 

2. **Configure the Script**

   Open the script in a text editor or VS Code. Modify the `folder_path` variable to point to the folder containing the files you want to inventory.

   ```python
   folder_path = '/path/to/your/folder/'
   ```

   Also, update the `output_csv_path` variable to specify where you want to save your generated CSV file.

   ```python
   output_csv_path = '/path/to/file-manifest.csv'
   ```

3. **Run the Script**

   If you're using an application like Visual Studio code feel free to run it in there, otherwise open a terminal or command prompt and navigate to the directory containing the script.    Run the script with the following command:

   ```bash
   python file_inventory_generator.py
   ```

4. **Review Output**

   The script will generate a CSV file with the specified information above. You can find it at the location you specified in `output_csv_path`. Note: This script could also be edited to add additional columns.

## CSV Columns

- **Relative Path**: Path to the file from the specified starting point.
- **File Name**: Name of the file without the extension.
- **File Extension**: Type of file (e.g., txt, csv, pdf).
- **File Size (in bytes)**: Size of the file in bytes.
- **Last Modified Time**: Date and time when the file was last modified.
- **Checksum**: Representation of the file's contents for data integrity.

## Example

```
relative Path,file name,file extension,file size (in bytes),last modified,checksum
path/to/file_1,file_1,jpg,1024,2023-10-18 14:32:21,abcd1234
path/to/file_2,file_2,mp4,2048,2023-10-17 10:45:32,abcd1234
path/to/file_3,file_3,pdf,4096,2023-10-16 16:28:45,abcd1234
```
```
