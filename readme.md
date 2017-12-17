# CATSS LXX Data

## Updates

### 2017-12-17
Work continues with the parallel files. Currently I am still processing the Hebrew/Greek columns, which require quite a bit of regex patterns and exceptions. Especially troublesome are the CATSS text critical notations, which are either poorly documented or there are many mistakes in the parallel files. This has caused delays in the parallel module development. Once the data is processed though, I will begin making the slot connections. But that too is likely to take a while due to the quirky nature of the LXX text. 

### 2017-12-16
New UTF8 feature added to the surface form of words using James Tauber's [Greek utilities](https://github.com/jtauber/greek-utils) for processing the Betacode transcriptions. There is not yet utf8 for lexemes.

### 2017-12-11
New features and corrections added:<br> 
* Now morphology has been extracted from the morphology codes. These new features are in [tf/enrichments](tf/enrichments). In total there are 11 new features: `typ` [part of speech], `styp` [subtype of part of speech], `lex` [lexeme], `case`, `gender`, `number`, `tense`, `voice`, `mood`, `person`, `degree` [comparative/superlative for adjectives].
* all values are mostly self-explanatory with the exception of the feature `styp`, see the [CCAT Morphology documentation](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxmorph/*Morph-Coding) to decode.
* all data has been extracted from the `morph` feature as stored in the "PARSE" code of CATSS. See link above for its explanation. 

## Provenance
This is a [Text-Fabric](https://github.com/Dans-labs/text-fabric) resource (python3) converted from the [publicly available](http://ccat.sas.upenn.edu/rak//catss.html) CATSS Septuagint database. CATSS stands for "Computer Assisted Tools for Septuagint/Scriptural Study." The data is supplied by the University of Pennsynvania's Center for Computer Analysis of Texts (CCAT).

Future versions of this dataset will include links to the Eep Talstra Centre for Bible and Computer's [BHSA Hebrew Database](https://github.com/ETCBC/bhsa) for use in statistical studies between the Hebrew Bible and Greek Septuagint.

*Note that the source datafiles are ignored and not uploaded to the repo since they are already available (see link above). 

Please read the CCAT [user agreement](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxmorph/0-user-declaration.txt). It is the user's responsibility to follow the relevant copyright guidelines. 
