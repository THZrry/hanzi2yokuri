# Hanzi to Yokuri Voice converter
[中文](README_zhcn.md)
***
This is a simple tool to convert Chinese Hanzi to Kirakana with a similar sound.
Thanks to [cnfurikana](https://github.com/Gleiphir/cnfurikana/). This project uses data from cnfurikana and fixed for a better result when generating sentences.

# Data
`kana_ascii.json` is a json file with escape sequence. `kana_utf8.json` is plain text json with utf-8 encoding.

# Steps
## Spliting sentence
This uses `jieba`, a lightweight Chinese sentence spliting module. Many Chinese characters have multiple pronunciations in different contexts, and spliting helps generating right pinyin.
## Converting to pinyin
Pinyin is Romanized Chinese signing characters' pronunciations. `pypinyin` is a lightweight python module to do this.
## Converting to kirakana
There is a table containing all the pinyin to kirakana conversion.

# What can I do with this?
Yokuri voice is common in Chinese Touhou videos, which is pronounced in Japanese. This project is set to create them in a simple way.

# How to use
`kanalize.py`