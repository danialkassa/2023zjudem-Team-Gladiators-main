# How To Develop the website

 ## A: Installing necessary Tools
 We installed all the following tools to build the website
    
- [Git](https://git-scm.com); It serves as a control system for tracking changes to the code base, collaborating, managing project versions, which allows us to clone, commit, and push changes to GitHub。
- [Github](https://about.gitlab.com/);This is where our web page is hosted.
- [Github desktop](https://www.gitbook.com/);Since it is a user-friendly GUI application, we use it to streamline our Git workflow, allowing us to easily clone, commit, and sync repositories.
- [VScode](https://code.visualstudio.com/); We enhanced our web development workflow with this versatile and customizable tool.
- [Nodejs](https://nodejs.org/en/);  Since the tool includes NPM, we used it to manage packages, interact with the command line, and integrate with VScode
- [Markdown language](https://www.nexmaker.com/doc/1projectmanage/markdown.html); This language helps us format plain text by creating headings, lists, links, images, and emphasis.

 ## B: Set up the page
 We visited the GitHub website (https://github.com) and registered a new account. Once logged in, we click the "+" button in the upper right corner of the GitHub homepage and select "New Repository." Then we gave it a name and selected whether it should be public or private. Then, after enabling the readme, we wrote some description of the project.
 <br>
<img style="float: center;" width=700 src="image/login.jpg">
<br>
<img style="float: center;" width=700 src="image/plus.jpg">
<br>
<img style="float: center;" width=700 src="image/Createrepository.jpg">
<br>
<img style="float: center;" width=700 src="image/Createrepository1.jpg">


 ## C: Local setup

   ### 1. Github Desktop

 In GitHub Desktop, we go to Files and Clone Repository.
After selecting the repository to clone, We selected the directory to save the cloned repository. Then we click "Clone" to start the cloning process. Once the cloning is complete, we navigate to the location of the cloned repository.

<br>
<img style="float: center;" width=700 src="image/clone.jpg">

<img style="float: center;" width=700 src="image/clone.jpg">

   ### 2. Vs Code

After installling VS code, We opened our folder on the vs code to develop the website.

<br>
<img style="float: center;" width=700 src="image/vs.jpg">

<br>

   ### 3. Install Docsify


 In the VS code, We opened the terminal and New terminal.

 <br>
<img style="float: center;" width=600 src="image/term.jpg">

<br>

And by Writing "npm i docsify-cli -g" in the terminal and hit enter, we installed docsify.

<br>

<img style="float: center;" width=600 src="image/installingdocsify.jpg">
<br>

 We then initialize it by typing “docsify init./docs” in the terminal command and hit enter so that Docsify creates the necessary files and folders in the specified directory.

  <br>
<img style="float: center;" width=600 src="image/initialize.jpg">

  We then type "docsify serve docs" into the command terminal to instruct Docsify to serve the documentation site. We open it in the browser by clicking CTRL + "https://losthost:3000".

  <br>
<img style="float: center;" width=600 src="image/serve.png">

<br>

Finally, our docs displayed this way.

<br>

<img style="float: center;" width=600 src="image/des.jpg">
<br>

    <!DOCTYPE html>
    <html lang="en" xmlns="http://www.w3.org/1999/html">
    <head>
    <meta charset="UTF-8">
    <title>Gladiators docs file</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="description" content="Description">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">
    <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar.min.css" />
    <meta name="theme-color" content="#661a1d">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
    <link rel="stylesheet" href="//unpkg.com/docsify/lib/themes/vue.css">
    <link rel="stylesheet" href="bootstrap-grid.min.css"/>



    <link rel="stylesheet" href="common-1.css"/>
        <link rel="stylesheet" href="style.css"/>
    <!-- Responsive-->
    </head>
    <div id="app"></div>

            <script>
        window.$docsify = {
        name: 'GLADIATORS',
        repo: '',

        loadSidebar: true, //prepare for sidebar
        loadNavbar: true, //prepare for navbar
        mergeNavbar: true,

        executeScript: true,
        homepage: 'home.md',
        search: 'auto', // default

        // complete configuration parameters
        search: {
            maxAge: 86400000, // Expiration time, the default one day
            paths: 'auto',
            placeholder: 'Search',
            noData: 'No Results!',
            // Headline depth, 1 - 6
            depth: 6,
            hideOtherSidebarContent: false, // whether or not to hide other sidebar content
        },

        copyCode: {
        buttonText: {
        '/zh-cn/': '点击复制',
        '/'      : 'Copy to clipboard'
        },
        successText: {
        '/zh-cn/': '复制',
        '/'      : 'Copied'
        }
    },



        subMaxLevel: 3,
        sidebarDisplayLevel: 1, // set sidebar display level
        }


    </script>
            <!-- Docsify v4 -->
            <script src="//unpkg.com/docsify/lib/plugins/search.js"></script>
    <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
            <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
            <script src="https://unpkg.com/docsify-copy-code"></script>
        </div>
    </div>
    </body>
    </html>
  - To preview web pages, we installed the "Live Server" extension from the VS Code Marketplace.
  <br>

<img style="float: center;" width=600 src="image/pre.jpg">

<br>

   Once the live server preview is installed, We opened the HTML file, then right-click and select Open with Live Server. 
   <br>

<img style="float: center;" width=600 src="image/live.jpg">
<br>


  ### 5.  Add sidebar and navigation bar

<!--docs/_sidebar.md -->

- ACTIVITIES

 + Project Management

    - [Website Development](AC/step/page.md)

 + CAD
  
    - [Introduction to Fusion 360](AC/CAD/installation.md)
    - [Assignment](AC/CAD/handson.md)
  
 + ARDUINO

    - [Introducation](AC/Arduino/Introduction.md)

 + PRINTING

   - [ 3D PRINTING](#)
 
 + LASER

   - [LASER CUTTING](#)

 + PROGRAMMING

   - [INTERFACE APPLICATION PROGRAMMING](#)

 + IOT

   - [IOT and INTERACTION](#)

 - FINAL PROJECT

   - [Proposal](AC/Project/proposal.md)
  
  

  
  
      -We open the index file and go to window. .$docsify and then add
              loadSidebar: true,

 - Collapsible sidebar
To make the sidebar collapsible,we just need to add this code in window.$docsify


             subMaxLevel: 3,
             sidebarDisplayLevel: 1, // Set sidebar display level

Then insert the script into the document, just like the official plugin usage

              <!-- plugins -->
               <script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>

- NAVBAR

Create file  Navbar.md

             - [MEMBERS](INTRO/NAVBAR/member.md)
             - LANDUAGE
              - [CHINESE](/CHINESE/)

Open the index file go to window.$docsify and add

             loadNavbar: true,

  ### 6. Prepare and save documents

  ### 7. Uploading Image

 We created an images folder in the document to store all the pictures.

A folder named "Image" is created in a directory named "docs". The purpose of this folder is to store all pictures or images related to a specific assignment or document.

Then we drag and drop them into the document.

We find the required image file in the images folder and drag it to the document we are working on. This action places the image at the desired location in the document.

"...use 'img style="float: center;" width=700 src="IMAGE/nameof ourimage.png/jpg" format.'"

This section describes how to use the HTML <img> tag to insert images into a document.

style="float: center;": This attribute sets the float property of the image to "center", which means that the image will be centered horizontally within its containing element.

width=700: This attribute sets the width of the image to 700 pixels. This determines the visual size of the image in the document.

src="image/foldr name.png": This attribute specifies the source of the image (src). In this case, it points to a file called "name of our image.png/jpg" located in the "image" folder. The path "name of our image.png/jpg" means that the image folder is located in the current directory, and the image file name is ""nameof our image.png/jpg".png".

Format: "Format" seems to be mentioned, but has no specific meaning in this context. It may be included as a placeholder or for other purposes, but it does not affect the image insertion itself.

In short, we describe the process of creating an image folder to store pictures. Then, add these pictures to our document by dragging and dropping them where we want. Images are inserted using the HTML <img> tag, which has specific properties to control its appearance, including alignment, size, and source.


 <br>
<img style="float: center;" width=700 src="image/im.jpg">

 ### 8: Upload files
  1. We established a connection between our local repository and the GitHub repository.
We commit and push the file to GitHub:

To upload our web files to GitHub, we used the command “push commits to the origin remote”.
The “push” command sends committed changes from our local repository to the GitHub repository.

 <br>

<img style="float: center;" width=700 src="image/commit.jpg">

 <br>
<img style="float: center;" width=700 src="image/push.jpg">
  <br>
   
<br>
 2. 
To publish our web page, we look for the settings for our GitHub repository. Then scroll down to the GitHub Pages section and select the branch that contains our web files.
We select the folder or root directory where the web page file is located.
Then click the "Save" or "Update" button to apply the changes.
GitHub generates a URL for our published web page that we can share and access publicly. We can see this process as follows.
<br>

<br>
<img style="float: center;" width=700 src="image/setting.jpg">

<br>
<img style="float: center;" width=700 src="image/page.jpg">
<br>
<img style="float: center;" width=700 src="image/save.jpg">


## D. Setting up  the Members

 [Template](https://bestjquery.com/tutorial/our-team/demo16/)
<br>
 First we downloaded the "saveallresourse" tool and addded to the chrome extention. 
 The "saveallresource" saves all the files and assets of any website. It downloads resources like HTML, CSS, JavaScript files, images, and more, preserving the folder structure. The tool helped us to quickly gather and preserve all necessary website files.

Here is the code to display the Members.   

            
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="style.css">
        <title>GLADIATORS</title>
        <link rel="stylesheet" href="teamstyle.css"/>
    </head>

    <body>
    <div class="container">
    <h2 style = "text-align: left; font-size:40px;">Group Introduction</h2>
            <strong><p> We , the Gladiators, are diverse group of passionate individuals studying industrial design engineering,<br> united by a common goal to create solutions that address the United Nations Sustainable Development Goals (SDGs).</</P></strong>
          
        </div>          
    </body>

    <div class="demo">
            <div class="container">
                <div class="row text-center">
                    <h2 class="white" style="text-align:left; font-size:40px;">Group Members </h2>
                    <br>
                    <br>
                </div>
    <div class="demo">
    <div class="container">         
                <div class="row">
                    <div class=" col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member1.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://danialkassa.github.io/"><h2>Daniel Kassa</h2></a></li>
                                <span><h3>From Ethiopia</h3></span>
                                <p class="description">
                                      I am interested in design and programming. I stay updated in rapidly evolving fields with the latest technologies, trends, and design principles.</p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member2.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://shahri128.github.io/EngShahari.github.io/"><h2>Arslan Ali</h2></a></li>
                                <span><h3>From Pakistan</h3></span>
                                <p class="description">
                                  I'm a versatile scholar with a background in agriculture engineering and am currently pursuing my master's in industrial design engineering at Zhejiang University, China. Beyond this, I share my passion for technical problem-solving as a content creator on YouTube.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    <div class="demo">
    <div class="container">         
                <div class="row">
                    <div class=" col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member3.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://sahle1415.github.io/Sah/"><h2>Sahle Hagos</h2></a></li>
                                <span><h3>From Ethiopia</h3></span>
                                <p class="description">
                                      I am a chemical engineer with a passion of designing industry products in a user-centered and sustainability-oriented way, 
                                      and soon I will be in touch with anyone who needs my support in industry product design.</p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member4.jpg" alt=""/>
                            </div>
                            <div class="member-prof">
                            <li><a href="https://arsl0011.github.io/alif.github.io/"><h2>Arslan Ali</h2></a></li>
                                <span><h3>From Pakistan</h3></span>
                                <p class="description">
                                  I am an industrial design engineer. My studies focused on the resource development and management sides of designing.  have always been interested in the science behind designing, which is why I chose to pursue a career in this field.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    <div class="demo">
      <div class="container">
          <div class="row">
                    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                            <img src="image/member5.jpg" alt=""/>
                            </div>
                            <div class="member-prof">,
                                <li><a href="https://steve12437.github.io/"><h2>Steve</h2></a></li>
                                <span><h3>From Cameroon</h3></span>
                                <p class="description">
                                  I am outgoing, dedicated,and open-minded. I get across to people and adjust to change with ease.
                                  believe that a person should work on developing their proffessional skills and learning new things all the time.
                                </p>
                            </div>
                        </div>
                    </div>

    <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member6.png" alt=""/></div>
                            <div class="member-prof">
                            <li><a href="https://atj12345.github.io"><h2>Ahmed Tajah</h2></a></li>
                                  <span><h3>From Sierra Leone</h3></span>
                                <p class="description">
                                  I am proud to be a Fula by tribe and a graduate of Njala University, holding both a BSc Hons in Business and Information Technology and an MSc in Information System Management.Currently based at Zhejiang University in China, I am pursuing my second master.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-sm-4">
                        <div class="Members">
                            <div class="pic">
                                <img src="image/member7.jpg" alt=""/></div>
                            <div class="member-prof">
                            <li><h2>Sana</h2></a></li>
                                  <span><h3>From pakistan</h3></span>
                                <p class="description">
                                  I hold a Bachelor's degree in BS Physics from Government Frontier College for Women, Peshawar. Currently, I am pursuing a Master's in Industrial Design Engineering at Zhejiang University, Ningbo, China, blending my passion for science and design into a unique skill set.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>


# E. LANGUAGE

The docs file's content when opened in the VS code

    .
    └── docs
       ├── README.md
       ├── index.htm
       ├── Sidebar.md
       └── navbar.md

The English and Chinese version the website Looks like This

    .
    └── docs
       ├── README.md
       ├── Home.md
       ├── index.html
       ├── Sidebar.md
       └── navbar.md
    └── CHINESE
       ├── Home.md
       ├── README.md
       ├── index.html
       ├── Sidebar.md
       └── navbar.md

 the index file

     homepage: 'home.md',
     mergeNavbar: true,

every member has the right to change or edit the website. 

<br>
<img style="float: center;" width=700 src="image/language.jpg">
<br>

# F. Collaboration
 ## Step1: 
   As admin, I login the github group account, Then click  "Settings". In the "Access" section of the sidebar, click "Collaborators and teams". Then "add people" displayed as follows.

<br>
<img style="float: center;" width=700 src="image/add.jpg">
<br>

 ## Step2: 
As shown in the figure, there is   "add people" section.
 by clicking "add people", I invited the members by writing Username, Full name, or Email. Then after the following image dispalyed.

<br>
<img style="float: center;" width=700 src="image/select.jpg">
<br>

 ## Step3:
   After sent invitation, I chose the role of every member in the team to have a mentain role. Now, every member has the right to change or edit the website. 
<br>
<img style="float: center;" width=700 src="image/list.png">
<br>

# G. References 

 - [Nexmaker](https://www.nexmaker.com/)
 - [Docsify](https://docsify.js.org/#/?id=docsify)
 - [Template](https://bestjquery.com/tutorial/our-team/demo16/)
 - [Google Translate](https://translate.google.com)
