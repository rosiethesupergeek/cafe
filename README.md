# Rosie's puds - Introduction

**Rosie's puds** Rosie's puds is a dessert website for those with a sweet tooth. I have used this as the website for my final project for a Code Institute bootcamp. This project uses Django full stack framework.

> It targets **puddings, traditional and new** of a large variety in order to delight and create a positive emotional response in the website user. These puddings are a lovely treat presented in a visually pleasing and easy to navigate way. This satisfies the need of the user to find a sweet treat easily, and then makes the sales and delivery process of that sweet treat smooth and trouble free.
The user can view the pictures of the puddings that they might like, order a pudding easily and organise payment and delivery of said pudding easily too.

----

## [Content](#content)
- [Rosie's puds - Introduction](#rosies-puds---introduction)
  - [User Experience - UX](#user-experience---ux)
    - [Site Aims](#site-aims)
    - [Agile Methodology](#agile-methodology)
      - [Epics and User Stories](#epics-and-user-stories)
      - [Tasks](#tasks)
  - [Design](#design)
    - [Colours](#colours)
    - [Imagery](#imagery)
    - [Wireframes](#wireframes)
  - [Database Diagram](#database-diagram)
  - [Features](#features)
    - [Home Page](#home-page)
      - [Navbar](#navbar)
      - [User Page](#user-page)
      - [Footer](#footer)
    - [About Page](#about-page)
    - [Menu Page](#menu-page)
      - [Deliver Page](#deliver-page)
      - [Search Button](#blog-comments)
    - [Super User Access](#super-user-access)  
  - [Technologies Used](#technologies-used)
    - [Languages Used](#languages-used)
    - [Django Packages](#django-packages)
    - [Frameworks - Libraries - Programs Used](#frameworks---libraries---programs-used)
  - [Testing](#testing)
      - [Validation](#validation)
      - [Manual Testing](#manual-testing)
  - [Bugs](#bugs)
      - [Fixed Bugs](#fixed-bugs)
      - [Future Implementation](#future-implementation)
  - [Credits](#credits)
    - [Code](#code)
    - [Learning Resources](#learning-resources)
  - [Acknowledgement](#acknowledgement)

-----

# User Experience - UX

## Site Aims

* Rosie's puds is a website that aims to show users great puddings that they can order, pay for and organise the delivery of in one easy to navigate place.
* The site gives the user a positive emotional experience by being easy to navigate, visually pleasing and excites the user by giving them the possibility of a tasty pudding arriving at their door.
* This website provides the user with the ability to see the puddings and choose as many as they would like for delivery.
* Staff who organise delivery can mark an order as delivered and can mark an order as paid. They can see all orders, order ID, whether it has been paid or not and whether it has been delivered or not.
* Business owners/super-user can also see the number of orders, order ID, total revenue taken, whether an order is paid and whether an order has been delivered. They can also add and delete items from the database and website.
* Super-user can access all the features of the website and can read, create, edit, and delete puddings or info of their choosing.

## Agile Methodology

The Agile Methodology was used to plan this project. This was implemented through Trello and the kanban board. Using this Kanban board I divided the project into several sections: 

* Design- This held all the design tasks for the project.
* To do- These were tasks yet to be completed, once began these were moved to the "Doing" label.
* Doing- Once tasks had begun they were moved to this column.
* Testing- These held the testing protocol for the project.
* Done- this holds all the completed tasks.
Please find my Kanban Board here ![Trello board](/readme_pictures/trello_board.png).

## Epics and User Stories

Following Epics were created which were further developed into several User Stories.

### Epic 1- Website UI
Epic Goals for User- 
* Easy to navigate and find the pudding of your choice.
* Easy to add the pudding to your basket, pay for it and organise delivery of it.
* Search bar for regular customers or new customers to find their favourite pudding, or a pudding of their desire.
* Can immediately see the purpose of the site once landing upon it.

#### Related User Stories:
* As a site user I can easily see the point of the site, so that I can stay on it and find what I need or leave immediately because it's not something I want.
* As a site user I can view a list of the puddings so I can find the one I want.
* As a site user I can use the search bar to find the pudding that I want.
* As a site user I can click on a pudding to add it to my basket.
* As a site user I can see a description of the pudding so that I can see if I want to order it.

### Epic 2- Registration and Account Management
Epic Goals-
* Quick and easy creation of staff account.
* Quick and easy sign up, sign in and sign out of the super user and staff.
* Upon signing in, the user should be able to add a pudding, delete a pudding, change the description of a pudding, add staff users (easy access to Create, Read, Update and Delete (CRUD) features)

#### Related User Stories:
* As a staff user, I can register an account so that I can make changes to the orders.
* As a staff user, I can login and logout of the site so that I can access the orders.
* As a staff and super user, I can view the number of orders, see which ones have been paid and which ones have been shipped.
* As a super user I can make changes to the description and pictures of the puddings on the website.

### Epic 3- Pudding Post Management
Epic Goals-
* Create/ Update / Read / Delete pudding images and descriptions.
* View the created puddings.
* Approve and publish a picture and description of a pudding.

#### Related User Stories:
* As a site admin/author, I can create, read, update and delete posts to manage the blog content.
* As a site admin, I can delete any pudding so that when puddings have ran out, the site visitor will no longer see them.
* As a super user I can see the total revenue, the current orders and what stage of the process they are at (shipped or not? paid or not?) helping me to keep track of what is going on with the business.

## Tasks

The tasks created for this project were put together following the tasks and order of the Django project "I Think Therefore I Blog" and Legion Script's YouTube channel series for the creation of a food delivery app.

**Before Project Inception**

- Design Entity Relationship Diagram in order to understand which data I wanted to gather and how it would relate to itself.
- Create Repository in GitHub and install Django, Bootstrap and Crispyforms.
- Create Project, Epics, User Stories and organise project tasks on Kanban Board in Trello.

**Creation of Project in GitPod**

- Create the Django project.
- Create the database models
- Set up models.py file in "rosecafe/restaurant" directory
- Set up Index and About pages: this includes creating base.html which contained the Navbar and Footer content, which I used in all template files. This created the consistency of the design of the project.
- Set up other Template files: about.html, footer.html, index.html, menu.html, navigation.html, order_confirmation.html, order_pay_confirmation.html, order.html.
- Set up views.py and urls.py
- Set up order system
- Add payment system
- Create staff login and dashboard.
- Add order details.
- about.html (Description about Rosie's Puds)
- footer.html (footer containing our restaurant login and copyright details)
- index.html(homepage containing the order now button and hero image)
- menu.html ( contains the puddings available for order)
- navigation.html(the navigation bar holding the buttons to order, get info about the company and to see the menu)
- order_confirmation.html(to confirm to the customer their order has gone through successfully)
- order_pay_confirmation.html(confirms to the user that they have paid successfully)
- order.html (takes the details of the delivery for the order)
- Install Allauth for sign in, sign up and sign out templates with-  pip3 install django-allauth 
- Install crispy-forms to add styles to Django account templates with-  pip3 install crispy-bootstrap4
- Deployment

-----

[Back to top](#content)

## Design

### Colours

The colour scheme is inspired by other sweet treat websites. I chose pastel colours associated with sweets in order for the website to be consistent with the baking industry.  

![Color Palette](readme_pictures/colours.png)

### Imagery

All imagery is related to cakes and puddings as this is the produce the website is selling, aimed to entice the viewer to purchase through strong appealing imagery.

### Wireframes

The wireframes for this projected were generated using Canva. 
- [Wireframes for Desktop Homepage](readme_pictures/homepage_desktop.png)
- [Wireframes for Desktop About Us](readme_pictures/about_us_desktop.png)
- [Wireframes for Desktop Order](readme_pictures/order_page.png)
- [Wireframes for Mobile Menu and Order](readme_pictures/mobile_menu_order.png)
- [Wireframes for Mobile ](readme_pictures/mobile_about_us.png)

----

## Database Diagram

ERDplus was used to create a database schema to visualise the types of database models this project needed. In hindsight this project could use a "customer" model which would allow for customer login and more customer data to be stored.

![ERD Diagram](readme_pictures/erd_diagram.png)

[Back to top ⇧](#content)

----

# Features

## Home Page

- The user can immediately tell what the page is about.
- The hero image is pleasing and appetising enticing the user to view further products.
- The user can immediately navigate through to the other pages to see the menu of products, information about the company (about Us) and place an order.

![Homepage Desktop View](readme_pictures/homepage_desktop_rosecafe.png)
![Homepage Tablet View](readme_pictures/tablet_view_cafe.png)
![Homepage Mobile View](readme_pictures/mob_home.png)


----

## Navbar

- The nav bar is present on all pages and means the user doesn't need to press the back button lots.
- The navbar is responsive and clear.

![Navbar Mobile](readme_pictures/navbar_mobile_cafe.png)

![Navbar Desktop](readme_pictures/desktop_nav.png)



## User Page

* The logged in super user and staff can see a dashboard with all orders, total revenue, the shipping status of each order, the paid status of each order, and the total number of orders.
* Each order has an: ID, price, name, email, street, city, state, zip code, and a space for details.

![logged-in dashboard](readme_pictures/dashboard_cafe.png) 

----

## Footer

- The website footer contains the copyright information for the company, the login button for staff/user and another deliver button.

![Footer](readme_pictures/footer_cafe.png)

----

## About Page

- The About Page gives users information about Rosie's puds company and the current business. This adds a human touch to the site.

![About Us](readme_pictures/about_cafe.png)
----

## Menu Page

This page contains the menu of different puddings available to buy. These images are intended to entice and encourage the user to buy.

![Menu Page](readme_pictures/menu_page.png)

----

## Order Page

This page contains the menu with the ability to select each menu item the customer wants to order.

![Order Page](readme_pictures/m.png)


----

## Deliver Page

- This page contains a very obvious call to action button that encourages the customer to place an order.
- When the customer clicks the button it takes them through to the website page.

![Deliver Page](readme_pictures/deliver_page.png)

----

## Search Button 

On the Menu page there is a search bar to allow users to find a favourite regular order, or see if there is a particular pudding they are hoping to find.

![Search button](readme_pictures/search_pic.png)

- On the search results page customers can see the corresponding puddings to their search query.
![Search button](readme_pictures/search_query_pic.png)


----

[Back to top ⇧](#content)

## Superuser access

- The superuser can access the backend of the site by inputting their username and password. The page appears like so:

[here](readme_pictures/admin_page.png).

- On the Admin Panel accessible to the superuser, I can carry out all CRUD functions so I can view, create, edit and delete menu items (puddings).
- The superuser can also give other permissions to staff users and alter orders too.

### Admin 'Pudding Item' Model Management

- On selecting Menu Items in Customer, a list of Menu Items is displayed. When a menu item is selected, the superuser can see the: item name, description, image, price and category.
- The superuser can select menu items, delete them, add them and edit their associated information.

The admin site for pudding item model appears as shown [here](readme_pictures/menu_item.png).

### Admin 'Order' Model Management

- Upon selecting the order model under customer in the admin panel, the superuser can see a list of orders with the date and time the order was placed.
- When the superuser clicks on an order, it displays the: price, menu items ordered, the name, email and address details of the person who sent the order. The order also has a paid check box and a shipped check box. These are either checked or unchecked depending on the status of the order.

The admin site for order model appears as shown [here](readme_pictures/order_page.png).


----

## Technologies Used

### Languages Used

* HTML 5- used for the templates and therefore site content.
* CSS 3- for styling of the site.
* Python- For site functionality.

### Django Packages

* Allauth - for registration, authentication and account management.
* Crispy Forms - for form styling.

### Frameworks - Libraries - Programs Used

* Django framework held the project and connected the Model, View and Controller.
* Bootstrap4: used to style the wesbite and for responsiveness.
* Git for version control.
* PostgreSQL for the project database.
* Canva to build the wireframes for the project.
* Google Chrome Developer Tools to understand bugs and to test the site using the Lighthouse function.
* Font Awesome for icons used on the site.

-----

[Back to top ⇧](#content)

## Testing

### Validation
In order to test my site I used the following tools:
- [W3C HTML validator](https://validator.w3.org/) to test HTML
- [Jigsaw CSS validator](https://jigsaw.w3.org/css-validator/) to test CSS.
- [PEP8 CI Python Linter](https://pep8ci.herokuapp.com/) to test Python code.

### Manual Testing
Testing that the project performed as expected took place continuously throughout the build. Bugs were fixed before moving on.

Please see below a walk through of the steps of ordering and paying for some puddings:

- Select puddings:
![Search button](readme_pictures/pud_select.png)

- Fill out form:
![Search button](readme_pictures/pud_form.png)

- Click the submit button and confirm on the modal:
![Search button](readme_pictures/pud_modal.png)

- Submit payment details and click submit and you will see this screen :
![Search button](readme_pictures/pud_paid.png)

- To see the order, login to admin or staff:
![Search button](readme_pictures/pud_dashboard.png)

- Select the order details icon to see the details of the order:
![Search button](readme_pictures/pud_order_details.png)


- The search bar works as shown below:
![Search button](readme_pictures/search_query_pic.png)

----

## Bugs

| **Bug** | **Fix** |
| ----------- | ----------- |
| Whole site would not function.| Had just tried to add authentication, but I had accidentally left out "Mixin" so it would not work. I reviewed my code and added "Mixin" in to code in the appropriate places and the site then worked |
| Problems with allauth | The site would not call in functions of allauth because I had put the templates folder in the wrong place. I moved the templates directory and put the correct file path and the allauth then worked |

----

## Future Implementation

* Add more models to the database so that the site can include drinks to accompany the puddings and an extras menu so that customers can add extra toppings or sauces of their choice.

[Back to top ⇧](#content)

# Credits

## Code
- I used the CI course content to put together my code as well as Legion Script YouTube channel series "Build a Food Delivery App".
- I worked alongside many colleagues who all contributed to the debugging process and understanding of this project.

## Learning Resources
- Youtube videos by Legion Script.
- Code with Mosh subscription service.
- W3Schools website
- Django documentation
- Stack overflow posts
- Bootstrap documentation

## Content and Media

Images are taken from Pexels and Canva.

----

## Acknowledgement

Thanks to Richey Malhotra and Jack Crane for helping me so much with this project.

[Back to top](<#content>)
   