# Dir for Source

This dir contains the source to experiment with:
    * numpy
    * pandas
    * tensorflow
    * keras

It contains the `requirements.txt` file for setup and notes
regarding the different tested runtimes.

It also contains the [vscode setup instructions](vscode_setup.md) notes.


# Source Notes

Currently, these notebooks run in vs code as jupyter notebooks.  The goal is to 
have them run in Google Collab, Vertex AI, AWS and IBM cloud environments.


The notebooks are separated into two components:
    * notebooks for generating data
        - Generally they read from an input csv file and write to csv files in the same location
        - Reads from `data/xxx.csv`` and writes to `[data/train|test|valid].csv`
            - simple clean data no norm 
                - simply reads a csv file and writes to train,test, and valid csv files using pandas.
            - simple clean data no norm with augmentation
                - reads a csv file and writes augmented data (additional slightly modified data) to train,test, and valid csv files using pandas for the simple model dtv1.
            - simple clean data
            - water clean data
                - uses `data\usgs_gsvb_v2.csv` as data input and writes train, test, valid
    * notebooks for using data to do model experiments
        - simple model dtv1
            - does a regressor to model X + Y = Z using a Keras/TensorFlow DNN
        - water model dtv
            - defines, trains and validates a model for virtual water sensor using Keras/TensorFlow DNN