Art store
This project is a part of the 5 milestone projects within the Full Stack Developer course provided by Code Institute and was created using Django. The business offers a collection of different kinds of artwork which are available for sale, and also an opportunity to order a commissioned piece. The purpose of this project is to build a e-commerce store that is fully functional, with registered users and guset checkout.

UI/UX
The overall design of the site follows a simplistic and neutral style, that to make the artwork stand out.

Agile
This project was designed and built using the agile approach. When planning the project, I created a Kanban project, where to input 'issues' (or user stories), to help me following a direction while building this site. Each issue has been tagged with a label to signify how crucial a particular feature is to the overall workings and acceptability of the site.

Wireframes
The initial wireframes in Balsamiq are a simplified version of the finished application and merely served the purpose of listing most of the site's essential features.

Not all features and functions are covered by these first drafts. For a full list of existing features see Features.

SEO and marketing
My initial short key words for my site was:

Art commission
Functional art
Unique art
Artists in Stockholm
Buy unique art
Within the key word searches I found these:

How do I ask for an art commission?
Looking for art commissions
What are some examples of functional art
Wordtracker
Marketing strategies
This is a b2c business and the strategy for marketing I find relevant is:

Social media marketing On different media platforms, posting updates of what the artist is currently working on, finnished pieces, upcomming art shows etc.
E-mail marketing Setting up a newsletter subscription and start building up a mailing list. The send outs contains some additional perks for subscribers only, such like discounts etc.
Attending art shows. Word of mouth.
Features
Existing Features

Technologies Used
Work Environments and Hosting
Balsamiq (Wireframes) Lucid (ERD diagrams) GitHub (Version control) Codeanywhere (IDE) Heroku (Site hosting)

Python Libraries
Gunicorn (Python HTTP server for WSGI applications)
pyscopg2 (PostgreSQL Database adapter)
Pillow (Python Imaging Library)
django-storages (collection of custom storage backends for Django)
Flake8 (Python linter used for python code validation)
Django Libraries
django-allauth (User authentication)
django-summernote (WYSIWYG HTML editor)
Payment processing
Stripe (Online payment platform)
Emails/Newsletter
Mailchimp (Automated newsletter subscription service)
SEO/Marketing
XML Sitemaps (Sitemap generator)
Privacy Policy Generator
Testing
Bugs
Deployment
Using Github and Codeanywhere
To set up this repository, I use the Code Institute Full Template.

Click the Use This Template button.
Add a repository name.
Click the Create Repository from Template to create your repository.
To create a Codeanywhere workspace

create a new workspace with the URL that were created when the Github repository was created.
Pin the workspace so that it wont be deleted.
Committing your work should be done often and should have clear andexplanatory messages, use the following commands to make your commits:

git add . : adds all modified files to a staging area
git commit -m "A message explaining your commit": commits all changes to a local repository.
git push: pushes all your committed changes to your Github repository.
Installing libraries
The following steps outline all libraries needed for successful deployment on Heroku. All necessary requirements and settings updates will not be discussed in this section as they are assumed as logical follow-up steps to installments.

Install pyscopg2 (connects to PostgreSQL): pip 3 install dj_database_url pyscopg2
Install Gunicorn (server used to run Django on Heroku): pip3 install django gunicorn
Creating the Heroku App
Log into Heroku and go to the Dashboard
Click New and select Create new app from the drop-down
Name app appropriately and choose relevant region, then click Create App
Create PostgreSQL database using ElephantSQL
This is necessary to create a database that can be accessed by Heroku. The database provided by Django can not be accessed by the deployed Heroku app.

Log into ElephantSQL and go to Dashboard
Click Create New Instance
Set up a plan by providing a Name (project name) and select a Plan. Tags are optional.
Click Select Region and choose appropriate Data center
Click Review, check all details and click Create Instance
Return to Dashboard, click on the name of the newly created instance
Copy the database URL from the details section
Preparing for Heroku deployment
Create Procfile (tells Heroku to create web dyno which will run gunicorn and serve Django app)
Temporarily disable collectstatic (prevent Heroku from collecting static files when deploying)
Allow Heroku as host:

In settings.py add ALLOWED_HOSTS = ['app-name.herokuapp.com', 'localhost']

Connecting Heroku to Database
In Heroku dashboard, go to Settings tab
Add three new config vars DATABASE_URL (value is database URL), SECRET_KEY (value is secret key string) and PORT (value "8000")
Deyploying with Heroku
In Heroku dashboard, go to Deploy tab
Select "GitHub" as Deployment method and choose correct repository
Enable Automatic Deploys
Click "Deploy Branch" button
Fork and clone
Source Credits
References/Documentation/Tutorials

General:

The official Django Documentation was used throughout creating this project. The skeleton of this project is based on the Code Institute tutorial "Boutique Ado".

Fonts
All fonts were taken from Google Fonts.
