# 🔨 nlp2 🔧

Tools for NLP using Python

This repertory used to handle file io and string cleaning/parsing

## Usage

Install:

```
pip install nlp2
```

Before using :
```
from nlp2 import *
```


# Features

###File Handling

## get_folders_form_dir(path)
Arguments
- `path(String)` : getting all folders under this path (string)
Returns
- `path(String)(generator)` : path of folders under arguments path
## get_files_from_dir(path)
Arguments
- `path(String)` : getting all files under this path (string)
Returns
- `path(String)(generator)` : path of files under arguments path
## read_dir_files_into_lines(path)
Arguments
- `path(String)` : getting all files line by lines under this path (string)
Returns
- `line(String)(generator)` : files line under arguments path
## read_files_into_lines(path)
Arguments
- `path(String)` : getting content in input file path (string)
Returns
- `path(String)(generator)` : file line under arguments path

### String cleaning/parsing

## lines_into_sentence(lines)
Arguments
- `lines(Array(String))` : lines array 
Returns
- `path(String)(generator)` : split all line base on punctuations
## split_sentence_to_ngram(text)
Arguments
- `path(String)` : sentence to ngram
 
Returns
- `ngrams(Array)` : ngrams array  

Examples  
```
split_sentence_to_ngram("加州旅館")
return ['加','加州',"加州旅","加州旅館","州","州旅","州旅館","旅","旅館","館"]
```
## split_sentence_to_ngram_inpart(text)
Arguments
- `path(String)` : sentence to ngram
Returns
- `path(String)(generator)` : multiple ngrams array in different start character  
Examples  
```
split_sentence_to_ngram("加州旅館")
return [['加','加州',"加州旅","加州旅館"],["州","州旅","州旅館"],["旅","旅館"],["館"]]
```
## spilt_text_to_combine_ways(text)
Arguments
- `text(String)` : input text
Returns
- `path(String)(generator)` : all of the text combines ways
Examples  
```
spilt_text_to_combine_ways("加州旅館")
return ['加 州 旅 館', '加 州 旅館', '加 州旅 館', '加 州旅館', '加州 旅館', '加州旅 館', '加州旅館']
```
## spilt_sentence_to_array(sentence)
Arguments
- `sentence(String)` : input text
Returns
- `sentencearray(Array)` : sentence array
## is_all_english(text)
Arguments
- `text(String)` : input text
Returns
- `result(Boolean)` : whether the text is all English or not
## is_contain_number(text)
Arguments
- `text(String)` : input text
Returns
- `result(Boolean)` : whether the text contain number or not
## is_contain_english(text)
Arguments
- `text(String)` : input text
Returns
- `result(Boolean)` : whether the text contain english or not
## full2half(text)
Arguments
- `string(String)` : input string which needs turn to half
Returns
- `(String)` : a half-string
## half2full(text)
Arguments
- `text(String)` : input string which needs turn to full
Returns
- `(String)` : a full-string
