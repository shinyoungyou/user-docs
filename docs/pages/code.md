# Editing Code Efficiently in VS Code
In this section, we will talk about editing code efficiently in VS Code. This guide shows how to make your HTML and CSS editing faster and smarter using features like multi-cursor, and other powerful editing tools. These tips will help you save time, reduce repetitive work, and focus on more creative and meaningful tasks in your web design projects.


## Using Multi-Cursor for Faster Code Editing
VS Code allows you to place multiple cursors in different places to edit code at once.

### Overview
This set shows how to use the multi-cursor feature in two common scenarios:

- **Renaming Repeated Code**: Changing a repeated class name across multiple HTML elements.
- **Placing Multi-Cursor**: Adding an attribute to each list item in a simple HTML list.

### Example 1: Renaming Repeated Code
1. Prepare Your HTML File
Copy and paste the following HTML structure into a new file:
``` { .html }
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Efficient Coding Demo</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="card">
    <h1>Hello World</h1>
    <p>This is a simple component.</p>
  </div>
  <div class="card">
    <h1>Hello World</h1>
    <p>This is a simple component.</p>
  </div>
  <div class="card">
    <h1>Hello World</h1>
    <p>This is a simple component.</p>
  </div>
  <div class="card">
    <h1>Hello World</h1>
    <p>This is a simple component.</p>
  </div>
</body>
</html>
```
You now have multiple `<div class="card">` elements.
Let's say you want to change the class name `card` to `box`.

2. **Select the Text to Edit**: Highlight one of the word `card`.
3. **Select More Matches**
    - **One by One**: Press `Ctrl` + `D` to select the next matching word.
        -  While holding down Ctrl, press D repeatedly to select the next matching word each time.
    - **Select All at Once**: After selecting one of the words, press `Ctrl` + `Shift` + `L` to select all matching words in the file at once
4. **Edit the Text**: Once selected, type `box`. Then, all selected words will change at the same time.


### Example 2: Place Multi-Cursor
1. **Prepare Your HTML File**
    
    Copy and paste the following HTML structure into a new file:
``` { .html }
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <ul>
        <li>Apple</li>
        <li>Banana</li>
        <li>Orange</li>
        <li>Mango</li>
    </ul>
</body>
</html>
```
Now, you want to add `class="item"` to each `<li>` tag.

2. Hold down the `Alt` key and click in front of each `<li>` tag where you want to insert the attribute.
3. Type `class="item"`, so you can have it at each cursor position.


## Quickly Close Multiple Tabs
Tired of closing tabs one by one?
VS Code gives you easy ways to close tabs without doing it one by one.

1. Right-click on any open tab.
2. Choose a Tab Closing Option:
    - `Close`
    - `Close Others`
    - `Close to the Right`
    - `Close to the Left`
    - `Close All`

Use these to clean up your editor quickly and get back to coding!


## Open Files Quickly by Searching
Finding files in large projects can be time-consuming. 
If you can’t remember the exact location, use **Quick Open** to locate your files instantly.

1. Press `Ctrl`+`P` to open the Quick Open dialog.
2. **Search for Your File**: Type part of the file name. VS Code will display a list of matching files, including those recently or frequently opened.
3. **Select and Open the File**: Use the arrow keys (↑ / ↓) keys to navigate the list, then press Enter to open the file.

Note: The more specific you are with the file name, the quicker you’ll find the file you need.

This is much faster than browsing through the folder structure manually!