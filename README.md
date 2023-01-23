# IAM
#### Here are the step-by-step instructions on how to create an IAM user in AWS using the AWS Management Console

1. Sign in to the AWS Management Console using your root account or an IAM user with the appropriate permissions.

![aws console](/aws/)

In the navigation menu, choose "Services" and then select "IAM". This will take you to the IAM dashboard.

In the navigation menu, choose "Users". This will show you a list of all the existing IAM users.

On the Users page, choose the "Add user" button. This will take you to the "Add user" page.

In the "Add user" page, enter a name for the new user in the "User name" field.

Select the type of access for the new user. If you want the user to have access to the AWS Management Console, select "AWS Management Console access". If you want the user to have programmatic access, select "Programmatic access".

If you selected "AWS Management Console access", you will be prompted to set a password for the user. You can also choose to have AWS generate a random password for you.

If you selected "Programmatic access", you will be prompted to create an access key for the user. An access key consists of an access key ID and a secret access key, which are used to make programmatic requests to AWS services.

In the "Permissions" section, you can either add the user to an existing group, or create a new group with specific permissions. You can also give the user permissions by attaching policies directly to the user.

On the review page, you can review the user's name, access type, permissions, and password or access key. When you're ready, choose "Create user".

Once the user is created, you will be taken back to the Users page, where you can see the new user listed. You can then use this user to access the AWS services that you have granted it permissions to.

Note that you can also create roles and groups, assign permissions and policies to them and then assign them to the user. This way you can give permissions to multiple users at once and also manage them centrally.

 

Here are the steps to create an IAM role and group, and then assign them to an IAM user:

Go to the IAM dashboard in the AWS Management Console.

In the navigation pane, choose "Roles". This will show you a list of all the existing IAM roles.

Choose the "Create role" button. This will take you to the "Create role" page.

In the "Create role" page, select the AWS service that will use this role. You will be prompted to select the permissions that you want to grant to this role.

In the "Permissions" section, you can either attach existing policies or create new policies to define the permissions for the role.

On the review page, you can review the role's name, permissions, and trust relationships. When you're ready, choose "Create role".

Once the role is created, you can now create a group.

In the navigation pane, choose "Groups". This will show you a list of all the existing IAM groups.

Choose the "Create new group" button. This will take you to the "Create new group" page.

In the "Create new group" page, enter a name for the new group and a description if desired.

In the "Permissions" section, you can either attach existing policies or create new policies to define the permissions for the group.

On the review page, you can review the group's name, permissions, and attachments. When you're ready, choose "Create group"

Now you can assign the created role and group to the user

In the navigation pane, choose "Users". This will show you a list of all the existing IAM users.

Choose the user you want to assign the role and group to.

In the "Permissions" tab, choose "Add permissions"

In the "Add permissions" page, choose "Attach existing policies directly"

Select the group and role created previously and choose "Next: Review"

Review the changes and choose "Add permissions"
