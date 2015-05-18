# DumpConverter [![Build Status](https://travis-ci.org/WikidataQuality/DumpConverter.svg)](https://travis-ci.org/WikidataQuality/DumpConverter)  [![Coverage Status](https://coveralls.io/repos/WikidataQuality/DumpConverter/badge.svg?branch=master)](https://coveralls.io/r/WikidataQuality/DumpConverter?branch=master) [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/WikidataQuality/DumpConverter/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/WikidataQuality/DumpConverter/?branch=master)
Downloads and parses dumps of databases for external validation in [Wikidata](https://www.wikidata.org) using the [WikibaseQualityExternalValidation](https://github.com/wikimedia/mediawiki-extensions-WikidataQualityExternalValidation) extension. 

## Installation
DumpConverter requires libxml2 and libxslt to be installed. To install the required development packages of these dependencies on Linux systems, use your distribution specific installation tool, e.g. apt-get on Debian/Ubuntu.

```sudo apt-get install libxml2-dev libxslt-dev python-dev```

To install DumpConverter, just run the setup script.

```
git clone https://github.com/WikidataQuality/DumpConverter.git
sudo pip install -e DumpConverter
```

## Usage
`python dumpconverter.py [options]`  

**Options**
* `--list-databases` list all available databases, that can be imported and exit
* `-d / --database DATABASE` name of a specific database that should be imported
* `-o / --output-file OUTPUT_FILE` output file for data values of dumps - default: external_data.tar
* `-q / --quiet` suppress output
