# Airbnb-NYC-analysis-on-a-dynamic-page

## Introduction

Streamlit is an awesome new tool that allows engineers to quickly build highly interactive web applications around their data, machine learning models, and pretty much anything. It gives you a blazingly fast, iterative, and interactive development loop

The best thing about Streamlit is it doesn’t require any knowledge of web development but just some basic python knowledge.

This repository is an example to build interactive web application by using streamlit and python.

The st.cache decorator indicates that Streamlit will perform internal magic so that the data will be downloaded only once and cached for future use.

Behind the scenes, Streamlit keeps track of the function name, the code in the function body, and the input arguments we pass in the function call. Upon first invocation, it stores the function’s return value in a local cache. Upon subsequent invocations of the function with the exact same arguments, Streamlit returns the result from the local cache.

The main limitation of Streamlit’s data caching is that it cannot keep track of changes to the data happening outside the function body.

## Functions

Some basic functions of streamlit:

**st.title** is suitable for the main title. For section titles, use **st.header** or **st.subheader**.

**st.markdown** renders any string written using Github-flavored Markdown. It also supports HTML but Streamlit advises against allowing it due to potential user security concerns.

**st.map** displays locations on a map without having to write a single line of boilerplate code to prepare a map object. The only requirement is that the dataframe must contain columns named lat/latitude or lon/longitude.

**st.table** displays a static table. 

We display a histogram of property prices displayed as a Plotly chart using **st.plotly_chart**.

We use **st.slider** to provide a slider that allows selecting a custom range for the histogram. We tuck it away into a **sidebar**.

Using **st.radio**, we show a list items to select from. Also, we create checkbox using **st.checkbox**.

**st.write** accepts strings, dataframes, dictionaries, plots, maps, and so on (full list in the documentation). It allows passing in multiple arguments, and its behavior depends on their types.

**st.pyplot** renders plots built using matplotlib.

We display an error message using **st.error**.

Use **st.image** to show images

Use **st.button** to create a button

## Applications

Check out the source code and application website to dig out more!

## References and links

Full code of the Streamlit app created for this tutorial: https://github.com/shaildeliwala/experiments/blob/master/streamlit.py

From Adrien Treuille, the co-founder of Streamlit: https://towardsdatascience.com/coding-ml-tools-like-you-code-ml-models-ddba3357eace

Streamlit API documentation: https://streamlit.io/docs/api.html

Streamlit demo video: https://youtu.be/B2iAodr0fOo

Airbnb NYC listings data (unofficial): http://data.insideairbnb.com/united-states/ny/new-york-city/2019-09-12/visualisations/listings.csv

Plotly histogram documentation: https://plot.ly/python/histograms/
