# bikesharing
Module 14 repository


### Deliverable 1 Requirements

The data in the "tripduration" column is converted to a datetime datatype and has the correct time format (15 pt)
The DataFrame is exported as a new file without the index column (5 pt)

```python
# 3. Convert the 'tripduration' column to datetime datatype.
bikeshare_df['tripduration']= pd.to_datetime(bikeshare_df['tripduration'], unit='s')
```

![Deliverable 1 snapshot](resources/deliverable1_modified_DF_head.png)

```python
# 5. Export the Dataframe as a new CSV file without the index.
bikeshare_df.to_csv('bikeshare-tripdata-edited.csv', index = False)
```