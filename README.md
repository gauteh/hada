# HADA

## Setup

```
$ mamba env create -f environment.yml
$ conda activate hada
$ pip install -e .
$ hada --help
```

## Usage

Check out `hada --help`.

Retrieve all configured variables for the last 24 hours:

```
$ conda activate hada
$ hada --output last_24h.nc
```

Increase debug output, configure the bounding box (in longitude, latitude, resolution) and select only variables
containing 'temp':


```
$ hada --log-level=debug -v temp --bbox-deg 5,6,64,64.3 --dx 0.01 --dy 0.01 --output test3.nc
```
