# pesto-TakeHomeAssignment
Pesto Take Home Assignment 

HTML File:
-----------

(app.component.html) -- file name
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

CSS File:
---------

(app.component.css) - file name

1. General Styles;

   * body: Sets the font to Arial, background color to a light grey, removes default margin, and adds padding around the entire content for better spacing.
   * .container: Centers the content with a maximum width of 600px and adds background color, padding, border-radius for rounded corners, and a box-shadow for a subtle depth effect.

2. Task Form Styles:

   * .task-form: Uses flexbox to arrange child elements in a column direction.
   * input[type="text"], select: Styles text inputs and select dropdowns with padding for larger click areas, margin for spacing between elements, rounded borders, and a light border color.
   * button: Styles buttons with padding, a green background color, white text, no border, and rounded corners. The hover state changes the background color to a darker green.

3. Task List Styles:

   * .task-list: Removes default list styling and left padding.
   * li: Sets background color to off-white, adds a bottom border for separation between tasks, adds padding for spacing inside each task item, and uses flexbox to space out task content and buttons evenly.

4. Button Group Styles:

   * .button-group button: Adds margin to the right of buttons to ensure they don’t touch each other.

5. Task Filter Styles:

   * .task-filter select: Styles the filter dropdown to match the form inputs with padding, rounded borders, a light border color, and an auto width to adjust based on content.

This CSS enhances the visual appeal of your task management application by adding spacing, colors, and interactive elements like hover states.

  TypeScript File:
  -----------------

  (app.component.ts) -- file name

  Detailed Explaination of typescript file:

  1. Import Statements:

     import { Component } from '@angular/core';: This imports the Component decorator from Angular’s core library, which is used to define a class as a component in Angular.

  2. Task Interface:

     interface Task: Defines a TypeScript interface named Task, which represents the structure of a task object with three properties: title, description, and status, all of which are strings.

  3. Component Decorator:

     * @Component({...}): The @Component decorator defines metadata for the component, including its selector, template URL, and style URLs.
     * selector: 'app-root': This is the custom HTML tag that will be used to insert this component into other templates.
     * templateUrl: Points to the HTML file that contains the template for this component.
     * styleUrls: Points to the CSS file that contains styles for this component.

   4. AppComponent Class:

      * export class AppComponent: This line exports the class so it can be imported into other parts of your application.
      * Inside the class, three properties are defined:
          1)  newTask: Task: Holds the data for a new task being created. It’s initialized with empty strings for title and description, and ‘pending’ as the default status.
          2) tasks: Task[]: An array to store all tasks. It’s typed with the Task interface.
          3) filterStatus: string: A string to hold the current filter status selected by the user.

    5. Methods:

       * addTask(): This method adds a new task to the tasks array if both title and description are provided. After adding, it resets newTask to its initial state.
       * deleteTask(taskToDelete: Task): This method filters out the task to be deleted from the tasks array.
       * updateStatus(taskToUpdate: Task): This method toggles the status of a task between ‘completed’ and ‘pending’.


This TypeScript code works together with your HTML template and CSS styles to create a dynamic and interactive task management application using Angular.

  
