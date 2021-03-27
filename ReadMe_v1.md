## Overview

This guide describes the concept of Data Explorer, how to get access to Data Explorer catalog, and further use it to discover data by classified categories. 

In the later sections, it provides an introduction to Jupyter Notebook and steps to use a Notebook in JupyterLab; followed by helpful links to information about using Notebooks, and process to raise a support request.

----

[toc]

-----

## 1. What is Data Explorer?

Data Explorer is a robust and highly intuitive data exploration platform for data science applications. It helps users visualize, and analyze diverse data from some interesting classified datasets and associated notebook resources. 

### 1.1 Unlocking the Benefits

- This Data Explorer offers the advantage for the end users to discover data using its featured cataloging capabilities, and to explore machine learning algorithms/code with Notebook.
- It offers an interesting collection of data scientist textbooks and iPython notebooks that helps users to explore the datasets, learn about different algorithms, and process the data using Python notebooks.
- Users can make use of Jupyter Notebooks which already contain the code relevant to certain data science capabilities. 
-  It makes easy for the data scientists to interact with their data using catalog functionalities combined with the power of JupyterLab to perform complex operations on target data streams.

## 2. Run Data Explorer on AWS

To get started, follow the below steps.

**Step 1:** On Data Explorer Product page, click on `Continue to Subscribe` button.

![image-20210326164828396](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run1.png)



**Step 2**: Click on `Accept Terms` (visible in yellow button) on the Subscription page.

![image-20210326164947801](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run2.png)



**Step 3**: You will view a Thank you message on the top of the page. 

![image-20210326165252959](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run3.png)

The page also displays the processing status of your Subscription Request.

![image-20210326165305803](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run3a.png)



**Step 4**: When your subscription request is processed successfully, click  on`Continue to Configuration`.

![image-20210326165626177](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run4.png)



**Step 5**: On *Configure* page, confirm your selection of *Delivery Method*, *Software Version*, *Region*. You can also choose to proceed with default values, and click on `Continue to Launch` button.

![image-20210326165841756](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run5.png)



**Step 6**: On *Launch* page, select `Launch through EC2`  from **Choose Action** drop-down list, and then click on `Launch`.

![image-20210326165909349](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run6.png)

**Step 7**: Choose the `Instance Type`, and click on `Configure Security Group` in the given Menu bar.

![img](file:///C:/Users/MUGDHA~1/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)
 ![img](file:///C:/Users/MUGDHA~1/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)



**Step 8**: Verify that the below ports are added.

![image-20210326170429073](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run8.png)



**Step 9**: Click on `Review and Launch` button.

![image-20210326170533647](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run9.png)

**Step 10**: Once you've reviewed all the settings, click on `Launch` button.

![image-20210326170608287](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run10.png)

**Step 11**: Select the option `Proceed without a key pair`, check the acknowledgement statement box, and then click on `Launch Instances` button to proceed.

![image-20210326170921176](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run11.png) 

This redirects you to Launch Status page.

**Step 12**: Click on the <Instance ID> highlighted in blue. (Here, it is i-0ce08ec9ef7d55442).

![image-20210326171312477](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run12.png)



**Step 13**: On `Instances` page, select the instance (with same Instance ID) to view the details.

![image-20210326171605826](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run13.png)

Wait for some time (around 3 minutes) until the instance gets started. 



**Step 14**: Click on `open address` link provided under **Public IPv4 DNS** section.

![image-20210326171647058](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\run14.png)

If the instance has started completely, you would see **Data Explorer Catalog** page.

> **That's it!** Now you are ready to get hands-on with Data Explorer.

-----

The upcoming sections talk about the following topics on Data Explorer.

- Components of Data Explorer
- Understanding Data Explorer Catalog
- Deploying a Dataset
- Exploring Data Assets using Notebook in JupyterLab



***Let's get started!***



## 3. Components of Data Explorer 

Data Explorer is composed of the two major components that users can leverage to perform data science related tasks. These classic components are:

- Data Explorer Catalog
- JupyterLab

The following diagram shows a snapshot of Data Explorer UI.

![image-20210325171654260](C:\Users\MugdhaThareja\Desktop\image-20210325171654260.jpg)Catalog

### 3.1 Data Explorer Catalog

As illustrated in the diagram above in section 1.1, this menu is available on the top-left corner of the UI. 

As soon as you click on *Data Explorer Catalog* tab, it will open an interface below containing two columns - one containing catalog categories arranged in vertical, and other containing a grid of dataset and notebook tiles.

#### 3.1.1 Catalog Categories

This column contains four categories - Show, Types, Tags, and Categories. A user can sort the grid view by making choices from the given selection list boxes.

##### 3.1.1 Show

This allows the user to view the grid content based on the selection of radio button - All or Deployed.

- If a user selects `All`, it will show the entire list of available datasets and notebooks.
- If a user selects `Deployed`, it will show only the installed versions of datasets and notebooks.



**Show All**

![image-20210325184628384](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\showall.png)



**Show Deployed**

![image-20210325184530870](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\shoedep.png)



##### 3.1.2 Types

Under this category, a user can make his choice to view Dataset or Notebook or both in the grid column.

**Dataset Type**

![image-20210325185127878](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\typed.png)

This produces the list of available dataset tiles in the grid column.

**Notebook Type**

![image-20210325185316793](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\typen.png)

This produces the list of available Notebook tiles in the grid column.

> Selecting both the list boxes will display a collection of dataset and notebook tiles.

##### 3.1.3 Tags

Selecting this category will display the grid of dataset tiles containing CSV files. CSV files are easy to work with and are characterized by their tabular format.

##### 3.1.4 Categories

This contains the datasets categories upon which Notebooks have been built. A user can choose to view particular tile(s), making choices from the given genres of categories.

### 3.2 Browsing through the Data Catalog

Now, you have learned about various catalog categories and resulting grid view upon user's selection. This section details about browsing through the Data Explorer Catalog.

**Example**

Suppose the user clicks on `All` and selects `Dataset` type. This will display the below content on Catalog UI.

![image-20210325191537429](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\Browsedc.png)

Now, clicking on one of the dataset tiles (say, Flower Classification Data), the user will view a small window opening to the right of the grid. See below.

![Dataset view](C:\Users\MugdhaThareja\Desktop\Dataset_view.PNG)

This window will display the name of selected dataset on the top, and following information about this dataset.

- Metadata (Install Time, Type, Last Updated, Categories, By)
- Brief Description

## 4. JupyterLab

### 4.1 Getting Started

Popularly known as Jupyter’s Next-Generation Notebook Interface, JupyterLab brings many new features to users. It is an open-source, web-based interactive development environment for Jupyter notebooks, code, and data. The peculiar features of JupyterLab are:

- *Flexible* - Users can configure and arrange the UI to support a broad range of workflows in data science, scientific computing, and machine learning. 
- *Modular and Extensible*  - Users can write plugins that add new components and can integrate with existing ones.
- *Unified View Model* - JupyterLab provides an integrated model to handle different data formats (images, CSV, PDF, JSON, Markdown, etc.). It can display kernel output by interpreting these formats.
- *Rich User Experience* - Working with Jupyter Notebooks offers users with the advantage of building rich web applications, statistical modeling, numerical simulation, plotting and much more. 

### 4.2 JupyterLab Credentials

On the top-right corner of the Explorer UI, you find *JupyterLab Credentials* with a key icon. Once clicked, this will open the credential details - username and password.

These credentials can be copied for use by the end users to sign in to JupyterLab console.

![JupyterLab Login](C:\Users\MugdhaThareja\Desktop\JupyterLab Credentials.PNG)

> Clicking on the eye icon on the right side of password, a user can view the actual password.

### 4.3 Directories and File Structure

After successful login, the user is redirected to JupyterLab user interface.  The following diagram depicts the snapshot of JupyterLab UI.

![image-20210326140754070](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\dirstr.png)

Here, you can see the Folder view, and the Launcher view. 

- Folder view: It contains a structured list of files and folders sorted in alphabetical order. Each folder contains two sub-folders : dataset, and notebook.

- Launcher view: This shows the content of Notebook to be explored by the end user. To launch the content of selected Notebook, it is required that the corresponding dataset of that Notebook must be pre-installed.

  

### 4.4 Deploy a Dataset

To install the dataset,

1. Go to Data Explorer Catalog.

2. Select type as `Dataset`, and click on the desired dataset tile.

   ![image-20210326142359614](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\depds1.png)

3. Click on the icon on the bottom right of the dataset tile. This will open the selected dataset in new tab displaying information about the chosen dataset.

   ![image-20210326142426189](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\depds2.png)

4. Click on `Deploy Dataset` to install the chosen dataset.

5. On successful installation, the page will display installation details with Dataset path that a user can reference while exploring Jupyter Notebooks in the JupyterLab console.

![image-20210326142745272](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\depds3.png)

A folder gets added to the JupyterLab directory structure.

![image-20210326143019357](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\depds4.png)

> Note: Dataset folder and Notebook folder resides in the same directory in JupyterLab space.

## 5. Jupyter Notebook

Jupyter notebooks are rich documents that combine live runnable code with equations (LaTeX),  images, narrative text (Markdown), interactive visualizations and other file formats. The file extension of a Jupyter notebook  is `.ipynb`.

> In Jupyter Lab, the UI for a Jupyter Notebook closely follows that of a classic Jupyter Notebook.

### 5.1 Exploring Jupyter Notebook

1. To view the Notebook files in JupyterLab, click on `JupyterLab` tab. This will redirect you to login dashboard.
2. Enter the JupyterLab Credentials and click on Sign In. 

> Note: If you are already logged in to JupyterLab, ignore the above steps.

![image-20210326143325919](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\Jupnb.png)



3. Click on the target folder you want to access. (say, Flower_classification)
4. This will open the sub-folders of the chosen dataset folder.
5. Cliick `notebooks` folder, and then the corresponding `.ipynb` file. This will display the content in the Launcher view.

![image-20210326143551019](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\jupexpnb.png)

Now you can explore, experiment and visualize the data according to your requirements.

### 5.2 Create and Use a Notebook in JupyterLab

To learn about creating and using a notebook, refer `My first notebook` file. 

You can navigate to the file by following the below steps.

1. Go to `/home/jupyter-user/`.
2. Select the `My_first_notebook_1609928816737` folder from the list.
3. Double click on `My First Notebook.ipynb` file.

This opens the corresponding file in Launcher view as follows.

![image-20210326145144715](C:\Users\MugdhaThareja\Desktop\Operator Playground\DS_Data_Explorer\Images\usenb.png)

The file contains a step-by-step guide on how to create a new a Notebook and use it in JupyterLab.



## 6. Useful Links

A collection of links to information that will help you find what you are looking for:

- [About Python](https://docs.python.org/)
- [Python Standard Libraries](https://docs.python.org/3/library/)
- [JupyterLab Reference](https://jupyterlab.readthedocs.io/en/stable/)
- [More About Jupyter Notebook](https://jupyterlab.readthedocs.io/en/stable/user/notebook.html)



## 7. Help & Support

If you encounter any problems when setting up or using Data Explorer, please let us know - we're here to help you!

To report a bug, please open a [Github issue](https://github.com/edge-trial/Support/issues) and we will get back to you about your concern. 

> Make sure you set up a separate public Github account for this purpose.

Providing as much information as possible about your issue will help our Support Team to give you a more complete response in quick time.

*We also welcome suggestions for new feature or improvement as they will help make this project more useful for everyone.*
