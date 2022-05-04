---
title: "Tasks and Automation"
teaching: 20
exercises: 2
questions:
- "What are tasks?"
- "How do you manage and create new tasks?""
- "How do you run tasks?""

objectives:
- "Explain how to create, manage, edit and run tasks"
- "Successfully create and run a new task"
- "Successfully export a task"

keypoints:
- "MarcEdit tasks are a way to automate a series of functions"
- "Tasks can consist of any type of function offered in the MarcEditor tools"
---

# Tasks and Automation
Very often we deal with a set of MARC records where the data needs the same or very similar approach. A good example are electronic resources where the resource link in the MARC field 856 will need the proxy stem for that institution. Another example are adding RDA content, carrier, and media terms and codes to your records. In short, MARC records need to fit both national standards and local best practices and hence it is necessary to manipulate MARC data to fit these standards and practices. In the previous lessons we saw this at the scale of one change at a time. In this lesson, we move to seeing how to string together these changes.

Indeed, a MarcEdit task is a series of changes to MARC data that occur in the sequence they are entered in the task. One could think of tasks as a mini script of sorts that string together different MarcEditor tools that manipulate MARC data in some way. All tasks are created, managed, and run in the MarcEditor. In this way, tasks are another way to manipulate data in the MarcEditor and are an extension of the other tools offered in the MarcEditor.

## What are tasks?
A task is a series of MarcEdit functions to manipulate data. In the previous lessons, we've run one function at a time. Tasks string those functions together to run at once. Tasks run each function one after another. As such, it is important to think about which tasks follow other tasks. For instance, if you want to add a proxy and the MARC data already has a proxy that you need to delete, your task has to account for that and remove the old proxy before adding a new one.

Tasks are managed through the Task Manager in the MarcEditor. To access the Task Manager, go to Tools and then Manage Tasks in the top level menu. This will open the new tasks window.

In this window, you will see any tasks that you have created previously. You will see the name that you gave those tasks, the path or where those files are saved on your local computer, a shortcut, and a description. At the bottom of this window you will also have two options "Task Actions" and "Manage Existing Tasks".

Task Actions include:
- New Task: This will create a new task.
- Clone: This will duplicate an existing task.
- Delete: This will remove a task.
- Edit: This will allow you to edit an existing task.
- Rename: This is how to give a different name to an existing task.

Manage Existing Tasks include:
- Assign to Group: You can put tasks into different categories or groups.
- Assign keystrokes: You can assign shotcut keys to tasks.
- Backup all tasks: Make sure your work is backed up.
- Delete Task Group: This is to remove an existing group.
- Export Task File: This will save a task to your local computer.
- Import Task File: This will bring in a task from your local computer.
- New Task Group: This will allow you to create a new group.
- Relink tasks: This will allow you to relink tasks.
- Remove From Group: This will let you remove a task from a group.
- Rename Group: This will allow you to rename a group.

The difference between these two actions lists might seem confusing at first. Task actions allow you to work with a particular task in terms of creating and managing one specific task at a time. The Manage Existing Tasks menu allows you to create and manage groups, exporting and importing, and assigning keyboard shortcuts to tasks.

Tasks don't have to be categorized in groups or be linked to keyboard shortcuts. This is up to the users and their preference for how they organize their task workspace.

## Create and a new task
To create a task in the MarcEditor, Go to Tools in the top level menu and then Manage Tasks. In the Task Actions menu, select "New Task". This opens the task list window where you will see the name you gave your task, a description, tasks, and actions.

Please note that you will see the name of the task and can type something different in this window. However, these changes only for the name won't take effect. To change the name of a task, you need to go to Task Actions and select Rename task.

You can add or update a description in this task list window. The box in the middle will list the fuctions (or tasks) for this particular task. If there are none, this window will be empty.

Actions include:
- Add: Add a new function or task
- Duplicate: Clone a function or task already in the list
- Delete: Delete a function or task
- Edit: change an existing function or task

You can add a new task by clicking on the plus button. You can add any type of function available in the MarcEditor Tools and Edit Shortcuts menu options. This includes the RDA Helper, build a new field, change the case of a MARC field, or generate cutters. You can even include a list of functions (tasks) from another Task.

Click on save at the left bottom corner of the Task List window to save your Task. From there you can close the Task Manager window. To run a task, go to Tools, then Assigned Taks, Current Tasks.

If you have a lot of Tasks, it does help to assign them to groups to more easily find what you need. If you don't use Groups, the Task Manager will list all your Tasks in alphabetical order and it might be difficult to see them on especially on small screens such as laptops.

>## Create and run a new Task that runs the RDA helper and removes 9XX fields
>
>1. .
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Manage Tasks
> > 3. In the Task Manager window, in Task Actions, select New Task
> > 4. Click Select.
> > 5. Name your Task
> > 6. In the Task List window, you can describe this task.
> > 7. Click on the plus button and add RDA Helper.
> > 8. Click on the plus button and add a new Add Delete Task Field
> > 9. In the new window to delete a field, add 9XX and click on Delete field.
> > 10. Save Task
> > 11. Close the Task Manager
> > 12. Go to Tools, then Assigned Tasks, and select your task that you just created
> > 13. Check your MARC data. Are the 9xx gone? Does every record now have the appropriate RDA fields?
> {: .solution}
{: .challenge}

## Managing your Task
To change an existing task, go to Tools and Manage Task. This will open the Task Manager window. From here you can rename tasks, export, import them, or assign a Task to a Group.

>## Add a proxy to the 856 40$u in your Task
>
>1. After you run your Task, your MARC records should have your institution's proxy before the url. Remember to check your data to see if there are any proxy stems present.You will need to remove those before running your Task. If the MARC data has different types of electronic urls (resource, related resource, etc.) as noted in the MARC field 856 indicators, you will need to account for that in your Task.
>
> > ## Solution
> > 1. Go to Tools in the upper menu in the MarcEditor
> > 2. Select Manage Tasks
> > 3. Select the Task you just created
> > 4. In Task Actions, select Edit and click Select.
> > 5. Select the plus button and select "Add a Replace All Task"
> > 6. Replace the 856  40$u with 856  40$u[your proxy]. Remember to add 2 spaces after the MARC field.
> > 7. Save
> > 8. Close out of the Task Manager
> > 9. Run your Task again
> > 10. Check your MARC data. Do you see the changes?
> {: .solution}
{: .challenge}
