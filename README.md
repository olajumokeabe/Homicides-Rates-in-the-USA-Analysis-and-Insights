# About Dataset

Crime has been recorded in the United States since its founding and has fluctuated significantly over time.
 
According to a 2013 report by the United Nations Office on Drugs and Crime (UNODC), between 2005 and 2012, the average homicide rate in the U.S. was 4.9 per 100,000 inhabitants compared to the average rate globally, which was 6.2. However, the U.S. had much higher murder rates compared to four other selected developed countries, which all had average homicide rates of 0.8 per 100,000. - Wikipedia

The Washington Post collected data on more than 52,000 criminal homicides over the past decade in 50 of the largest American cities. Most departments provided a decade of data, ending in 2017. New York City, however, provided only two years.

Read the story [here](https://www.washingtonpost.com/graphics/2018/investigations/where-murders-go-unsolved/)

The data included the location of the killing, whether an arrest was made and, in most cases, basic demographic information about each victim.

Reporters received data in many formats, including paper, and worked for months to clean and standardize it, comparing homicide counts and aggregate closure rates with FBI data to ensure the records were as accurate as possible.

In some cases, departments provided only partial information about the homicides, so reporters consulted public records, including death certificates, court records and medical examiner reports, to fill in the gaps. The data is more specific than the federal homicide data gathered annually by the FBI from police agencies nationwide.

# Data Collection

The dataset was downloaded on Kaggle [here](https://www.kaggle.com/datasets/joebeachcapital/homicides)

## Analysis and insights are needed on the following:

Q1. Which state has the highest number of case?

Q2. What is the distribution of disposition status?

Q3. Which race are the highest victims of murder?

Q4. Are this murders gender based?

Q5. What age range or age group has the highest number of homicide victims?

Q6. Which year has the highest reported case?

Q7. Produce a map of the states in the dataset.

# Data Cleaning

Some rows had to be dropped due to missing data, and information on some victims was marked as unknown to avoid assumptions. This highlights potential data quality issues that need addressing.

The names of all states was written completely in full for easy identification, who would have known VA is Virginia and not Vancouver 😁, I did this by creating a dictionary of the names and replacing on the dataset

Since the names of the victims are irrelevant to this analysis, i simply dropped the columns

I also converted the reported date data type from object to datetime and also converted the age column to numeric. This step was done only so that I could get insights into the age group.

# EDA 

**Q1. Which state has the highest number of case?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/ed4da9ba-6ddb-4835-bea8-8f8b46a0a6e0)

**Q2. What is the distribution of disposition status?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/b9ab02ba-a0ae-41e8-b2ef-18eb6ebe1dd0)

**Q3. Which race are the highest victims of murder?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/d2bfa72e-9397-44aa-b6f4-8ff3911d7998)

**Q4. Are this murders gender based?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/3a038286-899b-46e5-b7cd-5ad147af03bb)

**Q5. What age range or age group has the highest number of homicide victims?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/c88e7f78-562a-4904-a88e-037b2687b956)

**Q6. Which year has the highest reported case?**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/5d219284-c3fb-4125-8fe6-93159d6bef6e)

**Q7. Produce a map of the states in the dataset.**

![image](https://github.com/olajumokeabe/Homicides-Rates-in-the-USA-Analysis-and-Insights/assets/125363157/72838a19-b96a-488a-befb-794f6a58a5fc)

# Insights and Conclusion

California has the highest number of homicide cases, exceeding 6000, followed by Texas and Illinois. In contrast, Colorado has fewer than 1000 cases.

While many cases have been closed with arrests made, there is an almost equal number of cases that remain open with no arrests.

Alarmingly, a significant number of homicide victims are of Black descent, totaling nearly 35,000. This highlights a concerning trend in victim demographics.

Homicide rates are higher among males compared to females, suggesting that men are more vulnerable to such incidents.

Victims tend to be young to middle-aged, with a noticeable focus on people in their 30s, this shows that age matters in the this cases.

The years 2016, 2015, and 2017 recorded the highest number of reports, indicating consistent reporting of homicides over the years.

# Recommendations

1. Address data quality issues to ensure more accurate and comprehensive reporting. This includes reducing missing information and standardizing data collection processes.

2.Given the significant number of Black victims, consider targeted interventions and community engagement initiatives in areas with higher homicide rates to address root causes and reduce disparities.

3. Develop outreach programs and support systems for young adults, especially those in their 30s, to help reduce their vulnerability to homicides.

4. Continue efforts to close open cases and make arrests. Implement proactive policing strategies to deter potential offenders.

5. Given the fluctuation in reporting over the years, establish yearly monitoring and analysis to identify trends and allocate resources effectively.

6. Collaborate with communities and local organizations to build trust and encourage reporting, which can help in solving cases more efficiently.

7. Provide training to law enforcement agencies to address any biases and ensure fair treatment in homicide cases.

8. Strengthen victim support services to assist families affected by homicides and provide them with the necessary resources and counseling.

*These recommendations aim to improve data reliability, address disparities, enhance community safety, and ensure a more effective response to homicide cases.*
