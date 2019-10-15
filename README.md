# phagocyte

### What's that?

Phagocyte is an app to get all the multimedia content from telegram groups and channels and aggregate in a common place. So, it's a "phagocyte" de facto.

Main goal is to have a list of resources (groups and channels with interesting content. Then, get all this content, for example, ebook files, and control duplicates, corrupted files and whatever. After this, program creates a list of uploadable stuff to destinty channels defined, and move the files to a local repository and also register a unique reference for each file in a MySQL database.

Next batch of files from another resource must be compared with database and/or repository file to avoid duplicates and so on.

When a list of files is ready to be uploaded, files are processed in order to categoryze, if possible, extract comments, graphic cover, and so on.

Filetypes processed:

| extension | cover | comments | author | date | language | other metadata |
|-----------|-------|----------|--------|------|----------|----------------|
| epub      |  yes  |   yes    |  yes   |  yes |    yes   |                |
| mobi      |  yes  |   yes    |  yes   |  yes |    yes   |                |
| pdf       |  yes  |    no    |   no   |   no |     no   |                |
| cbr       |  yes  |    no    |   no   |   no |     no   |                |
| cbz       |  yes  |    no    |   no   |   no |     no   |                |
