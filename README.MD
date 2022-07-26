README
Requirements for TODO Application

1. Users
   Users can register for an account.
   Users can log in to the app and log out from the app.
   When a user registers for an account they provide the following information:
   First Name
   Middle Name\*
   Last Name
   Email Address
   Password
   The user’s registration flow is as follows:
   When a user comes to your site, they will register and provide all the information required.
   The app must send an email to validate the email address.
   Only users with a validated email address can log in to the app.
   Users may request a new validation email be sent to them.
   The request must be throttled i.e., only one email can be sent by the system every 15 minutes.
   Each user in the system must have a unique email address.
   A user can change their email address after registration if it is a unique email address. The new email address must be validated before making the switch. An email should also be sent to the old email address for user confirmation.

2. Lists
   Users can create one or more lists.
   A default list is created for the user when they register.
   A list has the following attributes:
   Name
   Created date and time
   Last updated date and time
   A user can rename their list.
   The list is private by default. No other user in the system can see a user’s lists.

3. Task
   Users can create tasks.
   The task must be in exactly one list.
   Task has the following attributes:
   Summary (50 chars)
   Task (you determine the size of this field) _
   Due Date_
   Tags*
   Priority (High, Medium, Low)
   Attachments*
   Reminders\*
   Created date and time
   Last updated date and time
   A task can be moved from one list to another.
   The task is private by default. No other user in the system can see a user’s Tasks.
   Deleting a Task must delete all related items such as attachments & comments. Tags should not be deleted.
   A Task can be in one of the following states:
   TODO
   COMPLETE
   OVERDUE
   When a user updates Task’s due date, an OVERDUE task must reset its state.

4. Attachments
   The task can have 0 or up to 5 attachments.
   Attachments can be any file.
   Attachments can be added or removed from the Task.
   The attachment has the following attributes:
   Name
   Size
   Date Attached
   TBD

5. Tags
   A task can have 0 or up to 10 tags
   Tags are user-defined i.e., each user may have a unique set of tags.
   Same tags can be used in multiple lists.
   A user can rename a tag.
   A tag has the following attributes:
   Name
   Created date and time
   Last updated date and time
   Each user has their own set of tags.
   Comments
   A Task can have 0 or more Comments. There is no limit to how many comments a Task can have.
   A Comment has the following attributes:

6. Comment
   Created date and time
   Last updated date and

7. Reminders
   A Task may have 0 or up to 5 reminders.
   A Reminder has the following attributes:
   Date and Time for a reminder
   Created date and time
   Last updated date and time
   A Reminder is sent to the email address in the account profile.
