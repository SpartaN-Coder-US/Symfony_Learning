# Symfony_Learning

This is my project at applying the skills I gain throuout my journey of learning Symfony framework and php.

I'm following a course which is spread in sections. 

I will commit and push to the 'testing' branch after every video . After I complete  1 section I will push  it to the main and repeat.

After the 8 hrs I am spending at the office, my notes from the OneNote will be attached bellow with the date,  for better track of progress.

If you find my repo, I hope it can help you too.

Thanks!

Notes:

Monday Semptember 23 2024:
###########################################


-------------------------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section 1 (The introduction)

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-------------------------------------------


1. Course Outline

Monday, September 23, 2024
9:15 AM

Our end goal is a fully functioning application just like "x/facebook/"

    • Controllers and Routing: We will learn how to return a response and define your app's routes.

    • Twig:  We will master twig for front end, covering everything from basic templates to inheritance and control

    · Maker & Profiler: Tools for rapid development and debbuging

    · Doctrine: migrations, fixtures, repositories, and outer entity fetching with param converters to make everything look sharp

    · Forms & UI: symfony forms and tailwind CSS, and even diving into dark and light modes.
    
    · Doctrine relations: 1 to 1 / one to many/ many to many

    · Security & Auth:  authorization (Asian voters) and the security component. 
    
-------------------------------------------
2. Why You Need a Framework and What is Symfony?

Monday, September 23, 2024
11:00 AM

First things first, it starts with php, PHP runs on the servers remotely

Typically we have the following scenario:

{Client ->  server -> php -> database} then {php -> server -> client}

(sends data to server)->(server runs php) -> (php will interact with the database)

                        THEN
                        
(Generates some html) -> (Server sends it to client) -> (user has new data on the website) 

Many projects were created via php and they slightly differ from one to another. 
It would be very hard to pick up from the beginning if we didn't use a framework, because 
The framework has many reusable components and also it gives the code structure

-------------------------------------------
3. Why Use Symfony and How Symfony Works in a Nutshell?

Monday, September 23, 2024
12:05 PM

Simfony is a very mature and stable framework, also it has a very big community. LTS support. Sustainable.
Rich documentation and also the reputation.

                                     Symfony is utilizing the MVC model. 
                                            MODEL VIEW CONTROLLER




![alt text](/pictures_readme/image.png)

    • Is a model of building applications where you separate the part that controls the flow of the application  (THIS BEING THE CONTROLLER)
    • Views: are responsible for generating an output, which is HTML or can be Json data. (Twig)
    • Model (Entity): which typically translates to a database model

Those 3 components make our symfony application. 

Let's  go through the flow of this request:

     There is always a single entry point that handles all the requests that the application receives, and the main component that decides where the request should be handled is called the router.
 
 ![alt text](/pictures_readme/image-1.png)

    • So the router will always route every URL to a specific controller.

![alt text](/pictures_readme/image-2.png)
 
    • This is configurable, so we have to be very specific  about which controllers should  handle which routes. 
    • It's responsible for the control of the actions. For example, it can first want to fetch some data from the model entity (database) and then the data is passed to the controller again which it can send it to the template engine (Twig) which then is being sent to the controller.

![alt text](pictures_readme/image-3.png)

    • View is our templating engine , because it's actually creating templates.
    • Twig is just the name of the templating engine used in symfony, and it has it's own syntax.
    • Then after the view is generated, it will be sent back to the controller.

After all the changes have been made the controller is sending back the data/information to the symfony application, which in return it will sent that back to the user browser.


-------------------------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section 3 (Instalation for Mac <Apple silicone chips>)    

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-------------------------------------------


17. Section Intro: Setting up for Mac!

Monday, September 23, 2024
9:15 AM

We are recommended some of the following tools XAMMP, a docker based repo, Planet scale ( free sub).

-------------------------------------------

18. Installing the Homebrew Package Manager (Prerequisite)

Monday, September 23, 2024
1:54 PM

Install via terminal:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

-------------------------------------------

19. Installing PHP on Mac

Monday, September 23, 2024
2:01 PM

Installed the php

    • Brew install php. (install via package manager homebrew)

    • php  -v (check the current version of php)

    • Update brew &&. Upgrade php.  (this if necessary << updates and upgrades brew and php respectively)
    
-------------------------------------------

20. Installing Composer on Mac

Monday, September 23, 2024
2:07 PM

Install composer on mac.

    • Brew install composer (install via homebrew)
        ○ Brew install composer

    • Composer about (check the installation version)
    
-------------------------------------------

21. Installing and Running Docker (MySQL, MailCatcher) on Mac

Monday, September 23, 2024
2:37 PM

Install docker:
    
    -Website link:
      https://www.docker.com/
    
    -Log in or create account 

-------------------------------------------

22. Installing Symfony CLI - Symfony Command Line Interface

Monday, September 23, 2024
2:54 PM

    • Go to the website: 
https://symfony.com/download

    • We will be using the homebrew approach:
    
        brew install symfony-cli/tap/symfony-cli

    • Restart teminal to make sure we have it running

    • Type: symfony in the terminal to check if it's installed.


-------------------------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section 4 (Instalation for Mac <Apple silicone chips>)    

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-------------------------------------------


