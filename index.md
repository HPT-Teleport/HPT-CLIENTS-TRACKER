## Overview

**Note** that all of the examples and information displayed in this documentation are made up and do not use actual client information. The documentation guides the users about various aspects of this application.

 <br>
 This application utilizes various technologies, including:

- [Meteor](https://www.meteor.com/) for Javascript-based client and server code implementation.
- [React](https://reactjs.org/) for component-based UI implementation and routing.
- [Bootstrap UI React](https://react-bootstrap.github.io/) CSS Framework for UI design.
- [MongoDB](https://www.mongodb.com/) Production database

<br>

## Deployment

The application is deployed in the HPT organizations' server and can only be accessible within the local network.

<br>

## User Guide

This section provides a walkthrough of the HPT Clients Tracker user interface and its capabilities.
<br><br>

### Landing Page

The landing page is the first thing the users see upon visiting the root URL of the site.

Users are prompted to enter their username and password for login. Only users with the admin privilege can register new accounts.

![screenshot of the landing page](doc/landingwithoutlogin.png)

<br>

### Home Page

Upon logging in successfully, the home page is displayed. It contains frequently used information regarding the company and links to other internal websites. Additionally, it gives users the ability to modify their password.

![screenshot of the home page](doc/landingwithlogin.png)

<br>
<br>

### Customer Page

To access the Contact information, navigate to the Contacts menu in the navigation bar. The dropdown menu for Contacts contains two options - Customers and Providers. Selecting either option will redirect you to the respective page, where you can view the details of all active customers or providers. It's important to note that Providers may include both satellite and internet service providers. The page grants users the ability to modify, delete, and review customer/provider information.

![screenshot of active customer](doc/activecustomer.png)
<br>
<br>

To **modify** the customer information, select the "Edit" button. This will redirect you to the appropriate page. Utilize the form provided to make the necessary changes. Additionally, users can mark the customer as inactive on this page.

![Update Customer ScreenShot](doc/editcustomer.png)

To **add** a new customer, click on the "Add Customer" button located at the bottom of the page or simply navigate to the Admin dropdown in the navigation bar and click on "Add Customer". Fill out the required information and submit the form to create a new customer record.

![Add Customer ScreenShot](doc/addnewcustomer.png)

**Note** that if you deselect the active checkbox in the edit customer or edit provider page, the customer or provider will be marked as inactive and will no longer be displayed on the customer or provider page. To access inactive customer or provider details, navigate to the "Archive" page.

<br>

**Note** that the Providers page closely resembles the Customers page and serves to store the contact information of various vendors including Satellite Controllers and Internet Service Providers.

<br>

Below is the screenshot of the "Provider" page

<br>

![Provider Page ScreenShot](doc/activeproviders.png)

### Services Page

Select the "Services" tab on the navigation bar to access a list of active services. This page will only display services associated with active customers. Users can access the active customers on the left sidebar to review the services they are currently running.

![screenshot of the services Page](doc/services.png)
**Add Services**
<br>
To add a new service:
Navigate to the "Services" page and select the "Add Services" button or access it from the "Admin" dropdown in the navigation bar.
Complete the form with the required information, and upload any necessary files if desired.
Once complete, submit the form to finalize the process.

![screenshot of the addservices Page](doc/addnewservice.png)

**Individual Service**
<br>
By selecting the customer button on the left sidebar, the application will display the services associated with that specific customer
<br>
On this page, users have the ability to view and archive the service. Additionally, users have the option to add the service to Spectras, an external device that is utilized for monitoring services. The application interacts with the device through a REST API. Once added to the Spectras application, users can access the latest graph of the service. This feature allows for quick and efficient monitoring of the service status and aids in troubleshooting during issues and outages.

![screenshot of the individual services Page](doc/individualservice.png)

<br>
Click on the "Show Details" button to view the service's details.

![screenshot of the show details page](doc/servicedetails.png)

<br>
To add the TX/RX services to LPT Spectras, select the "Add to Spectras" button. After successfully adding the service to Spectras, the button label will change to "Remove From Spectras." If you wish to remove the service from Spectras, select the "Remove From Spectras" button.

![Screenshot of add to spectras page](doc/successfuladdtospectras.png)

<br>
<br>
Please take note that the "Archive" button on the service page will deactivate the service and remove its snapshot from Spectras. Nevertheless, information on inactive services can still be viewed on the "Archives" page.

<br>
<br>

Click on "Display Plot" button to view the latest updated graph of the service.

![screenshot of the plot](doc/spectrasplot.png)

### Antennas

Select the "Antenna" button on the navigation bar to view, edit, and archive existing antennas.

![screenshot of the antenna page](doc/addantennas.png)

To add a new antenna, navigate to the "Antenna" page and select the "Add Antenna" button or access it from the "Admin" dropdown in the navigation bar.

![screenshot of the antenna page](doc/addantenna-1.png)

<br>
<br>

### Archive

To access information on inactive entities such as Customers, Providers, Services, and Antennas, navigate to the "Archive" page via the navigation bar. Once on the page, simply select the desired entity and click on "Find" to display the related information

![screenshot of the archive page customer](doc/archiveantenna.png)

![screenshot of the archive page](doc/archiveservice.png)

**_To reactivate an entity, simply click on the "Activate" button._**

### Admin

The "Admin" dropdown button on the navigation bar provides access to the functionality for adding customers, providers, services, and antennas. Additionally, it includes options for the administrator to manage user accounts and audit customers associated with a particular antenna.

![screenshot of the Admin page](doc/admindropdown.png)

<br>
The "Manage Account" page is accessible only to users with an "Admin" role and allows them to delete/register users. This page is not visible to users with different roles.

![screenshot of the manage account page](doc/manageaccounts.png)

<br>
Users with non-admin role cannot manage accounts
<br>

![screenshot of the manage account page for non admin](doc/regularuser.png)

<br>

The "Audit Customer" page enables users to view a list of customers and the services associated with a particular antenna.

![screenshot of the get customers page](doc/auditcustomer.png)

<br>

### SignOut

To sign out, simply click on the username located at the top right of the navigation bar and select "Sign Out"

![screenshot of signout page](doc/signout.png)

## Contact Me

**HPT Clients Tracker** is designed, implemented, and maintained by [Ujjwal Gautam](mailto:ugautam@hawaiiteleport.com)

<br><br><br><br>
