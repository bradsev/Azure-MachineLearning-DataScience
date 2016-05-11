###  Linux Data Science Virtual Machine with Jupyterhub custom extension


[![Deploy to Azure](http://azuredeploy.net/deploybutton.svg)](https://azuredeploy.net/)

This Linux based virtual machine contains popular tools for data science modeling and development activities. The main tools include Microsoft R Open, Anaconda Python distribution, Jupyter notebooks for Python and R, Postgres database, Azure command line tools, libraries to access various Azure services like AzureML, databases, Azure storage and big data services. It also has machine learning tools and algorithms like CNTK (a deep learning toolkit from Microsoft Research), Vowpal Wabbit and xgboost. 

This extension enhances the Linux data science VM with  [Jupyterhub](http://jupyterhub.readthedocs.io/en/latest/) that provides a multi user capabilities to Jupyter notebook service. This capability can be useful in training or team environment where a shared VM is used serve multiple users. As a trainer, you create one or more shared Linux VM with the Jupyterhub extension and create separate OS user accounts for each student on the VM. The students will login with the credentials and will have their own instance of Jupyter that the can follow through independent of other students. The extension works by executing the script ```installjupyterhub.sh``` on the VM as a post provisioning step which installs Jupyterhub without any user intervention. Jupyter is already preinstalled on the data science VM. 

### Accessing Multi-user Jupyter through Jupyterhub 
Create local user accounts and password on the VM. Each user can access the multiuser jupyter notebook server by visiting ```https://<VM Full DNS name>:8000/``` on a browser and logging into Jupyter with the OS user login credentials. Once successfully logged in you will see your Jupyter home page with a list of sample notebooks.  Now you can execute existing notebooks or create new notebooks in R, Python 2 or Python 3. 

### About the Linux Data Science VM
The Linux data science VM helps jump start modeling and development for your data science project using software commonly used for analytics and machine learning tasks in a variety of languages including R, Python, SQL, Java and more all pre-installed. Jupyter notebooks offers a browser based experimentation and development environment for both Python and R. Microsoft R Open included in the VM. On the VM, the Azure SDK for Python, R, Java, node.js, Ruby, PHP allows you to build your applications using various Azure services in the cloud including the Cortana Intelligence Suite which is comprised of Azure Machine Learning, Azure data factory, Stream Analytics, SQL Datawarehouse, Hadoop, Data Lake, Spark and more. We also have other powerful machine learning tools and algorithms like CNTK (a deep learning toolkit from Microsoft Research), Vowpal Wabbit, xgboost pre-installed locally. Azure command line tools allow you to manage your Azure resources. Other development tools include run time for Ruby, PHP, node.js, Java, Perl, Eclipse, standard editors like vim, Emacs, gedit). A remote graphical desktop is also provided with VM side pre-configured (needs one time X2Go client side download). You have full access to the virtual machine and the shell including sudo access for the account that is created during the provisioning of the VM. This VM is built on top of Linux Openlogic CentOS-based version 7.2 distribution. 

For more information on provisioning and using the Linux Data Science VM, please check out the [documentation page](https://azure.microsoft.com/documentation/articles/machine-learning-data-science-linux-dsvm-intro/).

You can click on the "Deploy to Azure" button to try out the VM (Azure subscription required. Hardware compute [fees](https://azure.microsoft.com/en-us/marketplace/partners/microsoft-ads/linux-data-science-vm/) applies. [Free Trial](https://azure.microsoft.com/free/) available for new customers). 

**IMPORTANT NOTE**: Before you proceed to use the **Deploy to Azure** button you must perform a one-time task to accept the terms of the data science virtual machine on your Azure subscription. You can do this by visiting [Configure Programmatic Deployment](https://ms.portal.azure.com/#blade/Microsoft_Azure_Marketplace/LegalTermsSkuProgrammaticAccessBlade/legalTermsSkuProgrammaticAccessData/%7B%22product%22%3A%7B%22publisherId%22%3A%22microsoft-ads%22%2C%22offerId%22%3A%22linux-data-science-vm%22%2C%22planId%22%3A%22linuxdsvm%22%7D%7D)

[![Deploy to Azure](http://azuredeploy.net/deploybutton.svg)](https://azuredeploy.net/)