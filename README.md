# OneManArmy

## Project Description

The One Man Army mobile application provides a platform for small business owners to display their expertise and advertise their services. Additionally, it enables individuals who lack certain skill sets to locate competent professionals and outsource work to them.
______________________________________________________________

## Recent Updates
* Quick fix for passing the wrong ID through intent
* Receipts now dynamically populate necessary fields, hotfix on ownderdash
* Pulling currently logged in user in the dashboard activity and then passing it as an OwnerModel() to all the other activities. Each activity now has access to the info of the currently logged in user 
* Search implemented 
* Created a FAQ button with questions and answers for client side 
* Second registration screen working now, routing to profile setup 

## Technological Stack:

Kotlin

Android Studio

FireBase


## Project Setup

This app was created using Android API 30, and the platform that is being emulated is Google Pixel 3, so it is suggested that the same API and platform is used.


## About the App:

OneManArmy is an app created for sole proprietors to manage their businesses and for usual users to find a service they need. This app lets business owners register their businesses in the app, find new clients, manage their appointments, and send their clients the receipts of finished work.


## Main Features:

### Business Owner:

1) Ability to view and manage appointments with clients
2) Ability to create receipts for completed orders
3) Ability to send receipts to clients as proof of finished work
4) Ability to set up a profile with a phone number, picture, and a list of skills

### Client:

1) Ability to find sole proprietors by their names
2) Ability to make appointments with business owners


## Implementation:

The app uses FireBase for back-end management. All user-related data is stored in FireBase and pulled to the front end by request.

There are two separate dashboards for the business owner and client. The main difference is that the client's dashboard has a "Search" page instead of a "Receipt Creator."

On the "Appointments" page, clients and business owners can make appointments with each other. The dates are demonstrated in the calendar, the Material-Calendar library was used which allowed creation of appointments for specific days and times and track them. Days with the appointments on them are highlighted on the calendar.

On the "Account" page, the client can edit his basic information: name, e-mail, phone number, and address. From the business owner's side, the "Profile" page is similar, but it is possible to change the name of their business and add their skills.

On the "Receipt Creator" page, the business owner can create receipts for the orders that they complete. We made our receipt creator work in such a way that it gets saved as a PDF. After that, the business owner can use it either for keeping track of itemized deductions or for sending it to the clients as proof of finished work via e-mail. By default, the receipts are saved in the Downloads folder.

On the "Search" page, the client can look for the service providers; from there, they can access their profiles to make an appointment. The filter used for the search is the business owner's name.


## Issues:

1) Planned to use the OpenCV library for "Receipt Creator," so that there would be no need to input all the receipt information manually. Complications came up and the feature implementation was put on standby until further notice.
