# Harnessing-decentralized-and-generative-AI-for-secure-privacy-pollution-insights
 Air pollution poses a significant threat to global health, contributing to millions of deaths annually. This project presents a comparative analysis of NO, NO₂, and NOₓ levels across five capital cities in the southern states of India. The research integrates both real-world datasets and synthetic data generated using a diffusionbased generative AI model. Preprocessing techniques, including outlier removal and data visualization through heatmaps, are employed to enhance data quality and interpretability.<br>      
     To facilitate decentralized and privacypreserving analysis, federated learning is implemented using the Flower framework, with time series deep learning models deployed across the cities. Model performance is evaluated using MSE, RMSE, MAE, and R² metrics. Federated learning in environmental monitoring is implemented using the Flower Framework with time series Deep learning models precisely LSTM, GRU, LSTM_GRU, LSTM_BIGRU, GRU_BILSTM, Transformer_GRU where LSTM outperformed with R2 score of 0.7059 and 0.7542 for real data and the synthetic data. 
# Methodlogy
 The dataset used in this project comprises of data from different southern cities of India namely Amaravathi, Bangalore, Chennai, Hyderabad and Thiruvananthapuram which consists of 22784, 48192, 48192, 48107 and 26654 respectively. The total dataset of the five cities comprises of 193929 samples and 5 attributes individually in each city. <br>
      This dataset is based on regression which uses continuous timeseries data in hourly basis. According to the observation the data of each city contained outliers and missing values, as 
shown in the below figure. The images are the example of graphical representation of removal of outliers and missing values of bangalore dataset.

![image](https://github.com/user-attachments/assets/6941ac7b-48bd-4e60-8dea-c3b80f390b56)

![image](https://github.com/user-attachments/assets/fdafc92d-f9be-4aca-b9c6-f2673864f2ad)

