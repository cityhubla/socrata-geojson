socrata-geojson
===============

Convert the data from a Socrata SODA 'geo' json endpoint to actual geoJSON.

This gives you another option to download the data if there are no available geojson's to download.

## Python Setup
- You need python 2.7 or higher for this to work
- OSX has python installed already
- Windows, you must install from [here](https://www.python.org/downloads/)
 - In order to call python and it's scripts from the command prompt you must set the environment variables in your Windows Settings, click [here](https://docs.python.org/2/using/windows.html) for instructions on step "3.3. Configuring Python"
 - Be sure to set both your python folder (ex. C:\python27) and the python script folder (ex. C:\python27\Scripts) to the settings.

## Installation

    pip install -r requirements.txt

## Usage
In the command prompt, terminal or git shell type the following

    python parse-socrata-json.py URL OUTFILE

You will end up with a valid GeoJSON file that contains all the objects from the Socrata response that have a location.

Try it with

    python parse-socrata-json.py https://data.lacity.org/resource/nnrh-gpbn.json 'nameofyournewgeojson'.geojson
