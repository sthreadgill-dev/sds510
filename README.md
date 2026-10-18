# SDS 510

Project work for SDS 510 at Arizona State University.
**Instructor:** [Alex Halavais](http://alex.halavais.net/bio)

## Module 1: Basic Toolkit

- `bash_session.txt`: bash session recorded with `script`, showing file navigation, `curl`, `tar` and `grep` searches of the data in WSL
- `accessed_records.txt`: output of `grep`, which shows the rows whose filename contains "education" and end in ".txt"

The source data (`log.csv`, from `log.tar.gz`) is not included because of its size. To recreate it:

    curl -s -L https://www.dropbox.com/s/14jagxjbzhyxg8g/log.tar.gz -o log.tar.gz
    tar -xzvf log.tar.gz
