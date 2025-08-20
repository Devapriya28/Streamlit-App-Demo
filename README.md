# Streamlit-App-Demo
This Streamlit app is an interactive web application built with Python and Streamlit. It demonstrates how data, models, and visualizations can be combined into a user-friendly dashboard.

#first step-----pip install
!pip install streamlit

#second step-----code
import streamlit as st                             

st.title("Simple Streamlit App")

name = st.text_input("Enter Your Name?")           
age = st.slider("Select your age:", 1, 100, 18)

if st.button("Show Result"):
    st.success(f"Hello {name}! your age is {age}")

import pandas as pd

df = pd.DataFrame({"data": [2, 4, 1, 4, 1, 8]})
st.line_chart(df)

#third step-------run
!streamlit run app.py #! symbol is used to run system commands 
                      #directly from inside the notebook.
