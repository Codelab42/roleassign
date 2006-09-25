DESCRIPTION
----------- 

Roleassign lets site administrators delegate assignment of selected 
roles. 

It is possible for site administrators to delegate the administration 
through the 'administer users' permission. But the 'administer users' 
permission doesn't include the right to assign roles to the user. That 
is necessary if the delegatee should be able to administrate the user 
accounts without intervention from a site administrator. 

To delegate the assignment of roles, site administrators have had until 
now no other choice than also grant the 'administer access control' 
permission. But that is not advisable. The 'administer access control' 
permission is very far-reaching, giving rights to access all roles, and 
worse, to grant any rights to any role. That can be abused by the 
delegatee, who can assign himself all rights and thereby take control 
over the site. 

This module solves this dilemma by introducing the 'assign roles' 
permission. While editing a user's account information, a user with this 
permission will be able to select roles for the user from a set of 
available roles. Roles available are configured by the site 
administrator. 

This module is sponsored by Webbredaktoren <http://www.webbredaktoren.se/>. 


CONFIGURATION
------------- 

1) Go to 'administer > access control'. Under the permissions tab, grant 
'assign roles' permission to those roles that should be able to assign 
roles to other users. Notice that besides the 'assign roles' permission, 
these roles also must have the 'administer users' permission. 

2) Go to 'administer > access control'. Under the role assign tab, 
select those roles that should be available for assignment by users with 
'assign roles' permission. 

3) Go to 'administer > users'. For each user that should be able to 
assign roles, click on the corresponding 'edit' link, and assign the 
user a role with both the 'assign roles' and the 'administer users' 
permissions. 


USAGE
----- 

1) Log in as a user with both the 'assign roles' and the 'administer 
users' permissions. 

2) To change the roles of a user, go to 'administer > users' and click 
on the user's 'edit' link. Review the assignable roles and change the as 
necessary. 


BUG REPORTS, FEATURE REQUESTS AND OTHER ISSUES 
---------------------------------------------- 

This module is created and maintained by Thomas Barregren. 

Please use the roleassign project page 
<http://drupal.org/project/roleassign> for sending bug reports and 
feature requests. For other issues, please send an e-mail directly to 
Thomas Barregren <mailto:thomas@webbredaktoren.se>. 


LICENSE
------- 

Roleasign version 1.0. Copyright (C) 2006 Thomas Barregren. 

Roleassign is free software; you can redistribute it and/or modify it 
under the terms of the GNU General Public License as published by the 
Free Software Foundation; either version 2 of the License, or (at your 
option) any later version. 

Roleassign is distributed in the hope that it will be useful, but 
WITHOUT ANY WARRANTY; without even the implied warranty of 
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General 
Public License for more details. 

You should have received a copy of the GNU General Public License along 
with this program; if not, write to the Free Software Foundation, Inc., 
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.

$Id$
