ROLEASSIGN
----------

RoleAssign introduce the assign roles permission. While editing a user's account information, a user with this permission will be able to select roles for the user from a set of available roles. Roles available are configured by the site administrator.

Please always use this project's issue tracker <http://drupal.org/project/issues/roleassign> to report bugs or to request features or support.

This module is sponsored by Webbredaktören <http://www.webbredaktoren.se/>.


BACKGROUND
----------

It is possible for site administrators to delegate the administration through the administer users permission. But the administer users permission doesn't include the right to assign roles to the user. That is necessary if the delegatee should be able to administrate the user accounts without intervention from a site administrator.

To delegate the assignment of roles, site administrators have had until now no other choice than also grant the administer access control permission. But that is not advisable. The administer access control permission is very far-reaching, giving rights to access all roles, and worse, to grant any rights to any role. That can be abused by the delegatee, who can assign himself all rights and thereby take control over the site.

This module solves this dilemma by introducing the assign roles permission. While editing a user's account information, a user with this permission will be able to select roles for the user from a set of available roles. Roles available are configured by the site administrator.


CONFIGURATION
-------------

1. Go to administer » access control. Under the permissions tab, grant assign roles permission to those roles that should be able to assign roles to other users. Notice that besides the assign roles permission, these roles also must have the administer users permission.

2. Go to administer » access control. Under the RoleAssign tab, select those roles that should be available for assignment by users with assign roles permission.

3. Go to administer » users. For each user that should be able to assign roles, click on the corresponding edit link, and assign the user a role with both the assign roles and the administer users permissions.


USAGE
-----

1. Log in as a user with both the assign roles and the administer users permissions.

2. To change the roles of a user, go to administer » users and click on the user's edit link. Review the assignable roles and change the as necessary.


LICENSE
-------

RoleAssign: Copyright © 2006 Thomas Barregren.

RoleAssign is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

RoleAssign is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.>>>>>>> 1.1.1.1.2.4

$Id$