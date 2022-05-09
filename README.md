# YAGPDB-Dev-Journal

Source code for very simple development blog/journal capable of tracking current progress and future goals. 
It uses YAGPDB's ticket system, so be sure to enable it first!
My custom welcome message can be found in ticket-message.yag file

Enjoy ^^

---

**DONE**

Create a bot command capable of tracking the development of certain things.

---

**TODO**

Add ability to track how long have you been working on a task.

---

## Installation

As usual, there are instructions describing where to put the script and which trigger to use on the pages corresponding to the individual commands. 

## Features

`-devblog create new`

| Trigger | Command |
| ------- | ------- |

> Returns a new ticket channel created only for that person where he/she could write everything that person has done so far. It also posts a help message.



`<d>{{VALUE}}`

| Trigger | Starts with |
| ------- | ----------- |

> Trigger for adding description where {{VALUE}} is user input.
> After 5 sec, input will be saved and deleted.



`<g>{{VALUE}}`

| Trigger | Starts with |
| ------- | ----------- |

> Trigger for adding goal where {{VALUE}} is user input.
> After 5 sec, input will be saved and deleted.



`-devblog add post`

| Trigger | Command |
| ------- | ------- |

> If <d> and <g> fields are empty it will display an error message.
> Otherwise, it will upload user inputs into the database and display them in the embedded form.
> After 5 sec the Trigger will be deleted.



`-devblog show all`

| Trigger | Command |
| ------- | ------- |




> Will display every post that the user had made so far.

---

## ONLY FOR DEBUGGING PURPOSES

`-devblog -d rtest`

| Trigger | Command |
| ------- | ------- |

> Will display info about:
>   -number of stored posts
>   -staged description
>   -staged goal
> After 2 sec the Trigger will be deleted 
> After 30 sec the Response will be deleted 



`-devblog -d reset`

| Trigger | Command |
| ------- | ------- |

> Resets the database


