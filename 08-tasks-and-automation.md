---
title: Tasks and Automation
teaching: 20
exercises: 5
---

::::::::::::::::::::::::::::::::::::::: objectives

- Explain how to create, manage, edit, and run tasks
- Successfully create and run a new task

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What are tasks?
- How do you manage and create new tasks?
- How do you run tasks?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Understanding Automation in MarcEdit

When working with MARC records regularly, you will likely encounter record sets where the data needs the same or very similar approach. A good example is electronic resource records where the resource URL in the 856 field will require the addition of an institution-specific proxy stem. Another example is adding RDA content, carrier, and media terms and codes to your records. Because MARC records typically need to meet cataloguing community standards and local best practices, it is necessary to manipulate MARC data to fit these standards and practices. In the previous lessons learned how to apply one change at a time. In this lesson, we will learn how to string together and automate these changes so they can be re-used in the future.

In the MarcEditor, tasks are the tool that enable such automation. A task is a series of changes to MARC data that occur in the sequence they are entered in the task. One can think of tasks as a mini script of sorts that string together different MarcEditor functions that manipulate MARC data in some way. All tasks are created, managed, and run in the MarcEditor. In this way, tasks are another way to manipulate your data and are an extension of the other tools offered in the MarcEditor.

### What are Tasks?

A task is a series of MarcEdit functions to manipulate data. In the previous lessons, we ran one function at a time. Tasks string a set of functions together so you can run them as a group. Tasks run each function one after another. As such, it is important to think about how you order the functions in your task. For instance, if you want to add your institutions' proxy and the MARC data already has a proxy that you need to delete, your task has to account for that and remove the old proxy before adding a new one.

Tasks are managed through the Task Manager in the MarcEditor. To access the Task Manager, go to Tools and then Manage Tasks in the top level menu. This will open the Task Manager window.

In this window, you will see any tasks that you have created previously. You will see the name that you gave those tasks, the path to where those files are saved on your local computer, a shortcut, and a description. At the bottom of this window you will also have two options "Task Actions" and "Manage Existing Tasks".

Task Actions include:

- New Task: This will create a new task.
- Clone: This will duplicate an existing task.
- Delete: This will remove a task.
- Edit: This will allow you to edit an existing task.
- Rename: This will let you assign a different name to an existing task.

Manage Existing Tasks include:

- Assign to Group: This will let you put tasks into different categories or groups.
- Assign keystrokes: This will let you assign shortcut keys to tasks.
- Backup all tasks: This will let you backup your tasks to your local computer.
- Delete Task Group: This is to remove an existing group.
- Export Task File: This will save a selected task to your local computer for reuse or sharing.
- Import Task File: This will bring in a task from your local computer.
- New Task Group: This will allow you to create a new group.
- Relink tasks: This will allow you to relink tasks.
- Remove From Group: This will let you remove a task from a group.
- Rename Group: This will allow you to rename a group.

The difference between these two actions lists might seem confusing at first. Task Actions allow you to work with a particular task in terms of creating and managing one specific task at a time. The Manage Existing Tasks menu allows you to create and manage groups, exporting and importing, and assigning keyboard shortcuts to tasks.

Tasks don't have to be categorized in groups or be linked to keyboard shortcuts. This is up to the users and their preference for how they organize their task workspace.

:::::::::::::::::::::::::::::::::::::: instructor

Note: “Task Actions” and “Manage Existing Tasks” menu options are different on a Mac.

:::::::::::::::::::::::::::::::::::::::::::::::::

### Create a New Task

To create a task in the MarcEditor, Go to Tools in the top level menu and then Manage Tasks. In the Task Actions menu, select "New Task" from the dropdown menu and then click Select. In the dialogue box, enter the name of your task and click OK. This opens the Edit Task List window where you will see the name you gave your task, a description, tasks, and actions.

Please note that though the Task List Name box allows you to change the name, these changes will not save. To change the name of a task, you need to go to Task Actions and select Rename task.

You can add or update a description in this task list window. The box in the middle will list the functions (or tasks) for this particular task. If there are none, this window will be empty.

Actions include:

- Add: Add a new function or task
- Copy: Clone a function or task already in the list
- Delete: Delete a function or task
- Edit: Change an existing function or task

You can add a new task by clicking on the plus button. You can add any type of function available in the MarcEditor Tools and Edit Shortcuts menu options. This includes the RDA Helper, build a new field, change the case of a MARC field, or generate cutters. You can even include a list of functions (tasks) from another Task.

Click on save at the left bottom corner of the Task List window to save your Task. From there you can close the Task Manager window. To run a task, go to Tools → Assigned Tasks → Current Tasks.

If you have created many Tasks, it does help to assign them to groups to more easily find what you need. If you don't use Groups, the Task Manager will list all of your Tasks in the order they were created and it might be difficult to find a specific task, especially on small screens such as laptops. Tasks can also be reordered in the Task Manager by selecting a task and then moving it in the list using the up and down arrows.

:::::::::::::::::::::::::::::::::::::::  challenge

### Create and run a new Task that runs the RDA helper and removes 9XX fields

:::::::::::::::  solution

### Solution

1. Go to Tools in the upper menu in the MarcEditor
2. Select Manage Tasks
3. In the Task Manager window, in Task Actions, select New Task
4. Click Select.
5. Name your Task
6. In the Task List window, you can describe this task.
7. Click on the plus button and add RDA Helper.
8. Click on the plus button and add a new Add Delete Task Field
9. In the new window to delete a field, add 9XX and click on Delete field.
10. Save Task
11. Close the Task Manager
12. Go to Tools, then Assigned Tasks, and select your task that you just created
13. Check your MARC data. Are the 9xx gone? Does every record now have the appropriate RDA fields?
  
  

:::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

### Managing your Tasks

To edit an existing task, go to Tools → Manage Tasks. In the Task Manger select the task you want to edit, this will highlight the task. Under Task Actions choose Edit Task and click Select. This will open the Edit Task List window. Just like when creating a new task, you can add, delete, or edit functions in your task. Use the up and down arrows to the right to reorder your functions.

:::::::::::::::::::::::::::::::::::::: instructor

Note: If learners need instructions on deleting their existing proxies for the next challenge, suggest they use a find and replace, for example:

1. Click Edit->Replace
2. In the search box for Find, type in =856 40$3Full text:$uhttps://proxy.edu?url= *note the proxy they added may not be this exact string
3. In the search box for Replace, type in =856 40$3Full text:$u
4. Click Replace all
   
:::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::  challenge

### Add a proxy to the `856 40$u` in your Task

1. After you run your Task, your MARC records should have your institution's proxy before the URL. Remember to check your data first to see if there are any proxy stems present. You will need to remove any existing proxies before running your Task. If the MARC data has different types of electronic URLs (resource, related resource, etc.) as noted in the MARC field 856 indicators, you will need to account for that in your Task.

:::::::::::::::  solution

### Solution

1. Go to Tools in the upper menu in the MarcEditor
2. Select Manage Tasks
3. Select the Task you just created. The selected Task will be highlighted.
4. In Task Actions, select Edit Task and click Select.
5. Select the plus button and select "Add a Replace All Task"
6. Replace the `856  40$u` with `856  40$u[your proxy]`. Remember to add 2 spaces after the MARC field.
7. Save
8. Close out of the Task Manager
9. Run your Task again
10. Check your MARC data. Do you see the changes?
  
  

:::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::  callout

### Copying Functions to Tasks

It's possible to copy many functions run in the MarcEditor to a Task for easy reuse. To copy a function, look for the "Copy Task" button in the Batch Editing Tools and Replace Text windows. By clicking "Copy Task" after you've designed and run a function successfully, you can save that function. To add the function to a Task, go to Tools → Manage Tasks. In the Task Manger, under Task Actions choose New Task and click Select. Once in the Edit Task List window, right click and select "Paste Task Action". You can also add the function to an existing Task by selecting Edit Task, instead of New Task.


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: keypoints

- MarcEdit tasks are a way to automate a series of functions
- Tasks can consist of any type of function among the MarcEditor tools

::::::::::::::::::::::::::::::::::::::::::::::::::


