# Project
# [Instagram Reach Analysis exploration]
###### I've been studying Instagram reach for a long time. Every time I post a post on my Instagram account, I collect data on how well that post reaches in a week. This helps to understand how the Instagram algorithm works. If you want to analyze the reach of your Instagram account, you will have to collect the data manually, as there are some APIs, but they don't work well. Therefore, it is better to collect Instagram data manually.
###### Now let's get down to the task of analyzing the reach of my Instagram account by importing the necessary Python libraries and a dataset :

###### import pandas as pd
import plotly.graph_objs as go
import plotly.express as px
import plotly.io as pio
pio.templates.default = "plotly_white"

data = pd.read_csv("https://docs.google.com/spreadsheets/d/e/2PACX-1vTeWBHEZcdrfPTwC8drmZBWbWjhbpvpIAs61ouUwmiUsVBKnAI6uGMAdMYeBVdiPClc-hcurwfg4gRa/pub?gid=2074512117&single=true&output=csv", encoding = 'latin-1')
print(data.head())

![image](https://user-images.githubusercontent.com/118888509/236623609-73a8ace8-3a9e-4eb1-9d8f-8625f424890d.png)

###### I'm converting the Date column to datetime data type to move forward:
###### data['Date'] = pd.to_datetime(data['Date'])
print(data.head())

###### ![image](https://user-images.githubusercontent.com/118888509/236623717-ff435612-ba74-44c9-8ea4-6b271276aac2.png)

###### Analysis of Instagram's accessibility trends over time using a line graph.
