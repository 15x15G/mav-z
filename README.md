# Mastodon Archive Viewer (modified by slshyn 11/09/2020)
A html script to take a mastodon archive and convert it into a human-readable webpage for viewing. Currently available as a hacky html file with some inline JS. 

# Features:
## original
* organizes your old posts into a conveniently readable timeline
* includes media attachments in posts
* Preserves content warnings/summaries
* Tries to use the header from the archive as the background
* Tries to use the avatar from the archive as the avatar next to your old posts
## modified by slshyn 11/07/2020 
* fixed a few link problems
* prettier interface, more similar to mastodon dark theme
* more details from the toots and user profile added
## modified by slshyn 11/08/2020 
* separate page on only toots & media
* archive column on months and year, stick on the screen when scroll down
* back to top button when scroll down
## modified by slshyn 11/09/2020 
* added click to open image
* fixed a few visual problems
* added scroll on archive column
* added open link on a new tab when click
## fixed by slshyn 11/10/2020 
* fixed picture display problem
* modified .sticky column

# Usage
<b>With Python (unchanged, can still work as the original viewer):</b>
* To make a webpage to view your archive, just place the `html_from_archive.py` script in the root of the archive (the folder that has `outbox.json` and `media_attachments` in it) and run it using python3 
* From the command line: `python3 html_from_archive.py`
* You can also set it as executable and run it directly or, on Windows, right click and open it with python 3.
* Open the resulting `processed_archive.html` file in your web browser.

<b>Without Python (modified by slshyn):</b>

* Download the `archive_page.html` file. Place it in the root of the archive (the folder that has `outbox.json` and `media_attachments/` in it).
* Open `archive_page.html` in your web browser. Open the `actor.json` and `outbox.json` file from within the page and it will load it.


# Next steps:

- [x] separate page on only toots & media
	- [x] make medias easier to view
	- [x] click to open pictures (why `addEventListener click` didn't work...)
- [ ] prettier interface

Open to suggestions. Chinese and English ok.
