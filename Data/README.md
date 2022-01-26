

## Data

**Data Folder** contains two sub-folders: 
* **Synthetic Data Folder** includes training data and testing data generated; 
* **RCT Data Folder** contains real-world RCT data which has been split into training and testing.

### Synthetic Data Folder
This folder contains generated simulation data files with two types (training and testing) and four uncertainty levels. These data files are used for offline evaluation mentioned in section 5.1. These data files were generated following the description in section A.2, with different uncertainty weight levels. The unobserved variable was specifically discarded from training data to satisfy the "unobserved" condition.

Each training sample was attributed with the following:

1. **ID** - Column[0], data unique ID.
2. **Heterogeneous Variables** - Column[1-4].
3. **Treatment Variable** - Column[5], with four different level of treatments.
4. **Outcome Variables** - Column[6-7], Value and Cost under BTS problem setting.




### RCT Data Folder
This folder contains web-scale RCT data collected from a video streaming platform which was used as training instances. 
The dataset records the users' campaign engagement duration (i.e., outcome) in seven randomly enrolled incentive groups, each offered bonuses at different levels (i.e., multi-treatment). In the experiments of Section 5.2, our dataset consists of over 100 K app visit instances. 

Due to the protected coypright of the data, currently we are not able to disclose all the actual data used in our experiments until we get authorization but the practitioner can use the code provided to run this algorithm on other dataset. 
Note, a small part (about 2000 samples) of real-world data are provided in **Data Folder** just for running the code, **NOT FOR REPRODUCE THE RESULT** in Section 5.2, and **ALL THE 2000 SAMPLES HAVE BEEN ENCRYPTED**. As stated in the paper, the complete dataset used in offline test will be released upon we get authorization.

**RCT Data** - In order to let reader learn some meaning of our real-world RCT data features, we only introduce some of them.

1.  Column[1] - total number of campaign active days in the last 30 days.
2.  Column[4] - total number of video views in the last 30 days.
3.  Column[5] - number of fans.


