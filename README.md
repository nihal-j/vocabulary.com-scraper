# vocabulary.com Scraper

This repository contains scripts to make retrieving and using lists and definitions on <a href=www.vocabulary.com>vocabulary.com</a> easier. <br/>
Users may find this very helpful while preparing for exams such as GRE, SAT, etc. <br/>

## Usage

`vocabulary_list.py` script can be used to read a list on <a href=www.vocabulary.com>vocabulary.com</a> and store it locally in JSON and CSV formats.
```shell
python3 vocabulary_list.py --list_no <list_number> --name <output_file_name> --verbose <True/False>
```
Sample usage:
```shell
python3 vocabulary_list.py --list_no 6832259 --name common-deck-1 --verbose True
```
<hr></hr>

`vocabulary.py` script can be used to get word definition for single words from <a href=www.vocabulary.com>vocabulary.com</a>.
```shell
python3 vocabulary.py --word <word>
```
Sample usage:
```shell
python3 vocabulary.py --word pontificate
```

<hr></hr>

`add_word.py` script can be used to update an existing dictionary of learnt words.
```shell
python3 add_word.py --word <word> --name <output_file_name>
```
Sample usage:
```shell
python3 add_word.py --word annals
```
Note: `name` argument is optional, defaults to `dictionary.csv`.

<hr></hr>

`add_list.sh` script can be used to add a list of words to existing dictionary of learnt words.
```shell
bash add_list.sh <list_name>
```