# Movies_ETL

## Challenge

Amazing Prime wants the ablitity to keep the dataset we created updated. We are atsked with creating an automated pipeline that takes in new data, performs the apprpriate trannsformations, and loads the data into the existing tables. We will accomplish this goal in the follwing four steps:

### 1. Write an ETL Function to Read Three Data Files
    
For this task we created a function to read all 3 of the files containing the data we are working wwith (Kaggle Metadata, MovieLens, and Wikipedia). Then converted       them into individuals dataframes.
    
    
![image](https://user-images.githubusercontent.com/108442512/189793936-38bee00f-ec9c-4b92-a1eb-e08df2d903c1.png)
![image](https://user-images.githubusercontent.com/108442512/189794014-1b793c7f-bd86-4f37-98a4-b7f2b826e44a.png)
![image](https://user-images.githubusercontent.com/108442512/189794063-37f3aec2-04d9-40be-8b85-675d4b24cedf.png)

### 2. Extract and Transform the Wikipedia Data
Now that we have our dataframes made we need to clean the Wikipedia data to remove any columns, elemintae duplicates, and drop null values.
    
    
![image](https://user-images.githubusercontent.com/108442512/189794347-f7497b03-5bb3-4754-854a-f05744504d6c.png)
![image](https://user-images.githubusercontent.com/108442512/189794405-b591b4ac-61b3-4268-807b-9c53308ffa2f.png)
    
### 3. Extract and Transform the Kaggle Data
We repeat the process here for the Kaggle Metadata as we did for the Wikipedia data then merge the two dataframes together.
    
    
![image](https://user-images.githubusercontent.com/108442512/189794519-90b2a2d7-a180-44cb-ad77-f777335be705.png)
![image](https://user-images.githubusercontent.com/108442512/189794555-ff3aefde-6533-4078-a607-1b8854c8b194.png)

### 4. Create the Movie Database
Lastly we needed to add the dataframes to our SQL database
    
