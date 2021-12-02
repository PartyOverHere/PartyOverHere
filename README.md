Original App Design Project - README Template
===

# Party Over Here
By: Makia Henderson, Zion Forbes, and David Hill
## Table of Contents
1. [Overview](#)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
Party Over Here is a mobile Android application that allows the user to plan the perfect party, wedding, or social event. The app will take users on a journey from start to finish with planning their events. 

### App Evaluation
- **Category: Lifestyle/Productivity**
- **Mobile:This app would be primarily developed for mobile but would be just as useful on a computer. Functionality wouldn’t be limited to mobile devices, however mobile version could potentially have more features.**
- **Story: This app conveniently equips users with access to all of their party planning needs in one place to plan a sure to stand out event.**
- **Market: Anyone who has an event to plan can take advantage of this app. Personalized suggestions are available depending on the needs and interests of the user.**
- **Habit: This app could be used as often or unoften as the user wanted depending on how often they plan or look for ideas in regards to events.**
- **Scope: First we would start with allowing the user to take our survey to help them plan their parties/events.Then perhaps this could evolve into a larger party planning application as well to broaden its usage to help coordinate larger events. Large potential for use with AirBnb, Zillow, or other location finding applications.**

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

The following **required** functionality is completed:

- [X] User can create a new account 
- [X] User can login to their account
- [x] User can view venues
- [x] User can upload party venue for rent
- [x] User can choose a date and time for event
- [ ] User can book venue for event



**Optional Nice-to-have Stories**

* User can create and customize invitations
* User can discover exactly what stores have a particular decoration

Here's a walkthrough of implemented user stories:

<img src='https://github.com/PartyOverHere/PartyOverHere/blob/main/PartyOverHereLogin.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
<img src='https://github.com/PartyOverHere/PartyOverHere/blob/main/ViewVenues.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
<img src='https://github.com/PartyOverHere/PartyOverHere/blob/main/PartyOverHere.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
<img src='https://github.com/PartyOverHere/PartyOverHere/blob/main/PartyOverHere_UploadVenue.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
<img src='https://github.com/PartyOverHere/PartyOverHere/blob/main/FinalPartyOverHere.gif' title='Video Walkthrough' width='' alt='Final Walkthrough' />



### 2. Screen Archetypes

* Login Screen
   * User can login to their account
* Registration Screen
   * User can create a new account
* Venue Stream Screen
   * User can view venues 
   * User can choose a date and time for event 
* Venue Detail Screen
   * User can book venue 
* Venue Decoration Screen 
    * User can view different theme options 
* Venue Decoration Detail Screen 
    * User can view different decoratioms options   
* Survey Creation Screen
  * User can complete party planning survey
* Profile Screen
  * Users can look at there event history/ payment history and settings.



### 3. Navigation

**Tab Navigation** (Tab to Screen)

* [Login Screen/registration]
* [Home Screen / DashBoard ]
* [Venue Screen]
* [Decoration Screen]
* [Profile Screen]

**Flow Navigation** (Screen to Screen)

* [Login Screen]
   * [=> Home]
   
* [Registration Screen]
   * [=> Home]
* [Home Screen]
   * [=> Survey Screen]
   * [=> Venue Screen]
* [Venue Screen]
   * [=> Venue Detail Screen]
* [Decoration Screen]
   * [=> None]
* [Profile Screen]
   * [=> Event History/Payment History]

## Wireframes

<img src="https://github.com/PartyOverHere/PartyOverHere/blob/main/App_Wireframe1.JPEG" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 
### Models
Homescreen/Dashboard
| Property | Type     |Description|
| -------- | -------- | -------- |
|  get_planning _button  |  pointer to venue screen | Once clicked takes user to avaible venues  |
need_help_button | pointer to survey screen| Once cllicked allows user to take Survey to help them plan their event
venue_idea | pointer to venue screen| Once clicked takes user to a list of all venues in their area 

Venue Screen 
| Property | Type  | Description|
| -------- | -------- | -------- |
| location_button   | pointer to venues    |  Allows the user to pick their location for available venues    |
| date_button| pointer to venues| Allows the user to pick their date for available venues 
| venue_image| file | Allows user to see an image of the venue   |
| venue_price| float| Allows user to view the price of the location 

Venue Detail View 
| Property | Type  | Description |
| -------- | -------- | -------- |
| venue_image    | file    | Allows user to see an image of the venue    |
| venue_name | string | Allows the user to see name of the venue 
| venue_review| string | Allows the user to see an review of the venue 
| venue_location| string | Allows user to see the location of the venue 
| venue_price| float | Allows user to view the price of the location 
| book_venue| pointer to booking screen | Allows user to book venue on the venue detail screen 
| venue_description| string| Allows the user to view a description of the venue 

Decoration Screen (Ideas)
| Property | Type | Description |
| -------- | -------- | -------- |
| decoration_image  | file    | Allows the user to view different decoration ideas   |
| decoration_ideas | string | Allows user to see a brief descrption of the decoration 


Decoration Detail Screen 
| Property | Type     | Description|
| -------- | -------- | -------- |
| decoration_image | file | Allows the user to view different decoration ideas 
| decoration_name| string | Allows the user to see the name of the decoration
| decoration_description    | string    | Allows the user to view a description of the decoration

Profile 
| Property | Type | Description|
| -------- | -------- | -------- |
| dispaly_username   | string  | Allows user to see their username  |
| click_settings | pointer to settings screen | Allows user to view their personal settings for our application
| click_notifications|  | 
| click_event_history| pointer to event history sreen | Allows the user to see all the vents they have viewed while using our app 

Login Screen 
| Property | Type     | Description|
| -------- | -------- | -------- |
| user_username   | string   | Allows the user to type in their user name   |
| user_password | string| Allows the user to type in their password 
| login_button| pointer to the homescreen | Allows the user to access all their information located in the app 


Registration Screen 
| Property | Type | Description |
| -------- | -------- | -------- |
| create_firstname    | string   | Allows user to enter in their first name    |
| create_lastname| string | Allows user to enter their lastname 
| create_password| string| Allows user to create a password 
| create_email| string | Allows user to connect an email to their account 
| createAccount_button| pointer to the homescreen| Allows the user to access all their information located in the app

### Networking
* Login Screen

![](https://i.imgur.com/BkQChkp.png)

* Home Feed Screen
![](https://i.imgur.com/xF0IZb9.png)

* (Read/GET) Query all posts where user is author
* (Create/POST) Create a new like on a post
* ![](https://i.imgur.com/7UJLXkL.png)

* (Create/POST) Create a new comment on a post
* (Delete) Delete existing comment
* Create Post Screen
* Profile Screen
* (Read/GET) Query logged in user object
gith![](https://i.imgur.com/IpZNR4w.png)


