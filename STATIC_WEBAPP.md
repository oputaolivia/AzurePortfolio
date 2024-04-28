# Hosting a Static Website on Azure Blob Storage
---

# Table of Contents
1. [Set up a Static Website](#set-up-a-static-website)
2. [Create an Azure Storage Account](#create-an-azure-storage-account)
3. [Configure Static Website Hosting](#configure-static-website-hosting)

## Set up a Static Website
Using HTML and CSS I created a portfolio, with images. After creating the portfolio i ran it locally to test it.

##  Create an Azure Storage Account
1. Login to the [Azure Portal](https://portal.azure.com/).
2. In the search bar, search for __Storage Account__ and select it.

3. Click on __+ Create__ or __Create Storage Account__

4. On the __Basics__ tab, Select an Azure subscription and Resource Group in the project details section. 

5. In the Instance details section input a storage account name, select region performance and redundancy.

6. Leaving the Advanced, Networking, Data Protection, Encryption and Tags tab as default.
7. Click on the __Review__ button and await validation.

8. Once validation is passed, click on __Create__.

## Configure Static Website Hosting
In order to deploy a static website on Azure Blob Storage, we need to enable static websites. Enabling it allows you to host static contents.
1. Once the storage account has been created, go to the storage account.

2. In the __Data Management__ section, Select the __Static Website__ blade and click Enable. Key in the index page name for the static webpage.
> For me it was index.html

3. Save changes and take note or copy the primary endpoint.

## Upload Web Application to Azure Blob Storage
Next step is to upload the static contents to Azure Blob storage.
1. In the __Container__ blade, click on the __$web__ container.
> The $web container is created once static website is enabled.

2. Click on __Upload__

3. Upload all the static content for the web application (HTML, CSS and Image files).

4. Once the files are uploaded, paste the primary endpoint that was copied initially to a web browser and viola the static web application is up.
