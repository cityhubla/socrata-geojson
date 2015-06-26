socrata-geojson
===============

Convert the data from a Socrata SODA 'geo' json endpoint to actual geoJSON

## Python Setup
- You need python 2.7 or higher for this to work
- OSX has python installed already
- Windows, you must install from [here](https://www.python.org/downloads/)

## Installation

    pip install -r requirements.txt

## Usage
In the command prompt, terminal or git shell type the following

    python parse-socrata-json.py URL OUTFILE

You will end up with a valid GeoJSON file that contains all the objects from the Socrata response that have a location.

Try it with

    python parse-socrata-json.py https://data.lacity.org/resource/nnrh-gpbn.json 'nameofyournewgeojson'.geojson
