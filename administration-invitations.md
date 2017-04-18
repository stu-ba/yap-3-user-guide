# Invitations

- [Introduction](#introduction)
- [Quick invitation](#quickie)
- [Tedious invitation](#tedious)
	- [Options](#tedious-options)
	- [Amending invitation](#amending)
	- [Recent](#recent)

<a name="introduction"></a>
## Introduction

Inviting potential users via email is trivial, all you have to do is fill out an email and hit **Invite** button.

> {tip} You do not have to invite potential users before creating project, simply use [project creation](/docs/projects#create) interface and Yap will handle everything else.

<a name="quickie"></a>
## Quick invitation

You may quickly invite potential user using modal dialog. To open dialog you need to click on **Invite** button located on right hand side of card header in [user listing](/docs/users#listing) view. 

> {warning} You can not [amend invitation](#amending) using quick invitation. Filling out an email that already exists will result in error.

<a name="tedious"></a>
## Tedious invitation

You may invite potential user using invitation dialog, where you can tick off [options](#tedious-options). Invitation dialog is opened after clicking on **More options** button in model dialog ([quick invitation](#quickie)).

> {note} Inviting an user which is already in system will result in no operation, in addition, if the one is **banned** you will be informed.

<a name="tedious-options"></a>
### Options

Interface provides number of check-boxes with expressive description in form of **Should *something* be set?**.

For example check-box with label *Should user be administrator?* means that invited user is granted administrator privileges if ticked.

> {note} Suppressing emails takes precedence over force resending emails.

<a name="amending"></a>
### Amending invitation
You may amend already issued invitation using [options](#tedious-options). 

An attempt to amend an invitation specified by email will result in:
 - prolonging invitation validity by week (by default) or making it valid forever if adequate option is ticked
 - grant / refuse user administration privileges if adequate option is ticked / not ticked
 - owner of invitation (inviter / invited by) is changed to current user

> {warning} Amending already claimed invitation is not allowed.

<a name="recent"></a>
### Recent

Listing displaying most recent invitations. Invitations that are consumed or expired are not listed.

Table has following rows: 

| table row   | description                                                                     |
|-------------|---------------------------------------------------------------------------------|
| email       | email of potential user                                                         |
| invited by  | name (user-name) of administrator or project leader that created the invitation |
| invited at  | date of creation                                                                |
| updated at  | date of latest update                                                           |
| valid until | hourglass icon representing date until invitation is deemed as valid 			|