# ExoPlanet-detector
![image](https://user-images.githubusercontent.com/83130573/174457278-1b78377e-ac77-4b1f-a4e9-0acc7160cdd2.png)
## Summary
#### Machine Learning can help accelerate the time consuming data analysis process to find planets outside our solar system🪐! To achieve this, I trained Random Forest, Logistic Regression models, and Convolutional neural network (CNN) to detect the planet's transit signal with the data from the Kepler space telescope. Using accuracy, sensitivity and precision as performance evaluation metrics, these models scored:
| [Model](https://github.com/siudro/ExoPlanets-Classifier/tree/main/models) | [Random Forest](https://github.com/siudro/ExoPlanets-Classifier/blob/main/models/RandomForest/RandomForest3(best%20results).ipynb) | [Logistic Regression](https://github.com/siudro/ExoPlanets-Classifier/blob/main/models/Logistic-Regression/LogisticRegression4(best%20results)_.ipynb) | [CNN](https://github.com/siudro/ExoPlanets-Classifier/blob/main/models/CNN/CNN2(best%20results).ipynb) |
| :---: |     :---:      |          :---: |          :---: |
| Accuracy | 99.08%     | 99.08%    | 99.12%    |
| Precision | 99.08%       | 99.08%      | 100%    |
| Sensitivity(True detection rate) | 100%       | 100%      | 100%    |

#### All the [codes](https://github.com/siudro/ExoPlanets-Classifier/tree/main/models) and [details](https://github.com/siudro/ExoPlanets-Classifier/blob/main/Planetary%20Hunters%20Report.docx.pdf) are documented in this repo. I always appreciate your valuable feedback!
#### A very simplified and informative explanation on exoplanets and transit signals and how to use AI to detect them, data and data cleaning process in Arabic can be found [here](https://docs.google.com/presentation/d/1hBA3S2dAxeX4oug6FfbJNOPEeeGlCZIo/edit?usp=sharing&ouid=104485415291700481581&rtpof=true&sd=true)📑 
## Prerequisites
- [Pandas](https://pandas.pydata.org/getting_started.html)
- [NumPy](https://numpy.org/install/)
- [Matplotlib](https://matplotlib.org/)
- [Scikit Learn](https://scikit-learn.org/stable/index.html)
- [Scipy](https://scipy.org/)
- [TensorFlow](https://www.tensorflow.org/) and [Keras](https://keras.io/)
## What is an Exoplanet?
#### Exoplanet: *Extra-solar planet*, meaning that there are other stars that can be similar to our sun, that have planets orbiting around them and located outside our solar system.
## What is a planet's transit?
#### There are many ways to detect a planetary system, but the most used method is *time transit*.
#### A transit occurs when a planet passes in front of a star, resulting in a slight periodic drop in the star's light intensity, and is referred to as the *transit signal*.
![image](https://user-images.githubusercontent.com/83130573/174457671-a30cccc4-c9a6-4d03-a5dd-1b0b90fbc76e.png)
Source: *NASA Ames, 2021*
#### Once a transit signal is detected, we may use Kepler's third law of planetary motion to determine the planet's orbital size and the period required for the planet to orbit the star. These information are helpful to answer many questions about the planet, such as whether it is habitable or not!

## Data
#### Dataset of kepler's time series from [kagle](https://www.kaggle.com/keplersmachines/kepler-labelled-time-series-data)
![image](https://user-images.githubusercontent.com/83130573/145691208-2debe14f-139e-4cc1-953f-d8c3fd81131e.png)
#### more data can be found here:
1- https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html

2- https://exo.mast.stsci.edu/
## Data Preprocessing
#### Data splitting, removing outliers and instrumental noise, dropping nulls, reshaping values, then scaling and transformation have been performed, to make it easier to detect a transit-like signal.
 
## References
1. Thompson, S. E., Mullally, F., Coughlin, J., Christiansen, J. L., Henze, C. E., Haas, M.
R., & Burke, C. J. (2015). A machine learning technique to identify transit shaped
signals. The Astrophysical Journal, 812(1), 46. Retrieved from
https://iopscience.iop.org/article/10.1088/0004-637X/812/1/46/meta
2. Yeh, L. C., & Jiang, G. (2020). Searching for Possible Exoplanet Transits from BRITE
Data through a Machine Learning Technique. Publications of the Astronomical Society of
the Pacific, 133(1019), 014401, Retrieved from
https://iopscience.iop.org/article/10.1088/1538-3873/abbb24
3. Pearson, K. A. (2019). A Search for Multiplanet Systems with TESS Using a Bayesian
N-body Retrieval and Machine Learning. The Astronomical Journal, 158(6), 243.
Retrieved from https://iopscience.iop.org/article/10.3847/1538-3881/ab4e1c/meta
4. Malik, A., Moster, B. P., & Obermeier, C. (2020). Exoplanet Detection using Machine
Learning. arXiv preprint arXiv:2011.14135. Retrieved from
https://arxiv.org/abs/2011.14135
5. Priyadarshini, I., & Puri, V. (2021). A convolutional neural network (CNN) based
ensemble model for exoplanet detection. Earth Science Informatics, 14(2), 735-747.
Retrieved from https://link.springer.com/article/10.1007/s12145-021-00579-5
6. Kepler. (2018). NASA. Retrieved from
https://www.nasa.gov/mission_pages/kepler/overview/index.html
7. NASA, A Machine-Learning Algorithm Just Found 301 Additional Planets in Kepler
Data (November 26, 2021). Universe Today
https://www.universetoday.com/153441/a-machine-learning-algorithm-just-found-301-ad
ditional-planets-in-kepler-data/
8. Transit Method. (2021). Institute for Research on Exoplanets.
http://www.exoplanetes.umontreal.ca/transit-method/?lang=en
9. LightKurve documentation. Retrieved from https://docs.lightkurve.org/
10. N.A.S.A.A. (2021c, March 4). Light Curve of a Planet Transiting Its Star. Retrieved from
https://exoplanets.nasa.gov/resources/280/light-curve-of-a-planet-transiting-its-star/
11. P.B. (2015a). Finding Another Earth. Retrieved from
https://www.nasa.gov/jpl/finding-another-earth
