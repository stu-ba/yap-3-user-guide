# Invitations

- [Introduction](#introduction)
- [Quick invitation](#quickie)
- [Tedious invitation](#tedious)
	- [Options](#tedious-options)
	- [Prolong invitation](#prolong)
	- [Recent](#recent)

<a name="introduction"></a>
## Introduction

Inviting potential users via email is trivial process, all you have to do is fill out an email and hit **Invite** button.

> {tip} You do not have to invite potential users before creating project, simply use [project creation](/docs/projects#create) interface and Yap will handle everything else.

<a name="quickie"></a>
## Quick invitation

You may quickly invite potential user using modal dialog. To open dialog you need to click on **Invite** button located on right hand side of card header in [user listing](/docs/users#listing) view. 

> {warning} You can not [prolong invitation](#prolong) using quick invitation. Filling out an email that already exists will result in error.

<a name="tedious"></a>
## Tedious invitation

You may invite potential user using invitation dialog, where you can tick off [options](#tedious-options). Invitation dialog is opened after clicking on **More options** button in model dialog.


<a name="tedious-options"></a>
### Options

Interface provides number of check-boxes with expressive description in form of **Should *something* be set?**.

For example check-box with label *Should user be administrator?* means that invited user is granted administrator privileges if ticked.

> {note} Suppressing emails takes precedence over force resending emails.


<a name="prolong"></a>
### Prolong invitation

Filling out email that is already present in invitations table, will result in:
 - prolonging invitation validity by week
 - grant user administration privileges if adequate option is ticked
 - owner of invitation (inviter / invited by) is updated to current user

<a name="recent"></a>
### Recent

Listing displaying most recent invitations. Invitations that are claimed or expired are not listed.

Table has following rows: 

| table row   | description                                                                     |
|-------------|---------------------------------------------------------------------------------|
| email       | email of potential user                                                         |
| invited by  | name (user-name) of administrator or project leader that created the invitation |
| invited at  | date of creation                                                                |
| updated at  | date of latest update                                                           |
| valid until | asd