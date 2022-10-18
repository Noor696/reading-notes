## Read 08 Data Analysis with Pandas

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

[Real Python - Pandas Tutorials](https://realpython.com/learning-paths/pandas-data-science/)

* Pandas is a Python library used for working with data sets.

* It has functions for analyzing, cleaning, exploring, and manipulating data.
   - analyzing : Pandas allows us to analyze big data and make conclusions based on statistical theories.
   - cleaning : Pandas can clean messy data sets, and make them readable and relevant, able to delete rows that are not relevant, or contains wrong values, like empty or NULL values.

* The name "Pandas" has a reference to both "Panel Data", and "Python Data Analysis"

* Install Panda using this command:
 > C:\Users\Your Name>pip install pandas

* import it in your applications by adding the import keyword:
 > import pandas

* Example : 
 > import pandas
 mydataset = {
  'cars': ["BMW", "Volvo", "Ford"],
  'passings': [3, 7, 2]
  }
  myvar = pandas.DataFrame(mydataset
  print(myvar)

* Pandas is usually imported under the pd alias.
 > import pandas as pd

 Now the Pandas package can be referred to as pd instead of pandas.
 > myvar = pd.DataFrame(mydataset)

* Checking Pandas Version:
 > import pandas as pd
 print(pd.__version__)

### Refrencing
[w3schools-pandas_intro](https://www.w3schools.com/python/pandas/pandas_intro.asp)

[youtube-Pandas](https://www.youtube.com/watch?v=3ISW655DemU&list=PLvLvlVqNQGHCb2_ygmr1DQOMOv0yXp84F)


