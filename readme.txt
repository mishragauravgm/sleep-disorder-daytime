#Gaurav Mishra, Nov 10, 2022, CS7180

OS Used:MacOS X on Jupyter Notebooks

Libraries Required: They have been mentioned in the requirements.txt file and a simple 'pip install -r requirement.txt' should install those libraries.

The Feature_Generation+Modeling.ipynb is the main module that does predictive modeling. If you run the code by setting the current directory as the same directory in which the notebook is stored, it should run seamlessly. 

<You may choose to ignore the notebook below as it takes up a lot of compute time and storage as well>
The ECG_to_data.ipynb basically converts the raw data to CSVs which is then used by the notebook above. The data provided is in EDF format which requires processing. It saves all the converted data as all_data.csv in the data folder. It is a time-consuming process and yields all_data.csv as the main file which is then manipulated by the notebook above to generate features and do some predictive modeling. This notebook basically results in generation of all_data.csv which is like a central dataset for this task. Only all_data.csv will be used in the next notebook and for all future purposes. In the intermediate steps from edf to all_data.csv(~300MB), a lot of other csvs are generates which are ~10GB in size. 


To ensure that the size uploaded on Gradescope is minimal, I have only included the raw txt files and the final all_data.csv. If you choose to generate the data from the raw files you may run ECG_to_data.ipynb notebook. If not, you can directly move to Feature_Generation+Modeling.ipynb