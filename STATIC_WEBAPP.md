# Hosting a Static Website on Azure Blob Storage
---

# Table of Contents
1. [Set up a Static Website](#set-up-a-static-website)
2. [Create an Azure Storage Account](#create-an-azure-storage-account)
3. [Configure Static Website Hosting](#configure-static-website-hosting)

## Set up a Static Website
Using HTML and CSS I created a portfolio, with images. After creating the portfolio i ran it locally to test it.
![0](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/ac176d15-af70-456b-8a29-5323cd120e1d)

##  Create an Azure Storage Account
1. Login to the [Azure Portal](https://portal.azure.com/).
2. In the search bar, search for __Storage Account__ and select it.
![1](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/85159278-1938-457e-bfba-518219c15717)

3. Click on __+ Create__ or __Create Storage Account__
![2](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/b0c58e3a-82be-4eea-b2a7-b12ca86c47c9)

4. On the __Basics__ tab, Select an Azure subscription and Resource Group in the project details section. 
![3](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/cb44bc79-1a5c-4f24-a260-354c0b40486e)

5. In the Instance details section input a storage account name, select region performance and redundancy.
![4](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/6e44e658-2377-4260-be27-e2303f2aae2d)

6. Leaving the Advanced, Networking, Data Protection, Encryption and Tags tab as default.
7. Click on the __Review__ button and await validation.

8. Once validation is passed, click on __Create__.
![5](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/96c56ab1-44aa-461c-9ba5-4d381cf5ad62)

## Configure Static Website Hosting
In order to deploy a static website on Azure Blob Storage, we need to enable static websites. Enabling it allows you to host static contents.
1. Once the storage account has been created, go to the storage account.
![6](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/b657602c-7df1-48d7-9c94-5f2f20eef7af)

2. In the __Data Management__ section, Select the __Static Website__ blade and click Enable. Key in the index page name for the static webpage.
> For me it was index.html
![1](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/9b2b95d8-09c6-4f4f-9fa6-eac0ee7e2565)

3. Save changes and take note or copy the primary endpoint.
![2](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/16189840-8312-42fd-8797-8ab7ffbdfdf5)

## Upload Web Application to Azure Blob Storage
Next step is to upload the static contents to Azure Blob storage.
1. In the __Container__ blade, click on the __$web__ container.
> The $web container is created once static website is enabled.
![1](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/4f1f2e95-cf37-48ad-b0e7-cd5f6f87ed5e)

2. Click on __Upload__
![2](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/d12a7189-4c44-4804-a062-ad982f15ae25)

3. Upload all the static content for the web application (HTML, CSS and Image files).
![3](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/e8605158-58dd-4606-b807-6ed6e7ef7220)

4. Once the files are uploaded, paste the primary endpoint that was copied initially to a web browser and viola the static web application is up.
![4](https://github.com/oputaolivia/AzurePortfolio/assets/72948572/3cb946c8-22a0-47e6-8977-a1b01753ad26)
