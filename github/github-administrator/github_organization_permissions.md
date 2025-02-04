# Github Permissions

## Repository permission levels

You can customize access to a given repository by assigning permissions. There are five repository-level permissions:
- **Read**: Recommended for non-code contributors who want to view or discuss your project. This level is good for anyone that needs to view the content within the repository but doesn't need to actually make contributions or changes.
- **Triage**: Recommended for contributors who need to proactively manage issues and pull requests without write access. This level could be good for some project managers who manage tracking issues but don't make any changes.
- **Write**: Recommended for contributors who actively push to your project. Write is the standard permission for most developers.
- **Maintain**: Recommended for project managers who need to manage the repository without access to sensitive or destructive actions.
- **Admin**: Recommended for people who need full access to the project, including sensitive and destructive actions like managing security or deleting a repository. These people are repository owners and administrators.

You can give **organization members**, **outside collaborators**, and **teams** different levels of access to repositories owned by an organization. Each permission level progressively increases access to a repository's content and settings. Choose the level that best fits each person or team's role in your project without giving more access to the project than necessary.

After you create a repository with the correct permissions, you can make it a template so that anyone who has access to the repository can generate a new repository that has the same directory structure and files as your default branch.

## Team Permission Levels

Teams provide an easy way to assign repository permissions to several related users at once. Members of a child team also inherit the permission settings of the parent team, providing an easy way to cascade permissions based on the natural structure of a company.
There are two levels of permissions at the team level:


| Permission level	| Description                                                            |
| ----------------- | ---------------------------------------------------------------------- |
| Member	        | Team members have the same set of abilities as organization members    |
| Maintainer	    | Team maintainers can do everything team members can plus:                                                                  
- Change the team's name, description, and visibility.              
- Request that the team change parent and child teams.              
- Set the team profile picture.                                     
- Edit and delete team discussions.                                 
- Add and remove organization members from the team.                
- Promote team members to also have the team maintainer permission. 
- Remove the team's access to repositories.                         
- Manage code review assignment for the team.                       
- Manage scheduled reminders for pull requests.                     |

An organization owner can also promote any member of the organization to be a maintainer for a team.

## Organization permission levels

There are multiple levels of permissions at the organizational level:

| Permission level	| Description |
|------------------ | ----------- |
| Owner	| Organization owners can do everything that organization members can do, and they can add or remove other users to and from the organization. This role should be limited to no less than two people in your organization.|
| Member | Organization members can create and manage organization repositories and teams. |
| Moderator | Organization moderators can block and unblock nonmember contributors, set interaction limits, and hide comments in public repositories that the organization owns. |
| Billing manager |	Organization billing managers can view and edit billing information. |
| Security managers	| Organization security managers can manage security alerts and settings across your organization. They can also read permissions for all repositories in the organization. |
| Outside collaborator | Outside collaborators, such as a consultant or temporary employee, can access one or more organization repositories. They aren't explicit members of the organization. |

## Enterprise permission levels

| Permission level | Description |
| -----------------| ----------- |
| Owner	| Enterprise owners have complete control over the enterprise and can take every action. |
| Member | Enterprise members have the same set of abilities as organization members. |
| Billing manager | Enterprise billing managers can only view and edit your enterprise's billing information and add or remove other billing managers. |