# Canvas Downloader
Automate the download of all module attachments from your Canvas courses.  Maybe it's the end of the year and you want to save all the notes the teacher has made.

## Requirements
Python, selenium, tqdm, geckodriver, unix system.

The program might not work on Windows machines.  Symlinks are used to change the download directory without changing the Firefox download directory preference.

## Usage
Get the geckodriver if you do not have one already from here: https://github.com/mozilla/geckodriver/releases

Edit `config.py` with your preferences, including the geckodriver location, your school's Canvas url, and the course IDs of the courses that you want to download.  The course ID is just the numbers after courses/ in the url.

Edit `mimetypes.txt` with the mime types of the files that you want to download.  One line for each mime type.  Included already are pdf, docx, and pptx.

Now you can run the program.

`python main.py`

Then enter your login credentials in the selenium webdriver.  After the main Canvas page has loaded, press enter in the terminal and the program will download files to the `./downloads`.
