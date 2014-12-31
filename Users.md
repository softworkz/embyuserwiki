Most operations within Media Browser are based around users. Users can have their own personalized media libraries, user data, recommendations, security settings, and more.

Users are managed within the server dashboard by navigating to **Users**. The page will display as many as three kinds of users: Local Users, [Guests](Guests) and [Pending Invitations](Guests).

## Local Users

Local users are displayed under the user heading. These are users that you've created in the server dashboard.

![](images/server/users1.png)

A local user will be displayed with a cloud if it is linked to [Media Browser Connect](Media Browser Connect). 
![](images/server/users6.png)

Linking a user to Media Browser Connect will enable an easier sign in process that doesn't require the user to know your server's ip address. For more information, see [Media Browser Connect](Media Browser Connect).

## Guests

Guests are users that you've invited using [Media Browser Connect](Media Browser Connect).

For more information, see [Guests](Guests).

## Adding a User

To add a local user, click the + button within the Users heading:

![](images/server/users7.png)

You'll then be taken to the new user page page. The only required field is a user name:

![](images/server/users8.png)

In addition you can also configure library and channel access, and this can easily be changed later:

![](images/server/users9.png)

## User Access

Access controls allow you to specify what libraries, channels and devices a user can utilize. To manage access for a user, navigate to the server dashboard -> **Users** -> **Click User** -> **Access**. 

### Device Access

Device access allows you to configure the devices a user is allowed to sign in from. By default, users can use any device.

![](images/server/users17.png)

**Important notes about device control**: This only applies to devices that can be uniquely identified and will not prevent access from a browser. Also, filtering devices for a user will prevent them from being able to sign-in with a new device until it is enabled from this page.

## Parental Controls

There are a number of tools at your disposal to restrict content from users. To manage parental controls for a user, navigate to the server dashboard -> **Users** -> **Click User** -> **Parental Control**. 

The simplest way is to set the max parental rating for a user.

### Parental Controls via Ratings:

![](images/server/users13.png)

This value will not affect unrated content, but there are additional options to control that as well:

![](images/server/users14.png)

### Parental Controls via Tags:

In addition, you can also restrict content containing certain tags:

![](images/server/users15.png)

For more information on tags and how to configure them, see [Metadata manager](Metadata manager).

### Parental Controls via Access Schedule:

Access schedules allow you to control the days and times during the week in which a user is allowed access to the server:

![](images/server/users16.png)

To create a schedule, click the **Add Schedule** button. Once a schedule is assigned, the user will only be able to access the server during those listed times.

**Note**: Access schedules cannot be created on administrator accounts.


## Deleting a User

To delete a user or guest, simply click the dot menu button and select Delete:

![](images/server/users5.png)