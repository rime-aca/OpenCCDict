## OpenCCDict
1. simp2trad is an streamlined convertor which inproves the phrase conversion quality greatly.
2. ch2emoji performs a conversion from Chinese to Emoji, regardless of how you input the Chinese, providing an intuitive way to input emoji.
---
## Usage
1. Put the txt files together with the json file in 'opencc' directory under your Rime’s user directory;
2. Customise the schema file and add these to the corresponding sections:
```
switches:
  - name: show_emoji
    reset: 1
    states: [ "🈚️️\uFE0E", "🈶️️\uFE0F" ]
engine:
  filters:
    - simplifier@emoji_conversion
emoji_conversion:
  opencc_config: emoji.json
  option_name: show_emoji
  tags: abc
```
3. Deploy.
