#REAL WORLD PROBLEM


This case-study focuses on generating music automatically using Recurrent Neural Network(RNN). We do not necessarily have to be a music expert in order to generate music. Even a non expert can generate a decent quality music using RNN. We all like to listen interesting music and if there is some way to generate music automatically, particularly decent quality music then it's a big leap in the world of music industry. Task: Our task here is to take some existing music data then train a model using this existing data. The model has to learn the patterns in music that we humans enjoy. Once it learns this, the model should be able to generate new_ music for us. It cannot simply copy-paste from the training data. It has to understand the patterns of music to generate new music. We here are not expecting our model to generate new music which is of professional quality, but we want it to generate a decent quality music which should be melodious and good to hear. Now, what is music? In short music is nothing but a sequence of musical notes. Our input to the model is a sequence of musical events/notes. Our output will be new sequence of musical events/notes. In this case-study we have limited our self to single instrument music as this is our first cut model. In future, we can extend this to multiple instrument music.

DATA SOURCE


https://www.humdrum.org/Humdrum/representations/kern.html

How to Run the Model 


First we need to preprocess the kern datafile using “preprocessing.py”. Then we load the preproccessed data to “train.py”.
In order to train the model you can run the file " train.py" 	Or you load the already trained test model “model1.h5” to “melody generator.py” We ran our model for total of 80 epochs. You can add more layers into your model and fine tune the existing layers in the model. Any epoch weight can be loaded for fine tuning or "Transfer Learning". But due to time constraint and complexity we have limited our model to a dual layer lstm.


How to Generate Music Sequence


Once the model is defined and weights are calculated then run "melodygenerator.py" file and to listen to the music generated we can select “mel1.mid” and to view the musical notation select the same file with musescore.


Prerequisites


1.	Python 3(Pycharm)
2.	Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
3.	Keras
4.	Music21
5.	museScore


Installing


1.	Pycharm
2.	Anaconda
3.	Keras:pip install keras
4.	Music21:pip install music21
5.	Install MuseScore

Built With


•	PyCharm- Python Text Editor
•	numpy, scipy- number python library
•	pandas - data handling library
•	Keras - Deep Learning Library
•	MuseScore- Music data visualization /Output as sheet music and play midi files
