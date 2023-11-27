
NextJS Portfolio Template
Portfolio website template!
View Demo · Report Bug · Request Feature

Table of Contents
About The Project
Sections Available
Built With
Demos
Getting Started
Prerequisites
Installation
Usage
User Info
Blogs
Setting up Images
Setting up Themes
Setting up Contact Form
Deployment
Contributing
License
About The Project
Making a Portfolio website from scratch can be a tedious process. This repository solves that problem. How? Well, it is a easy-to-use portfolio template! You can use it by following a few simple instructions given below. Feel free to suggest changes and features too!

Sections Available
✔️ Landing Page - greeting
✔️ Work section
✔️ Capabilities
✔️ Education
✔️ About
✔️ Projects
✔️ Work Experience
✔️ Blogs - Custom, Medium and DevTo support
✔️ Contact me
✔️ Socials

Built With
🔧 NextJS
🔧 Chakra UI

Demos
To view a demo, click here
To view a live example, click here

Getting Started
To get a local copy up and running follow these simple steps.

Prerequisites
npm - Latest version of npm works the best with this project. Run the following command to install it.

npm -v //checks npm version
npm install npm@latest -g //installs latest npm version
Installation
Clone the repo
git clone https://github.com/AsavariA/nextjs-portfolio-template.git
Install NPM packages
npm install
Usage
These are instructions to use the project once you have cloned it. Follow them step by step for the best experience. Comments are mentioned in the files as guides.

User Info
Go to the file userinfo.js inside the Constants folder. Fill up this file like you are filling up a form.

logoText
contact - email, phone(leave blank if not willing to use), countrycode
socials - follow the json format
greeting - title, subtitle
capabilities - follow the json format
about - content, resume link ( can be drive link etc )
education - follow the json format
experience - follow the json format
blogs - if you want this section in your website, set it true, otherwise false. If true, follow the instructions in blog section
projects - go to Constants > projects.js and follow the json format. Import images as mentioned in the imports.
headings - you can customise all the headings in the template with this.
ctas - you can customise all the ctaTexts in the template with this.
Blogs
This instruction set is only applicable if blogs are set to visible. The blogs section provides 3 kinds of support. Custom blogs, importing medium blogs, or importing devto blogs.

Go to Constants > blogs.js
You will be able to see 3 different exports. Choose the one you want and comment out the others.
If your choice is Custom blogs, fill in the details as shown in json format.
If your choice is Medium blogs, then uncomment the medium blogs export down below and fill in your medium username.
Now move to Components > Work.js.
You will see three commented out sections each with a useEffect and heading MEDIUM BLOGS SUPPORT
Uncomment the useEffect in the section you want and comment the other two out.
You are set to import your medium blogs now!
Follow the steps from 4 - 8 but with DevTo details if your choice is DevTo blogs.
Setting up Images
There are only 3 images you need to set up externally. These images have to have a particular name and format and location.

Landing Page Background Image
name - background
type - .jpg
filename - background.jpg
location - root > styles
About Section Background Image
name - about
type - .jpg
filename - about.jpg
location - root > styles
Favicon Image
name - favicon
type - .jpg
filename - favicon.jpg
location - root > public
Setting up Themes
Go to the file theme.js inside the folder Constants. You can change the colors as per your wish or leave the theme as it is. Make sure to keep all the fields intact because skipping any field can lead to errors.

Setting up Contact Form
For this step, you will need to create a new google account which will send you the form data. Need for a new account - well, it is advisable to use this new account only for this purpose so as to prevent giving this template access to your personal emails ( which are on your original email account ). \

Once you have made your account, make sure you have selected that account and go to this link. Allow the access.\

Now go to the test.env file. Rename this file to only .env
If your project is on github, please make sure to exclude this file from github ( put it in gitignore ) since it contains private / environmental variables.

//type in all data without the < and > signs.

PASSWORD = <sender-mail-password> //password of newly created account
SENDER = <sender-mail> //email address of newly created account
TO = <reciever-mail> //email address of your personal account (which will be reciever of data in this case)
Contact form is now set up!

Deployment
To check if your website is running the way you wish, run the following command to start it locally on localhost:3000
npm run dev

To deploy your portfolio, you can use any of the following ways.

Vercel - this is the most advisable platform to deploy your nextjs applications because they are the building company and provide the best support for all nextjs websites.
Netlify - Use the exclusive nextjs support on netlify to deploy your site.
Both of these can be used directly through github and therefore any new changes and updates to your project repository will be updated immediately in the deployment. There are other ways and platforms to deploy your portfolio too.

Contributing
Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated.

Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
License
Distributed under the MIT License.