---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

A large portion of the people studying Cantonese are starting from a place of loving the language. Figuring out the technical pieces of the story is a secondary task and has not received consistent focused effort. As a community of developers we need to identify how to make the existing data better available to researchers, users, teachers, and learners of Cantonese.

This effort on datasets includes:
- Reviewing, cleaning, and (with permission), republishing existing data sets.
- Converting existing datasets into interoperable and maintainable formats.
- Creating new datasets.

Beyond merely capturing the datasets, we must also make that data beneficial to researchers, users, teachers, and learners of Cantonese. This requires both improving existing tooling and identifying missing tools and building them.

## Table of Contents

- [Datasets](#datasets)
- [Input Method Editors](#input-method-editors)
- [Romanization and Syllabarization Tools](#romanization-and-syllabarization-tools)
- [Character Sets](#character-sets)
- [Learning Tools](#learning-tools)
- [Publishing Tools](#publishing-tools)
- [Captioning and Coding (in the research sense) Tools](#captioning-and-coding-tools)
- [Machine Translation](#machine-translation)
- [Voice Recognition](#voice-recognition)
- [Optical Character Recognition](#optical-character-recognition)
- [Word Segmentation](#word-segmentation)
- [Grammar and Spell Checking](#grammar-and-spell-checking)
- [Dictionaries](#dictionaries)
- [Sign Language](#sign-language)
- [Character Compendium](#character-compendium)
- [Fonts](#fonts)
- [Locale Handling for Translation](#locale-handling-for-translation)
- [Text-To-Speech and Voices](#text-to-speech-and-voices)
- [Content](#content)

***

## Datasets

There are a lot of datasets available in poorly interoperable formats that could benefit from consolidation & maintenance.

- ISO-10646HK produced a ["Cantonese Pronunciation List of the Characters for Computers"](https://www.iso10646hk.net/download/jp/doc/JPTableFull.pdf) data sheet, but it is only available in PDF. It was last updated on September 7, 2004. It needs ongoing review.
- [Wenlin has produced a Cantonese dictionary.](https://wenlin.co/wow/Project:Jyut)
- The [Hong Kong Education Bureau](https://www.edb.gov.hk) has hired a contractor to build and maintain a [Lexical Items with English Explanations for Fundamental Chinese Learning in Hong Kong Schools](https://www.edbchinese.hk/lexlist_en/).
- Education University of Hong Kong has produced an [online dictionary](https://corpus.eduhk.hk/cantonese/search/).
- [CantoDict](http://www.cantonese.sheik.co.uk/dictionary/) is an open source Cantonese dictionary.
- Pleco has created [CC-Canto](https://cantonese.org/) which builds upon data from CC-CEDICT.
- [Words.hk](https://words.hk/) exists as a third open source Cantonese dictionary.
- [Research Centre for Humanities Computing at CUHK](https://humanum.arts.cuhk.edu.hk/) has produced the [Multi-function Chinese Character Database](https://humanum.arts.cuhk.edu.hk/Lexis/lexi-mf/).
- [CUHK Language Acquisition Laboratory](http://www.arts.cuhk.edu.hk/~lal/) has produced the [Hong Kong Cantonese Child Language Corpus (CANCORP)](http://www.arts.cuhk.edu.hk/~lal/corpora.html#CANCORP).
- CUHK has produced many resources:
  - [Lexis: A Chinese Syllabary Pronounced according to the Dialect of Canton](https://humanum.arts.cuhk.edu.hk/Lexis/Canton/)
  - [Lexis: A Chinese Talking Syllabary of the Cantonese Dialect](https://humanum.arts.cuhk.edu.hk/Lexis/Canton2/)
  - [Lexis: Chinese Character Frequency](https://humanum.arts.cuhk.edu.hk/Lexis/chifreq/)
  - [Lexis: Chinese-English Dictionary of Modern English](https://humanum.arts.cuhk.edu.hk/Lexis/Lindict/)
  - SWIF: Spoken/Written/Informal/Formal Dictionary (based upon the Education University of Hong Kong corpus.)
- CXTerm uses a dictionary originally produced by 李枫峰 (Fung-Fung Lee), the designer of the HZ character encoding.
  - [The oldest copy I can find is this, which contains license restrictions.](http://web.mit.edu/babel/zhongwen/lib/dict/CTCPS3.tit) "Permission for the use and redistribution is granted by the author as long as it is freely distributed for non-commerical purposes."
  - [CXTerm uses a version updated in 1993](https://gitee.com/xucs007/cxterm/raw/master/dict/gb/CTLau.tit)

## Input Method Editors

Input Method Editors that work across all platforms should be created. These input method editors should use the same training data for autocompletion across each platform.

Target platforms:
- iOS
- macOS
- Windows
- Android
- ChromeOS
- Linux

Input method types:
- Drawing
- Stroke
- Cangjie
- Phonetic
- Others?

To make for an optimum experience for multi-platform users, all training data should be centrally synced to enable consistent experiences across platforms.

## Romanization and Syllabarization Tools

Jyutping has become the standard format for Cantonese romanization to form a syllabary for Cantonese. There are, however, many other existing romanizations of Cantonese. Tools should be built for full conversion between:

- Jyutping (Prefix numeric, Postfix numeric, Diacritics)
- Yale (Prefix numeric, Postfix numeric, Diacritics)
- IPA
- SL Wong
- Sidney Lau
- Penkyamp
- Cantonese Pinyin
- Canton Romanization

## Character Sets

Historical Chinese language input has been reencoded many different times. In order to not lose previously created documents to time, point-in-time to point-in-time character set conversion should be offered. This should be configurable based upon known-shipped mapping tables with possible errors as well as standards-based idealistic methodolgy.

- HZ
- Big5
- ISO 10646
- HKSCS
- Unicode
- Others

## Learning Tools

A language must have learning tools in order to help the next generation of users learn it. Cantonese has a limited set of material available for it. This project should build:

- Flash Card Templates
  - Preconstructed flash card sets for known exam targets (KS1, KS2).
- Dynamic Question Generators for time, money, numbers, and other calculateable patterns.
- Character Writing Practice Tools, stroke-by-stroke
  - Songti
  - Kaiti
  - Heiti

## Publishing Tools

There are very few books published in Cantonese. This project should aim to make it as easy as possible to publish a book either *in* Cantonese, or to *teach* Cantonese. These tools should allow for streamlined publishing as an Ebook, PDF, print-on-demand, or even full publishing runs. This should also likely include tools for TeX and publishing of research articles.

## Captioning and Coding Tools

A large portion of the material that uses the Cantonese language comes from spoken sources. To make that more-accessible for machine processing it will need to be serialized from audio sources into written data sets. These data sets will need to be coded in order to provide additional required data at post-processing time.

## Machine Translation

Current machine translation of Cantonese is not very precise. This could be made better.

## Voice Recognition

Voice recognition for Cantonese requires massive amounts of data. An effort should be undertaken, possibly in partnership with Mozilla Common Voice, in order to capture as much data as possible.

## Optical Character Recognition

Support for handwriting, Songti, Kaiti, and Heiti.

## Word Segmentation

Identifying word boundaries in written Cantonese is a difficult task. This should be implemented in a way that is API-compatible with ICU (or tools that build on top of it) and uses more-complete data sets and/or better models.

This can be used as an input to improved [line breaking tools](http://userguide.icu-project.org/boundaryanalysis).

## Grammar and Spell Checking

After identifying word boundaries, in combination with a list of confusables, check for mistyped characters based upon sound, adjacency, and other signals. This should *also* work for romanizations of Cantonese.

## Dictionaries

The existing dictionaries are all flat lists. They do not implement strong relationship models that would act as an enabler for additional research and learning models built on top of them.

These dictionaries should support Sense:Cantonese lookup across a variety of languages, prioritizing Cantonese, Mandarin, and English.

## Sign Language

Provide tools for learning sign language as a user, and as a translator.

## Character Compendium

Character information regarding history and construction should be consolidated in order to make for simpler learning. Examples of common mnemonics for particular characters should be included.

## Fonts

There are thousands of characters. There exists programmatic tools for generating characters such as the [Wenlin Character Description Language](http://wenlin.com/cdl) which can be adopted to fill in gaps prior to further standardization of characters.

Further, identifying, creating, and distributing high quality open source fonts should be a priority. A high-quality open source Songti, Heiti, and Kaiti font should all be released.

A programmatic font may be extremely valuable to speed up adoption of new characters.

## Locale Handling for Translation

There should be a standard fallback procedure to ensure that more Chinese-language materials are better-localized for different populations, whether they are diaspora, Taiwan, Hong Kong, Macau, Singapore, or Mainland.

This should be clever about BCP-47 fallback ordering.

## Text-To-Speech and Voices

Given a passage in written Cantonese, turn it into spoken Cantonese. This should *also* support the translation from written formats to spoken formats.

The voices should be natural, with speakers from different locales and of different genders, as well as full-robotic for assistive technology users.

## Content

Above all, the more content that exists in Cantonese, the better the situation is for all Cantonese users.
