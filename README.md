# MN Legislature Political Balance

Application to visualize with the political balance of the MN Legislature.

## Data processing

We need to convert the CSV to JSONP.

1. Install [csvkit](http://csvkit.readthedocs.org/en/latest/index.html).
1. `csvjson data/district-pvi.csv > visualizations/data/pvi.json; echo "pvi_callback(" > visualizations/data/pvi.jsonp; cat visualizations/data/pvi.json >> visualizations/data/pvi.jsonp; echo ");" >> visualizations/data/pvi.jsonp;`