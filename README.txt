ROLEASSIGN
==========

RoleAssign lets site administrators delegate assignment of selected
roles.

RoleAssign introduce the 'assign roles' permission. While editing a
user's account information, a user with this permission will be able to
select roles for the user from a set of available roles. Roles available
are configured by users with the 'administer access control' permission.

Please always use this project's issue tracker
<http://drupal.org/project/issues/roleassign> to report bugs or to
request features or support.

This module is sponsored by Webbredaktoren <http://www.webbredaktoren.se/>.


BACKGROUND
----------

It is possible for site administrators to delegate the user
administration through the 'administer users' permission. But that
doesn't include the right to assign roles to users. That is necessary if
the delegatee should be able to administrate user accounts without
intervention from a site administrator.

To delegate the assignment of roles, site administrators have had until
now no other choice than also grant the 'administer access control'
permission. But that is not advisable, since it gives right to access
all roles, and worse, to grant any rights to any role. That can be
abused by the delegatee, who can assign himself all rights and thereby
take control over the site.

This module solves this dilemma by introducing the 'assign roles'
permission. While editing a user's account information, a user with this
permission will be able to select roles for the user from a set of
available roles. Roles available are configured by users with the
'administer access control' permission.


INSTALL
-------

1. Copy the entire 'roleassign' directory, containing the
'roleassign.module' and other files, to your Drupal modules directory.

2. Log in as site administrator.

3. Go to the administration page for modules and enable the module.


CONFIGURATION
-------------

1. Log in as site administrator.

2. Go to the administration page for access control and grant 'assign
roles' permission to those roles that should be able to assign roles to
other users. Notice that besides the 'assign roles' permission, these
roles also must have the 'administer users' permission.

3. Go to the administration page for role assign and select those roles
that should be available for assignment by users with 'assign roles'
permission.

4. For each user that should be able to assign roles, go to the user's
account and select a role with both the 'assign roles' and the
'administer users' permissions.


USAGE
-----

1. Log in as a user with both the 'assign roles' and the 'administer
users' permissions.

2. To change the roles of a user, go to the user's account and review
the assignable roles and change them as necessary.


LICENSE
-------

RoleAssign. Copyright (C) 2006 Thomas Barregren.

RoleAssign is free software; you can redistribute it and/or modify it
under the terms of the GNU General Public License as published by the
Free Software Foundation; either version 2 of the License, or (at your
option) any later version.

RoleAssign is distributed in the hope that it will be useful, but
WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
Public License for more details.

You should have received a copy of the GNU General Public License along
with this program; if not, write to the Free Software Foundation, Inc.,
51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.

$Id$