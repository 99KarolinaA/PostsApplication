# PostsApplication

### Two applications for posting. Made using ASP.NET Core.
#### The *ListingApp* is an application that will be used by anyone while *ListingsAdminApplication* is an application that will be used only by the administrator. ####
The administrator application communicates with the main listing application via HTTP protocol. 
Below are preview images of the user interface.

Everyone has access to the start page where all the posts are displayed and can be filtered by category, location and price. The search functionality filters the posts by name or description.

![homepage](https://user-images.githubusercontent.com/73672408/159190317-ef970b43-1040-40dc-bbae-0da899dc4af3.png)
<p align="center">
<i> Start page </i>
</p>
<br>

In order to register, the user needs to pay 5$. The online payment is made with the integration of the **Stripe service**.

![register](https://user-images.githubusercontent.com/73672408/159190903-5686f234-5e17-4047-999c-9914dbe5a5dd.png)
<p align="center">
<i> Register </i>
</p>
<br>

The registered user can create new posts. But one post can be added to the start page, if it is accepted by the administrator.
After creating the post, the administrator receives an email that he has a new post for validation. The **MailKit library** is used for sending emails.

The administrator uses the **administrator application** where he has access to all the posts and where he approves or disapproves the posts.

![administrator](https://user-images.githubusercontent.com/73672408/159191005-02c1b46b-d357-4190-acce-81ea64ae93aa.png)
<p align="center">
<i> Administrator application </i>
</p>
<br>

Also the administrator can export an excel file with weekly approved posts using **ClosedXML library**.

![export](https://user-images.githubusercontent.com/73672408/159192184-0f204d88-2950-4e9d-a93a-143c6f9dc8ff.png)
<p align="center">
<i> Export a file </i>
</p>
<br>

After the administrator validates a given post, the user receives an email for the post status. (approved or disapproved).

![mail](https://user-images.githubusercontent.com/73672408/159191875-021ac0d3-f16d-4159-8e26-26dadb8a2d78.png)
<p align="center">
<i> Email example </i>
</p>
<br>

А registered user has a separate view of all his posts and their statuses. The user can modify or delete his posts and add posts to his wishlist.
Also he can use the public chat to communicate with all the users of the application with the help of **ASP.NET Core SignalR library**.

![image](https://user-images.githubusercontent.com/73672408/159192394-f581e95b-9b64-4883-af2e-0013eb4740f2.png)
<p align="center">
<i> Public chat </i>
</p>
<br>

