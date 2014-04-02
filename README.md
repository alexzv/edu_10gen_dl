# EdX powered courses video downloader

This script is intended to download course videos from https://university.mongodb.com
or any other site 'Powered by EdX' (including, of course, http://edx.org itself).

This script relies on [youtube-dl](https://github.com/rg3/youtube-dl/) project
to download videos.

Accepts destination path as optional parameter.

###Dependencies:

* Python 2.7
* Mechanize
* BeautifulSoup4
* Youtube\_dl

### Installation

    git clone https://github.com/nonsleepr/edu_10gen_dl.git
    cd edu_10gen_dl
    sudo pip install -r requirements.txt

Populate `config.py` with domain and credentials of site, from which you're going to download videos.

Optionally set another options in `config.py` like `writesubtitles` to enable subtitles.

### Usage:

+ `python edx_dl.py`
+ `python edx_dl.py c:\Users\MyUser\Lectures\`
+ `python edx_dl.py --interactive c:\Users\MyUser\Lectures\`
