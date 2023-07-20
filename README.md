# Road Noise Excel Daschboard

![Road_noise_report_Poland_2018-2021](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/abc715d5-4613-4e7d-b42c-341a7ca98e51)

# Road Noise Project Background Description

### As a data enthusiast, I have undertaken a project aimed at analyzing road noise data. 

The dataset was sourced from the official data repository at https://dane.gov.pl/pl/dataset/1404. 
It comprises four separate CSV files, each corresponding to a specific year from 2018 to 2021.
To begin the data preprocessing, I loaded all the files into the Power Query Editor. In the subsequent step, I combined all four queries through appending. However, during this process, an error was encountered, as the 2021 file introduced additional columns that did not align with the other years.

 ![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/be75bd1e-6992-41fe-978e-bbf2e1b527d6)

 ![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/388d3e3e-261b-45fc-858e-bdd8849d8afe)
 

To address this issue, a simple solution was implemented by merging columns that shared the same data types. Following this, the data required fast cleaning, and I executed the following steps:
1.	Reordering columns: I organized the columns to have a consistent and coherent structure.
2.	Renaming columns: Meaningful names were assigned to the columns for clarity, such as "Województwo" (Voivodeship), "Miejscowość" (City), and "Kod punktu pomiarowego" (Measurement Point Code).
3.	Filtering out specific rows: Certain measure point names that represented partial days were excluded to ensure accurate data representation.
4.	Part of day cleaning: A new column was added to categorize the measurements based on the time of day.
5.	Data type transformation: Dates and numeric values were converted to appropriate data types.
After completing the data cleaning and transformation, the dataset was loaded into the data model. 
As part of the project requirements, an acceptable noise level threshold was defined as 70 dB, labeled as 'Grancia dB'. I developed a measure to count the number of noise level overruns above this threshold.

![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/86886732-f1db-4787-bd12-5f85cdc577be)
 
With the above measure in place, I calculated the percentage of noise level overruns to gain insights into the severity of the noise pollution.

![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/e565f440-61ac-42b3-9662-3f052208001d)
 
For further analysis, I prepared several pivot tables, including KPIs (Key Performance Indicators) such as average noise level, maximum noise level, the number of measuring places, the percentage of overruns, and the total number of measurements.

![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/9e5f3616-79e7-43c8-9e8d-960bd8da1509)
 
Additionally, I identified and highlighted the five loudest voivodeships and the ten loudest cities based on the noise levels recorded.

![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/e42e149a-5d8a-4ef0-965b-5e1b5eabce80) ![image](https://github.com/zdziebkowski/Road-noise-report/assets/126050762/cf28bebf-b783-40f5-a9b1-64e7eac7f449)

To enhance the presentation and improve data visibility, I applied formatting and conditional formatting to the pivot tables.
The final phase of the project involved creating a dashboard that incorporates two pivot charts illustrating noise levels by year and average noise levels by year and time of day. The dashboard also includes the previously mentioned KPIs and pivot tables.
To facilitate detailed insights and enable user interactivity, I incorporated slicers allowing data filtering by voivodeship and city. This feature empowers stakeholders to customize their view and extract specific information as needed.
