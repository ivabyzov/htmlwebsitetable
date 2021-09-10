import pandas as pd
import numpy as np
from unicodedata import normalize
import ssl
ssl._create_default_https_context = ssl._create_unverified_context

table_born = pd.read_html('https://worldtable.info/gosudarstvo/tablica-rozhdaemosti-po-godam-rossija.html', header=0)

df_born = table_born[0]

df_born['Количество родившихся чел.'] = df_born['Количество родившихся чел.'].apply(lambda x: int(x.replace(' ','')))
df_born['Год'] = df_born['Год'].apply(lambda x: int(x))

df_born
