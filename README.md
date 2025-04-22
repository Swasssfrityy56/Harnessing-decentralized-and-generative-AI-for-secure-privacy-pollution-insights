# Harnessing-decentralized-and-generative-AI-for-secure-privacy-pollution-insights
 Air pollution poses a significant threat to global health, contributing to millions of deaths annually. This project presents a comparative analysis of NO, NO₂, and NOₓ levels across five capital cities in the southern states of India. The research integrates both real-world datasets and synthetic data generated using a diffusionbased generative AI model. Preprocessing techniques, including outlier removal and data visualization through heatmaps, are employed to enhance data quality and interpretability.<br>      
     To facilitate decentralized and privacypreserving analysis, federated learning is implemented using the Flower framework, with time series deep learning models deployed across the cities. Model performance is evaluated using MSE, RMSE, MAE, and R² metrics. Federated learning in environmental monitoring is implemented using the Flower Framework with time series Deep learning models precisely LSTM, GRU, LSTM_GRU, LSTM_BIGRU, GRU_BILSTM, Transformer_GRU where LSTM outperformed with R2 score of 0.7059 and 0.7542 for real data and the synthetic data. 
# Methodlogy
 The dataset used in this project comprises of data from different southern cities of India namely Amaravathi, Bangalore, Chennai, Hyderabad and Thiruvananthapuram which consists of 22784, 48192, 48192, 48107 and 26654 respectively. The total dataset of the five cities comprises of 193929 samples and 5 attributes individually in each city. <br>
      This dataset is based on regression which uses continuous timeseries data in hourly basis. According to the observation the data of each city contained outliers and missing values, as 
shown in the below figure. The images are the example of graphical representation of removal of outliers and missing values of bangalore dataset.

![image](https://github.com/user-attachments/assets/6941ac7b-48bd-4e60-8dea-c3b80f390b56)

![image](https://github.com/user-attachments/assets/fdafc92d-f9be-4aca-b9c6-f2673864f2ad)

Flowchart

![image](https://github.com/user-attachments/assets/c4afefa0-6e2f-415c-949a-b801689d257d)

The proposed framework presents a comparative  study for air pollutant prediction using both real and synthetic data within a federated learning environment. The system begins with the preparation of datasets collected from five major Indian cities: Amaravati, Bengaluru, Chennai, Hyderabad, and Thiruvananthapuram. These datasets undergo preprocessing to handle outliers and missing values, ensuring data quality. Post preprocessing, the data is divided into two branches. 

One branch utilizes the cleaned real data, while the other employs a generative diffusion model to produce synthetic data, by strengthening dataset diversity and aiding in model generalization. Both data sets are used to train a variety of deep learning models, including LSTM, GRU, BILSTM, BIGRU, and Transformer-based hybrid models. The trained models are deployed across distributed clients in a federated learning setup. A central server coordinates the training by aggregating model updates from each client, preserving data privacy and enabling collaborative learning. Finally, the system evaluates performance using standard metrics such as MSE, RMSE, MAE, and R² to assess accuracy. This architecture ensures robust, scalable, and privacy-preserving pollutant level prediction across multiple urban locations.

#Results
Results of Federated Learning For Real Data

IMPLEMENTATION OF FEDERATED LEARNING FOR REAL DATA<br>
MODEL	      ROUND	LOSS	MAE	MSE	R2	RMSE<br>
LSTM	       1	0.0225	0.1195	0.0225	0.4256	0.1503<br>
	       2	0.0135	0.0737	0.0135	0.7026	0.1164<br>
	       3	0.0134	0.073	0.0134	0.7059	0.1158<br>
GRU	       1	0.014	0.0805	0.014	0.6683	0.1218<br>
	       2	0.0133	0.0738	0.0133	0.7062	0.1156<br>
	       3	0.0132	0.074	0.0132	0.7029	0.1151<br>
GRU_LSTM       1	0.0157	0.0816	0.0157	0.6474	0.0125<br>
	       2	0.0138	0.0749	0.0138	0.6969	0.1177<br>
	       3	0.0134	0.0729	0.0134	0.7037	0.1158<br>
GRU_BiLSTM     1	0.0156	0.087	0.0156	0.6526	0.1252<br>
	       2	0.0137	0.0741	0.0137	0.7025	0.1171<br>
	       3	0.0134	0.0742	0.0134	0.7028	0.1159<br>
LSTM_BiGRU     1	0.0188	0.0979	0.0188	0.5687	0.1374<br>
	       2	0.0225	0.1074	0.0225	0.4754	0.1502<br>
	       3	0.0277	0.1242	0.0277	0.3078	0.1665<br>
Transformer_LSTM 1      0.0559	0.1803	0.0559	0.5158	0.2365<br>
	       2	0.0193	0.1004	0.0193	0.5756	0.1392<br>
	       3	0.0161	0.0865	0.0161	0.6492	0.127<br>
Transformer_GRU	1	0.0608	0.2205	0.0608	0.5896	0.2465<br>
	       2	0.0167	0.0941	0.0167	0.6122	0.1295<br>
	       3	0.0144	0.0795	0.0144	0.6797	0.1203<br>
