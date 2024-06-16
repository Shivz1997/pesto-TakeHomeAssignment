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

CSS File:

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
     
