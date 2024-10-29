# Lab 3 - Explore Google Cloud Storage | Buckets

University: [ITMO University](https://itmo.ru)

Faculty: [FTMI](https://ftmi.itmo.ru)

Course: Cloud platforms as the basis of technology entrepreneurship

Year: 2024-2025

Group: U4225

Author: Sukhankulyev Davut Tumenovich

Lab: Lab3

Date of create: 28.10.2024

Date of finished: 29.10.2024

## Task

### Objective
Become familiar with the basic concepts and principles of cloud storage, explore various data storage models (block, file, object storage), and get to know the main services and functionalities provided by cloud storage solutions.

### Procedure

1. Select an existing project where you have the appropriate permissions.

2. Create a Cloud Storage bucket.

3. Upload 3-4 images to the Cloud Storage bucket.

4. Create a folder with any name and move the files into it within the bucket.

5. Set up public access for your files in the privacy settings.

6. Generate a link for your files through the file's context menu.

7. Delete all created services after use and write a report using screenshots.

## Answer

1. I entered our course project on Google Cloud Console named `cloud-platforms-as-the-basis`
links

2. Then I created Cloud Storage bucket:
    1. First set the name
    ![Bucket: set name](../media/lab3/2_1_BucketName.png)

    2. Then set the region
    ![Bucket: set region](../media/lab3/2_2_BucketRegion.png)

    3. Create the bucket
    ![Bucket: created bucket](../media/lab3/2_3_BucketCreated.png)

    4. Also set permissions for the account
    ![Bucket: Permission](../media/lab3/2_4_BucketPermissionsGranted.png)

3. Then I uploaded 4 images into my bucket
![Images uploaded](../media/lab3/3_1_BucketImagesUploaded.png)

4. After that I created folder in the same bucket and moved my images there. I used Transfer Files Job:
    1. Create a transfer job:
    ![Job: Configure source and desitnation types](../media/lab3/4_1_JobTransferFiles.png) 
    ![Job: Choose source](../media/lab3/4_2_JobTransferFiles.png) 
    ![Job: Choose destination](../media/lab3/4_3_JobTransferFiles.png) 
    ![Job: Choose job start time](../media/lab3/4_4_JobTransferFiles.png) 
    ![Job: set description and other options](../media/lab3/4_5_JobTransferFiles.png) 
    2. Then I ensured that my job was running at that time:
    ![Job: started](../media/lab3/4_6_JobTransferFilesCreated.png) 
    3. At last my job finished. Also I could assert that my files were copied but not moved:
    ![Files: copied](../media/lab3/4_7_JobTransferFilesFinished.png) 
    ![Files: ensure first files are safe](../media/lab3/4_8_JobTransferFilesFinished.png)

5. Then I granted to `allUsers` permission to view files. I set them the role `Storage viewer` on my folder:
![Permission: public role1](../media/lab3/5_1_AccessGrant.png) 
![Permission: public role2](../media/lab3/5_2_AccessGrant.png) 
![Permission: public role3](../media/lab3/5_3_AccessGrant.png)

6. Generated links for my files:
    - [SpidermanInMoscow.jpg](https://storage.googleapis.com/davut_lab3/SecondIterationImages/StableDiffusion_SpidermanMoscow.jpg)
    - [SovietBearOnMoon.jpg](https://storage.googleapis.com/davut_lab3/SecondIterationImages/StableDiffusion_SovietBearMishaMoon.jpg)
    - [OMG.jpg](https://storage.googleapis.com/davut_lab3/SecondIterationImages/StableDiffusion_OMG.jpg)
    - [BitcoinTreasure.jpg](https://storage.googleapis.com/davut_lab3/SecondIterationImages/StableDiffusion_BitcoinTreasure.jpg)
    ![Public: links](../media/lab3/6_1_GeneratePublicURL.png)

7. Removed my own bucket from the Console

## Conclusion
In this lab, I learned the basics of Google Cloud Storage by by creatin my own bucket. I learned to:
- Create and configure storage buckets; 
- Manage file uploads;
- Organize files within folders. 
I also practiced:
- Setting up public access to files and generating public URLs;
- Making the files accessible to all users.

This exercise improved my understanding of cloud storage permissions and file accessibility. Finally, I cleaned up by deleting all resources, reinforcing the importance of managing cloud resources responsibly.