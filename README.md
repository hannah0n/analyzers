# analyzers
Runnable Morphological Analysis Tools from the UniMorph Project

## Warning

This software is at an **alpha** stage. 

## Prerequisites

[DirecTL+](https://github.com/GarrettNicolai/DTL)

[CTranslate](https://github.com/OpenNMT/CTranslate)



## Installation
Due to the size of DirecTL+ models, we do not include them here; please contact gnicola2 AT jhu DOT edu for pre-trained models.
Uncompress DTL models into models/DTL directory. See **releases** tab above to download.

```
tar -xvzf DTLModel.tgz
```

Set environment variables to point to required binaries.

```
export DTL=<location of DTL binary>
export CTRANSLATE=<location of ctranslate binary>
```

## Usage

```
python src/analyze.py -i input.wordlist -a output.analyses -l language
```

For example:

```
python analyze.py -i Welsh.toAnalyze -a Welsh.out -l welsh
```


## Supported Languages

```
adyghe, albanian, amharic, arabic, armenian, asturian, azeri
bashkir, basque, belarusian, bengali, breton, bulgarian, 
catalan, cornish, crimean-tatar, czech, danish, dutch,
english, estonian, faroese, finnish, french, friulian, galician,
georgian, german, greek, greenlandic, haida, hebrew, hindi, 
hungarian, icelandic, indonesian, ingrian, irish, italian, 
kabardian, kannada, karelian, kashubian, kazakh, khakas,
khaling, kurmanji, ladin, latin, latvian, lithuanian, livonian, 
lower-sorbian, macedonian, maltese, mapudungun, middle-high-german,
middle-low-german, murrinhpatha, navajo, neapolitan, norman,
northern-sami, norwegian-bokmaal, norwegian-nynorsk, occitan,
old-armenian, old-french, old-irish, old-saxon, pastho, persian,
polish, portuguese, quechua, romanian, russian, sanskrit, 
scottish-gaelic, serbo-croatian, slovak, slovene, sorani,
spanish, swahili, swedish, tagalog, tamil, tatar, telugu, 
tibetan, turkish, turkmen, ukrainian, urdu, uzbek, venetian, welsh, 
west-frisian, yiddish, zulu, ...
```
