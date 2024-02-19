## Bash for Data Scientists

### Useful tools

- **cowsay**

```
# For macos
brew install cowsay

# For linux
sudo apt install cowsay
```

- **csvkit**

```
sudo apt-get install python-dev python-pip python-setuptools build-essential
pip install --upgrade setuptools
pip install --upgrade csvkit
```

### Useful commands

`csvgrep tmnt-with-header.csv --column=name --regex '^Leonardo' | csvlook -I`

| name     | nickname | mask_color | weapon        |
| -------- | -------- | ---------- | ------------- |
| Leonardo | Leo      | blue       | two ninjakens |


tìm trong file `tmnt-with-header.csv`, column `name` tìm tên `Leonardo`


`in2csv --names top2000.xlsx` : lấy sheet trong file top2000.xlsx

```bash
curl -sL "https://www.gutenberg.org/files/11/11-0.txt" | ➊
> tr '[:upper:]' '[:lower:]' | ➋
> grep -oE "[a-z\']{2,}" | ➌
> sort | ➍
> uniq -c | ➎
> sort -nr | ➏
> head -n 10 ➐
```
➊ Downloading an ebook using curl.
➋ Converting the entire text to lowercase using tr47.
➌ Extracting all the words using grep48 and put each word on separate line.
➍ Sort these words in alphabetical order using sort49.
➎ Remove all the duplicates and count how often each word appears in the list using uniq50.
➏ Sort this list of unique words by their count in descending order using sort.
➐ Keep only the top 10 lines (i.e., words) using head