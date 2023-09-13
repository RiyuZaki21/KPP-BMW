# KPP-BMW

import streamlit as st 
import numpy as np 
import matplotlib.pyplot as plt

st.header("KPP BMW peminatan C")
st.subheader('Riyu Zaki Rizqulloh Putra Ardi ')
ecg1 = np.loadtxt('Data ECG.txt', dtype = 'float')
Ndata1 = len(ecg1)
ECG = np.arange(Ndata1)
st.line_chart(ecg1)
plt.figure(figsize=(18,8))
plt.plot(ECG, ecg1)
st.pyplot(plt)
