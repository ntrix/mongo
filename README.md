MongoDB & Mongoose
==================

Use MongoDB Atlas to host a free mongodb instance for your projects
For the following challenges, we are going to start using MongoDB to store our data. To simplify the configuration, we are going to use MongoDB Atlas.

MongoDB Atlas is a MongoDB Database-as-a-Service platform, which basically means that they configure and host the database for you, making it so that the only responsibility you have is to populate your database with what matters: data! We are going to show you how to:

Create a MongoDB Atlas account.
Create a new cluster.
Create a new user on the database.
Whitelist your IP address.
Connect to your cluster.
Create a MongoDB Atlas account
Let's start by going to MongoDB Atlas.

Once you open the MongoDB Atlas page, you should sign up for a new account.

Click the Sign In button in the top right corner to open the registration page.
Click the Register for a new account link at the bottom of the sign in page.
Fill the registration form with your information and press continue.
You should now be logged into your new account and see a modal with a green Build my first cluster button, click on it.
Create a new cluster
Go through the steps of building your first cluster by following the instructions they provide and clicking next after each step.

Choose your cloud provider and region, you can leave this as the default provided (typically AWS).
Customize your cluster's specs, you can also leave this as the default provided, M0 Sandbox (Shared RAM, 512 MB Storage) Encrypted.
Give your cluster a name, you can also leave this as the default provided, Cluster 0.
Now click the green Create Cluster button at the bottom of the screen and verify the image captions they provide.
You should now see the message Your cluster is being created - New clusters take between 7-10 minutes to provision. Wait until the cluster is created before going to the next step.
Create a new user on the database
On the left side of your screen click the Database Access button under Security to start creating a new user.
Click the Add New Database User button that is displayed in the next menu.
Enter a new username and password. You can set the privileges to Read and write to any database if they are not already. Then click Add User to finish creating the user.
Add your IP address
If you now click on the green Get Started button in the bottom left of your screen, you should see the next step to take highlighted, Add your IP address, click on it.

Follow the instructions by clicking on the IP Access List tab under the Security tab.
Click on the green ADD IP ADDRESS button.
In the modal, click the ALLOW ACCESS FROM ANYWHERE button and you should see 0.0.0.0/0 pre-filled for the whitelist entry field, click the green Confirm button.
Connect to your cluster
Clicking on the green Get Started button in the bottom left of your screen should now show you the final step, Connect to your cluster, click on it.

Follow the instructions by clicking on the Connect button in the Sandbox section.
In the pop-up modal, click on Connect Your Application, a connection string will be displayed, you can copy that connection string by clicking on the copy button.
This will be the final URI that you will use to connect to your db and will look something like mongodb+srv://<user>:<password>@<cluster#-dbname>.mongodb.net/test?retryWrites=true. Notice that the user and cluster#-dbname fields are already filled out for you, so all you would need to replace is the password field with the one that you created in the previous step.
