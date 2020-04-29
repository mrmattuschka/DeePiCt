# tomo-spectrum-matcher

Utility to normalize CryoET data by matching amplitude spectrums.

Currently it consists of two main components: 
- Extraction of a tomogram's radially averaged amplitude spectrum
- Applying an extracted spectrum to other tomograms

## Installation
- Clone the git repo
- Optional: create a new conda environment
```
    $ conda create -n tsm
    $ conda activate tsm
```
- Install requirements
```
    $ pip install requirements.txt
```
- Done!

## Usage
### Extracting an amplitude spectrum
To extract a tomogram's amplitude spectrum run:  
```$ python extract_spectrum.py --input <input_tomo.mrc> --output <amp_spectrum.tsv>```

### Match a tomogram to an extracted spectrum
To apply an extracted amplitude spectrum to another tomogram run:  
```$ python match_spectrum.py --input <imput_tomo.mrc> --target <amp_spectrum.tsv> --output <filtered_tomo.mrc>```

## TO DO
- Packaging
- Better CLI
  - Unify functionalities into one tool
  - Make tool accessible from PATH
- Add detailed algorithm explanation to README
- Make sigmoid cutoff adjustable