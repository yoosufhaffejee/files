# GitHub File Downloader

This web application allows users to download files from a GitHub repository, including the ability to merge split files or download them as separate parts. It also supports selecting local files, viewing file details, and splitting large files into smaller chunks for easier download.

## Features

- **Download files from GitHub**: Fetch and download files from a specified GitHub repository.
- **Merge and download file parts**: If a file is split into multiple parts (e.g., `file.part1`, `file.part2`), the app allows users to merge them and download the combined file.
- **Local folder selection**: Users can select files from their local system and download merged files.
- **Split large files**: Files larger than 100MB can be split into smaller chunks for easier downloading.

## How to Use

### 1. Clone the Repository
To get started, clone the repository to your local machine:

```bash
git clone https://github.com/<your-username>/github-file-downloader.git
cd github-file-downloader
```

### 2. Open the Application

Simply open the `index.html` file in any modern web browser to start using the application.

### 3. GitHub File Downloader

- The app will automatically load the files from a specified GitHub repository (`yoosufhaffejee/files`).
- The file list will be displayed with options to download or merge and download parts.
  
### 4. Local Folder Selection

- You can select a local folder using the file input.
- The application will show valid files (based on extensions) and display their size and chunk count.
- If the files are part files, you can download them as a single merged file.

### 5. Splitting Large Files

- Upload files larger than 100MB, and the app will split them into smaller chunks for easier downloading.
- After splitting, each chunk will be automatically downloaded.

## Supported File Types

The app supports the following file extensions:

- **Text and Document**: `.pdf`, `.txt`, `.doc`, `.docx`, `.rtf`, `.odt`, `.csv`, `.md`, `.xlsx`, `.xls`, `.pptx`, `.ppt`
- **Images**: `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.webp`, `.svg`
- **Audio**: `.mp3`, `.wav`, `.ogg`, `.flac`, `.aac`, `.m4a`
- **Video**: `.mp4`, `.mov`, `.avi`, `.mkv`, `.webm`, `.flv`
- **Archives**: `.zip`, `.tar`, `.rar`, `.7z`, `.iso`, `.tar.gz`, `.tar.bz2`, `.tar.xz`

## How It Works

- **GitHub File Fetching**: The app uses GitHub's public API to retrieve files from a given repository and displays valid files for download.
- **Local File Handling**: Local files are filtered by their extensions, and users can merge or download the files directly.
- **File Splitting**: The application splits files larger than 100MB into smaller 50MB chunks using the `FileReader` API.

## Requirements

- Modern web browser (Chrome, Firefox, Safari, etc.)
- No server-side setup required (client-side only)

## Contributing

Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is open-source and available under the MIT License.

---