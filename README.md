# Quality of Service Forecasting with LSTM Neural Networks

An evaluation of QoS forecast methods described in paper Quality of Service Forecasting with LSTM Neural Networks

### Abstract
A robust and accurate forecast of the Quality of Service (QoS) attributes is essential for effective web service recommendation, enhanced user experience, and service management. Deep learning methods, especially Long Short-Term Memory Neural Networks (LSTM NN), have proven to be worthy for sequence forecasting in various domains recently. In this paper, we pilot an experimental application of LSTM NN in the domain of QoS forecasting. We develop a LSTM NN model for QoS prediction and compare its forecast performance with existing approaches for QoS attribute forecasting -- ARIMA and Holt-Winters models. The approaches are compared on two real-world QoS attribute datasets created using centralized passive QoS attribute collection technique. Our results show that LSTM NN improves the accuracy of QoS forecast for attributes collected with high granularity while maintaining a reasonable computation time.

### Prerequisities
* Jupyter notebook (http://jupyter.org/)
* Python 3 (https://www.python.org/)
* Numpy (http://www.numpy.org/)
* Pandas (https://pandas.pydata.org/)
* Matplotlib (https://matplotlib.org/)
* Statsmodels (http://www.statsmodels.org/)
* Keras (https://keras.io/)
* Scikit-learn (http://scikit-learn.org/)

All of these Python libraries are available via Pip install tool (e.g. python3 -m pip install *package*).

### Analyses

All analyses are present in *analyses/SERV-x/* directories. To run any analysis yourself, you need to start your own Jupyter notebook session and load selected analysis.

### Acknowledgement

The data collection and technical implementation and evaluation of the experiment were supported by the Technology Agency of the Czech Republic under No. TA04010062 "Research and Development of Advanced Analytics Tools for Security and Performance Analysis of Network Infrastructure, Applications and Services". The state-of-the-art description, methodology of the experiment, and results discussion was supported by "CyberSecurity, CyberCrime and Critical Information Infrastructures Center of Excellence" (No. CZ.02.1.01/0.0/0.0/16\_019/0000822) supported by ERDF.
