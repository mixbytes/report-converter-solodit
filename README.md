# Convert to Solodit

## Install
```
pip3 install docopt
```

## Run
Download reports from the MixBytes public reports repository: https://github.com/mixbytes/audits_public
Copy all the data from https://github.com/mixbytes/audits_public to the root of this repository and print data for the Solodit in JSON format:
```
python3 convert.py
```

Additional options can be set via `config.json` or command line:
```
python3 convert.py -h
```

## Problems

Some reports are **skipped** because they do not have vulnerability titles. Those reports are replaced with EMPTY file in `config.json`