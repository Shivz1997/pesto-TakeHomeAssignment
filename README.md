# pesto-TakeHomeAssignment
Pesto Take Home Assignment 

HTML File

(app.component.html)
HTML code for te task managemnet application consists of 3 major parts:

1. Task Form:

   * This section contains a form for creating a new task.
   * There are two input elements for the user to enter the task’s title and description.
   * A select element allows the user to choose the status of the task from three options: Pending, In Progress, and Completed.
   * A button element is used to submit the form and add the new task to the list. The (click) event is bound to the addTask() method which will be defined in your Angular component.

2. Task Filter:

   * This section provides a dropdown menu to filter tasks by their status.
   * The select element here binds to filterStatus in your Angular component, which will control which tasks are displayed based on their status.

3. Task List:

   * An unordered list (ul) displays the tasks.
   * The *ngFor directive is used to loop over each task in the tasks array.
   * Each task is displayed as a list item (li) showing its title, description, and status.
   * Two buttons are provided for each task: one to delete the task and another to update its status. These buttons are bound to deleteTask(task) and updateStatus(task) methods respectively.

The Angular directives like [(ngModel)] and *ngFor bind parts of your template to your component’s properties and methods, enabling dynamic updates and interaction.
