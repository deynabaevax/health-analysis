<p float="left">
  <img width="60px" src="https://apkresult.com/Logos/apple-health-appresult.jpg">
  <img width="400px" src="https://9to5mac.com/wp-content/uploads/sites/6/2019/07/prioritize-apple-health-sources-iphone-walkthrough.png">
  <img width="200px" src="https://support.apple.com/content/dam/edam/applecare/images/en_US/psp_content/content-block-md-watch-set-goals_2x.png">
</p>

 # Analyzing Personal Health Data with Python
 
# Introduction
Our phones are great mini-trackers that can be used for analyzing insights in our health. If you are an Apple user, you probably know about Apple Health. It is an iOS feature that monitors and organizes health-related data. It consolidates data gathered by the Apple ecosystem and third-party devices and apps. Depending on your specific setup, it may offer valuable insights on your physical activity, body measurements, sleep habits, heart rate, hearing, nutrition, blood glucose or even menstrual cycle, to give a few examples. While some metrics are simple such as the number of steps, others are more elaborated as the ratios of double-support time or asymmetry while we walk. As I am using an Apple watch, I would like to create something with Python, which will provide me with better understanding of the data I am providing my watch.

## The Data

I will be using the exported data from my Apple Health App.

## Steps Taken

- Download the Data
- Exploring the Data
- Analyzing the Data

__1. Downloading the dataset First, I need to download the dataset. It requires a few manual steps:__
   - Open the Health app on your phone.
   - Touch the profile picture on the top-right corner.
   - Press on "Export All Health Data" at the bottom of the screen.
   - Download the created .zip file. I chose to save it on iCloud and then manually download it on my laptop.

__2. Set-up Data Version Control (DVC)__

    As the downloaded health data file is too big to be uploaded on GitHub, I quickly set-up DVC to access the data from there.

__3. Processing the XML file__

    From the two files inside the archive, the one named export.xml has the data I need.

## Data Analysis

> Firstly, I started by analyzing the steps that I have made throughout the years. I will attach few figures, which will show overview. The first one on the left shows the top 5 results throughout the years. The second figure in the middle represents the top 10 results for most active months. Finally, the figure on the right represents the steps in overview of ___August 2022___.

![creationdate1](https://user-images.githubusercontent.com/64732465/197808146-c9d8793a-f99d-41f7-9f18-6fc2fd37dea5.png)
![top10months](https://user-images.githubusercontent.com/64732465/197808447-66292198-70b2-4a9a-95ca-e7c540a75c10.png)
![overview of 2022 august](https://user-images.githubusercontent.com/64732465/197808841-16a3c9d2-b665-424d-b7bf-96b6cf8681f4.png)

Secondly, I took a look at the distribution of the walking activity during the week. 

![weekday](https://user-images.githubusercontent.com/64732465/197809531-4e84d9e7-fb46-42f8-a55d-cfee0f614131.png)

Looks like I am pretty active in the beginning and the end of the week. 

> Besides that, I created aa plot, which represents my cycling activity throughout the years. Recently, I started cycling more, so I wanted to take a look at that.

![index](https://user-images.githubusercontent.com/64732465/197810171-07b745df-329e-4011-b2a0-f863a92053fe.png)

As I thought, my cycling activity has increased rapidly. 🙂
