# Input Data

Unfortunately the input data is too large to host on github, but it is available from [Kaggle](https://www.kaggle.com/dcohen21/8anu-climbing-logbook).

## About the Data

It was collected from the website [8a.nu](https://www.8a.nu/) by David Cohen. This dataset was collected on 9/13/2017.

The idea behind [8a.nu](https://www.8a.nu/) is to provide a logbook for climbers to keep track of their climbs digitally. Many climbers have a manual logbook that they use to keep track of this information, and [8a.nu](https://www.8a.nu/) provides a digital alternative to this. Fortunately for us this means we have a wealth of information available.

## Import the Data

The download from [Kaggle](https://www.kaggle.com/dcohen21/8anu-climbing-logbook) is in sqlite format, which is nice, but pandas seemed to read this information quite slowly so I converted each of the tables within the database into csv's from the sqlite3 interface. Pandas reads the csv files much faster.

To use this repo you will need to perform the same conversion of `sqlite` to `csv` files. It's quite straight forward. Conversely, it would also be quite trivial to modify the cleaning notebook to read the `sqlite` file and create the resulting csv files. As this is a one time operation (now) it might not be a problem that it is slow.
