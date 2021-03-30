## Overview

<p>This guide describes the concept of Data Explorer, how to get access to Data Explorer catalog, and further use it to discover data by classified categories.
<p>In the later sections, you will gain insights into essentials of Jupyter Notebook including steps to create and use a Notebook in JupyterLab and some helpful links to information about using JupyterLab and Jupyter Notebook interface. 
<p>Also, learn how to raise a support request for any issue related to using the Data Explorer.

----
#### Contents

- [Overview](#overview)
- [1. Introduction to Data Explorer](#1-introduction-to-data-explorer)
  * [1.1 Unlocking the Benefits](#11-unlocking-the-benefits)
- [2. Running Data Explorer on AWS](#2-running-data-explorer-on-aws)
- [3. Components of Data Explorer](#3-components-of-data-explorer)
  * [3.1 Data Explorer Catalog](#31-data-explorer-catalog)
    + [3.1.1 Catalog Categories](#311-catalog-categories)
      - [Show](#show)
      - [Types](#types)
      - [Tags](#tags)
      - [Categories](#categories)
  * [3.2 Browsing through the Data Catalog](#32-browsing-through-the-data-catalog)
- [4. JupyterLab](#4-jupyterlab)
  * [4.1 Getting Started](#41-getting-started)
  * [4.2 JupyterLab Credentials](#42-jupyterlab-credentials)
  * [4.3 Directories and File Structure](#43-directories-and-file-structure)
  * [4.4 Deploy a Dataset](#44-deploy-a-dataset)
- [5. Jupyter Notebook](#5-jupyter-notebook)
  * [5.1 Exploring Jupyter Notebook](#51-exploring-jupyter-notebook)
  * [5.2 Create and Use a Notebook in JupyterLab](#52-create-and-use-a-notebook-in-jupyterlab)
  * [5.3 Use Dataset in Sample Notebook](#53-use-dataset-in-sample-notebook)
    + [Installing a Dataset](#installing-a-dataset)
    + [Installing a Notebook](#installing-a-notebook)
    + [Using the Dataset in Notebook](#using-the-dataset-in-notebook)
  * [5.4 Run a Notebook File](#54-run-a-notebook-file)
- [6. Getting Help](#6-getting-help)
- [7. Further Reading](#7-further-reading)
-----

## 1. Introduction to Data Explorer
<p>Data Explorer is a robust and highly intuitive data exploration platform for data science applications.
<p>It helps users visualize, and analyze diverse data from some interesting classified datasets and associated notebook resources. 

### 1.1 Unlocking the Benefits
- This Data Explorer offers the advantage for the end users to discover data using its featured cataloging capabilities, and to explore machine learning algorithms/code with Notebook.
- It offers an interesting collection of data scientist textbooks and iPython notebooks that helps users to explore the datasets, learn about different algorithms, and process the data using Python notebooks.
- Users can make use of Jupyter Notebooks which already contain the code relevant to certain data science capabilities. 
-  It makes easy for the data scientists to interact with their data using catalog functionalities combined with the power of JupyterLab to perform complex operations on target data streams.

-----

## 2. Running Data Explorer on AWS

To get started, follow the below steps.

**Step 1:** On Data Explorer Product page, click on `Continue to Subscribe` button.

![Run_on_AWS](/_images/run1.png)


**Step 2**: Click on `Accept Terms` (visible in yellow button) on the Subscription page.

![Run_on_AWS](/_images/run2.png)


**Step 3**: You will view a Thank you message on the top of the page. 

![Run_on_AWS](/_images/run3.png)

The page also displays the processing status of your Subscription Request.

![Run_on_AWS](/_images/run3a.png)


**Step 4**: When your subscription request is processed successfully, click  on`Continue to Configuration`.

![Run_on_AWS](/_images/run4.png)


**Step 5**: On *Configure* page, confirm your selection of *Delivery Method*, *Software Version*, *Region*. You can also choose to proceed with default values, and click on `Continue to Launch` button.

![Run_on_AWS](/_images/run5.png)


**Step 6**: On *Launch* page, select `Launch through EC2`  from **Choose Action** drop-down list, and then click on `Launch`.

![Run_on_AWS](/_images/run6.png)


**Step 7**: Choose the `Instance Type`, and click on `Configure Security Group` in the given Menu bar.

![Run_on_AWS](/_images/run7a.png)
![Run_on_AWS](/_images/run7b.png)


**Step 8**: Verify that the below ports are added.

![Run_on_AWS](/_images/run8.png)


**Step 9**: Click on `Review and Launch` button.

![Run_on_AWS](/_images/run9.png)


**Step 10**: Once you've reviewed all the settings, click on `Launch` button.

![Run_on_AWS](/_images/run10.png)


**Step 11**: Select the option `Proceed without a key pair`, check the acknowledgement statement box, and then click on `Launch Instances` button to proceed.

![Run_on_AWS](/_images/run11.png)

This redirects you to Launch Status page.


**Step 12**: Click on the `Instance ID` highlighted in blue. (Here, it is i-0ce08ec9ef7d55442).

![Run_on_AWS](/_images/run12.png)


**Step 13**: On `Instances` page, select the instance (with same Instance ID) to view the details.

![Run_on_AWS](/_images/run13.png)

Wait for some time (around 3 minutes) until the instance gets started. 


**Step 14**: Click on `open address` link provided under **Public IPv4 DNS** section.

![Run_on_AWS](/_images/run14.png)

If the instance has started completely, you would see **Data Explorer Catalog** page.

> **That's it!** Now you are ready to get hands-on with Data Explorer Interface.

----
The upcoming sections talk about the following topics on Data Explorer.
- [Components of Data Explorer](#3-components-of-data-explorer)
- [Understanding Data Explorer Catalog](#31-data-explorer-catalog)
- [Deploying a Dataset](#44-deploy-a-dataset)
- [Exploring Data Assets using Notebook in JupyterLab](#51-exploring-jupyter-notebook)

-------
## 3. Components of Data Explorer 

Data Explorer is composed of the two major components that users can leverage to perform data science related tasks. These classic components are:

- Data Explorer Catalog
- JupyterLab

The following diagram shows a snapshot of Data Explorer UI.

![Data Explorer UI](/_images/desnap.png)

- In addition, you find a `FAQ & Support` tab which is provided to assist users in reaching out for troubleshooting support. 
- On the right end, it shows a tab `JupyterLab Credentials` which will be used to sign in to JupyterLab Console.

### 3.1 Data Explorer Catalog

As illustrated in the diagram above, this tab is available on the top-left corner of the UI. 

As soon as you click on *Data Explorer Catalog*, it will open an interface below containing two columns - catalog categories arranged in vertical, and a grid containing dataset and Notebook tiles.

#### 3.1.1 Catalog Categories

This column contains four categories - Show, Types, Tags, and Categories. A user can sort the grid view by making choices from the given selection list boxes.

##### Show

This allows the user to view the grid content based on the selection of radio button - All or Deployed.

- If a user selects `All`, it will show the entire list of available datasets and notebooks.
- If a user selects `Deployed`, it will show only the installed versions of datasets and notebooks.

> Show All

![CatalogUI](/_images/showall.png)

----
> Show Deployed

![CatalogUI](/_images/shoedep.png)


##### Types

Under this category, a user can make his choice to view Dataset or Notebook or both in the grid column.

> Dataset Type

![CatalogUI](/_images/typed.png)

This produces the list of available dataset tiles in the grid column.

> Notebook Type

![CatalogUI](/_images/typen.png)

This produces the list of available Notebook tiles in the grid column.

> Selecting both the list boxes will display a collection of both datasets and Notebooks.


##### Tags

Selecting this category will display the grid of dataset tiles containing `CSV` files. CSV files are easy to work with and are characterized by their tabular format.

##### Categories

This contains the datasets categories upon which Notebooks have been built. A user can choose to view particular tile(s), making choices from the given genres of categories.

![Catalog_Categories](/_images/catlist.png)


### 3.2 Browsing through the Data Catalog

Now, you have learned about various catalog categories and resulting grid view upon user's selection. This section details about browsing through the Data Explorer Catalog.

**Example**

Suppose the user clicks on `All` and selects `Dataset` type. This will display the below content on Catalog UI.

![Browse Catalog](/_images/Browsedc.png)

Now, clicking on one of the dataset tiles (say, Boston House Prediction Evaluation), the user will view a small window opening to the right of the grid. See below.

![Dataset view](/_images/depds1.png)

This window will display the name of selected dataset on the top, and following information about this dataset.

- Metadata (Install Time, Type, Last Updated, Categories, By)
- Brief description

<p>The same happens when you click on any Notebook tile, after selecting Types as 'Notebook' from the Category titles.
 
 ![Notebook View](/_images/expnb.png)


-------
## 4. JupyterLab

### 4.1 Getting Started

Popularly known as _Jupyter’s Next-Generation Notebook Interface_, JupyterLab brings many new features to users. It is an open-source, web-based interactive development environment for Jupyter notebooks, code, and data. The peculiar features of JupyterLab are:

- *Flexible* - Users can configure and arrange the UI to support a broad range of workflows in data science, scientific computing, and machine learning. 
- *Modular and Extensible*  - Users can write plugins that add new components and can integrate with existing ones.
- *Unified View Model* - JupyterLab provides an integrated model to handle different data formats (images, CSV, PDF, JSON, Markdown, etc.). It can display kernel output by interpreting these formats.
- *Rich User Experience* - Working with Jupyter Notebooks offers users with the advantage of building rich web applications, statistical modeling, numerical simulation, plotting and much more. 

> The Jupyter Notebook is quite useful not only for exploring and analyzing data, but also for learning a programming language such as Python.

### 4.2 JupyterLab Credentials

On the top-right corner of the Explorer UI, you find *JupyterLab Credentials* with a key icon. Once clicked, this will open the credential details - username and password.

These credentials can be copied for use by the end users to sign in to JupyterLab console.

![Jupyter Login](/_images/juplogin.png)

> Clicking on the eye icon on the right side of password, a user can view the actual password.

### 4.3 Directories and File Structure

After successful login, the user is redirected to JupyterLab user interface.  The following diagram depicts the snapshot of JupyterLab UI.

![Jupyter Login](/_images/dirstr.png)

Here, you can see the Folder view, and the Launcher view. 

- Folder view: It contains a structured list of files and folders sorted in alphabetical order. Each folder contains two sub-folders : dataset, and notebook.

- Launcher view: This shows the content of Notebook files to be explored by the end user. 

> Note: To successfully view or launch the selected Notebook, it is required that the corresponding dataset for that Notebook must be **pre-installed**.
  
### 4.4 Deploy a Dataset

To install the dataset,

1. Go to Data Explorer Catalog.

2. Select type as `Dataset`, and click on the desired dataset tile.

 ![Install Dataset](/_images/depds1.png)

3. Click on the icon on the bottom right of the dataset tile. This will open a new tab displaying more information about the the selected dataset.

 ![Install Dataset](/_images/depds2.png)

4. Click on `Deploy Dataset` to install the chosen dataset.

5. On successful installation, the page will display installation details with `Dataset path` that a user can reference while exploring Jupyter Notebooks in the JupyterLab.

![Install Dataset](/_images/depds3.png)

Consequently, a folder gets added to the JupyterLab directory.

![Install Dataset](/_images/depds4.png)

> Note: Dataset folder and Notebook folder resides in the same directory within JupyterLab.

------------
## 5. Jupyter Notebook

Jupyter notebooks are rich documents that combine live runnable code with equations (LaTeX),  images, narrative text (Markdown), interactive visualizations and other file formats. The file extension of a Jupyter notebook  is `.ipynb`.

> In JupyterLab, the UI for a Jupyter Notebook closely follows that of a classic Jupyter Notebook.

### 5.1 Exploring Jupyter Notebook

1. To view the Notebook files in JupyterLab, click on `JupyterLab` tab. This will redirect you to login dashboard.
2. Enter the JupyterLab Credentials [section 4.2](#42-jupyterlab-credentials) and click on `Sign in`. 

> Note: If you have already logged in to JupyterLab, ignore the above steps.

![Entering Jupyter Notebook Interface](/_images/Jupnb.png)

3. Click on the target folder you want to access. (say, Flower_classification)
4. This will open the sub-folders of the chosen dataset folder.
5. Cliick `notebooks` folder, and then the corresponding `.ipynb` file. This will display the content in the Launcher view.

![Entering Jupyter Notebook Interface](/_images/jupexpnb.png)

Now you can explore, experiment and visualize the data according to your requirements.

### 5.2 Create and Use a Notebook in JupyterLab

To learn about creating and using a notebook, refer `My first notebook` file. 

You can navigate to the file by following the below steps.

1. Go to `/home/jupyter-user/`.
2. Select the `My_first_notebook_1609928816737` folder from the list.
3. Double click on `My First Notebook.ipynb` file.

This opens the corresponding file in Launcher view as follows.

![Explore Jupyter Notebooks](/_images/usenb.png)

The file contains a step-by-step guide on how to create a new a Notebook and use it in JupyterLab.

---------------
### 5.3 Use Dataset in Sample Notebook
This section describes how a user can use the dataset(s) deployed from the [Data Explorer Catalog](#31-data-explorer-catalog) in a sample notebook.

Let's recall once.

#### Installing a Dataset

1. Navigate to **Data Explorer Catalog --> Types --> Dataset**.
2. Select any one dataset you want to install or deploy.
3. To install, click on the icon ![install icon](/_images/inst-icon.png) on the right-bottom of the dataset tile. This will open a new tab containing metadata, and brief description about the dataset.
4. Click on **Deploy Dataset**.
5. The dataset is successfully installed.

![install dataset](/_images/deply-ds.png)


#### Installing a Notebook

1. Navigate to **Data Explorer Catalog --> Types --> Notebook**.
2. Select any one Notebook you want to install or deploy.
3. To install, click on the icon ![install icon](/_images/inst-icon.png) on the right-bottom of the dataset tile. This will open a new tab containing metadata, and brief description about the Notebook.
> Note the Dataset information given in the metadata description.
4. Click on **Deploy Notebook**.
5. The Notebook is successfully installed.

![install dataset](/_images/deply-nb.png)

> Now, let's see how we can use the deployed dataset in a sample Notebook using JupyterLab.

#### Using the Dataset in Notebook
- To consume a dataset in sample Notebook, it is important to understand how the notebook interprets which dataset to use and where that dataset is located.
- A user can easily read any CSV dataset and track the information about the deployed dataset to be consumed by the Notebook.

> This interesting information snippet is well documented within a Notebook file (.ipynb) itself and that is `pandas.read_csv("location")`.

See below.

![Dataset Information in NB](/_images/usedsinb.png)

- The information about consumable dataset for a particular Notebook can also be found in the metadata of Notebook description.

To see the content of deployed CSV dataset, open the file in the dataset folder. Refer the figure below.

![Dataset Information in NB](/_images/contentdsnb.png)


### 5.4 Run a Notebook File

To run a selected Notebook file, follow the below steps.

1. Go to `Run` menu.
2. Select `Run All Cells`.

This will cause the corresponding dataset get consumed and enable processing the algorithms.

![Run Notebook File](/_images/run_nb.png)

> Note: To execute these steps, you should be logged in to JupyterLab. Then you should navigate inside target notebook folder where the file to be processed is saved.

Alternatively, you can choose to click `Play` button visible on the top menu of the Notebook file, consume and process the dataset. 

![Run Notebook File](/_images/playnb.png)


## 6. Getting Help

If you encounter any problems when setting up or using Data Explorer, please let us know - we're here to help you!

To report a bug, please open a [Github issue](https://github.com/edge-trial/Support/issues) and we will get back to you about your concern. 

> Make sure you set up a separate public Github account for this purpose.

_Providing as much information as possible about your issue will help our Support Team to give you a more complete response in quick time._

------------
## 7. Further Reading

> A comprehensive list of links to information that will help you find what you are looking for.

To learn more about the repositories for a Jupyter project, you can take a moment and read the following documentation.

- [About Python](https://docs.python.org/)
- [Python Standard Libraries](https://docs.python.org/3/library/)
- [JupyterLab Reference](https://jupyterlab.readthedocs.io/en/stable/)
- [More About Jupyter Notebook](https://jupyterlab.readthedocs.io/en/stable/user/notebook.html)
