# my_code_challenge
my_code_challenge


# Unit test for Invalid Data
https://pandas.pydata.org/pandas-docs/version/0.21.0/timeseries.html

```python

Invalid Data
Note In version 0.17.0, the default for to_datetime is now errors='raise', rather than errors='ignore'. This means that invalid parsing will raise rather that return the original input as in previous versions.
The default behavior, errors='raise', is to raise when unparseable:

In [2]: pd.to_datetime(['2009/07/31', 'asd'], errors='raise')
ValueError: Unknown string format
Pass errors='ignore' to return the original input when unparseable:

In [34]: pd.to_datetime(['2009/07/31', 'asd'], errors='ignore')
Out[34]: array(['2009/07/31', 'asd'], dtype=object)
Pass errors='coerce' to convert unparseable data to NaT (not a time):

In [35]: pd.to_datetime(['2009/07/31', 'asd'], errors='coerce')
Out[35]: DatetimeIndex(['2009-07-31', 'NaT'], dtype='datetime64[ns]', freq=None)

```
