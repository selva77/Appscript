# WSR Automation for ABC Project

This Google Apps Script project simplifies tasks related to weekly status reports (WSRs) for the ABC project. It covers the following:

1. **Email Distribution:** Sends the latest WSR (as a PDF) from a designated folder to a specified email list. The email message and subject line are customizable.

2. **Archiving:**  Creates a dated copy of the WSR in an archive folder for easy historical reference. It then renames the currently active WSR for clarity. 

## Installation

1. **Create a Copy:**  Open this Google Apps Script project in your Google Drive and make a copy.
2. **Replace Placeholders:** Find the placeholders in the code marked with `<< >>` and replace them with:
   * Your WSR file's Drive Folder ID 
   * Your archive folder's  Drive Folder ID
   * Email addresses for the distribution list (`to` and `cc`) 
3. **Permissions:** When you first execute the script, Google Apps Script will request permissions to access your Drive and send emails on your behalf. Please review and grant these permissions. 

## Usage

* You can run the script directly from the Apps Script editor for manual execution.
* To automate the process, set up a time-driven trigger for weekly execution from within the Apps Script project.

## Customization

* **`folderId` and `archiveFolderId` (near the top):** Adjust  these if your folder locations change.
* **`emailAddresses`, `ccemailAddresses`:**  Modify the recipient lists.
* **`message`:** Tailor the default email body.
* **`subject`:**  Edit the subject line if needed.

## Important Notes

* The script assumes that weekly status reports are in PDF format. If you use a different file type, the code will need to be adjusted.
* Archiving copies files with a `YYYYMMDD` datestamp added to the original filename.

## Contributions

Contributions to improve this script are welcome!  Please follow these guidelines:
*  [Insert contribution guidelines or a link to your CONTRIBUTING.md file]

## License

This project is licensed under [the MIT License](https://choosealicense.com/licenses/mit/) (or specify your preferred license). 

## Contact

* For questions or support: selvaj@google.com
