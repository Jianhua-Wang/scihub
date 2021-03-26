![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/suqingdong/scihub)
![GitHub Release Date](https://img.shields.io/github/release-date/suqingdong/scihub)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/suqingdong/scihub)
![GitHub branch checks state](https://img.shields.io/github/checks-status/suqingdong/scihub/master)
![Python Version](https://img.shields.io/badge/python-v3.8-blue)

<div>
<img src="https://suqingdong.github.io/scihub/examples/raven_1.png" height=55>
<img src="https://suqingdong.github.io/scihub/examples/logo_en.png" height=50>
</div>

# PDF Downloader with SCI-HUB
![](https://suqingdong.github.io/scihub/examples/tutorial.gif)

### Advantages
- could detect url automaticly
- could download in batches
- could run in command line mode

### Installation
```bash
pip3 install sci-hub
# or
python3 -m pip install sci-hub
```

### Command Line Examples
```bash
# checking available urls
scihub -c

# searching pmid(s)
scihub -s 1,2,3

# searching doi
scihub -s 10.1038/s41524-017-0032-0

# searching with a file
scihub -s pmid-list.txt

# searching with a specific url
scihub -s 1 -u https://sci-hub.ren

# name the output file by searching string
scihub -s 123 -ns

# specify the output directory
scihub -s 1,2,3 -O out

# overwrite or not when file exists, default will ask
scihub -s 1,2,3 -ow N
scihub -s 1,2,3 -ow Y
```

### Acknowledgement
- URL Detecting From: https://lovescihub.wordpress.com/