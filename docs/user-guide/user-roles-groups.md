# User Roles and Groups

## Basics

Permissions are based on groups and levels. Users are assigned to groups and each group has a level. Commands can be run by users who have the minimum level required to use the command.

## Groups

Spunky Bot has several user groups, each serving a specific purpose.

Level | Group       | Description
----- | ----------- | -----------
100   | headadmin   | The **Head Admin** is the highest level of authority. A Head Admin has access to all commands and is assigned to the server owner.
90    | superadmin  | The **Super Admin** is a representative of the Head Admin and has access to all commands including the commands used in the server setup.
80    | senioradmin | **Senior Admins** are the highest admins. They have access to most commands except the commands used in server setup.
60    | fulladmin   | **Full Admins** have less authority than Senior Admins, but still have access to punishment commands such as `!ban`.
40    | admin       | **Admins** are the first level of administrators. Their hardest punishment is the command `!kick`.
20    | mod[erator] | **Moderators** are the first step to becoming an admin. They can only `!warn` users.
2     | reg[ular]   | **Regulars** are not admins or moderators, but your loyal server population. You would only give regular status to members of your community.
1     | user        | A **user** is like a self-appointed regular.

New players can use the `!register` command to get user status. Users have a few commands, but gain extra privileges compared to one-time visit players.

## User Management

Users can be added to any group by privileged admins with the `!putgroup` command.

Useful Commands:

* `!register` - Register yourself as a basic user
* `!makereg <player>` - Used by admins to add a user to the regular group
* `!unreg <player>` - Used by admins to remove a user from the regular group
* `!putgroup <player> <group>` - Used by admins to add a user to the group
* `!ungroup <player>` - Used by admins to remove all levels from the user

Senior Admins can add and remove the admin level of players within the level **User** to **Full Admin**.

!!! warning "Security"
    A Senior Admin cannot remove the admin level of another Senior Admin.
    Only Super Admins can do that.

In the following example the player 'Adam' is added to the **moderator** [group](#groups):

```bash
!putgroup Adam mod
```

!!! note
    Users can only be a member of one group.
