# organized-me

## Overview
Organize Me is a task management tool built with plain JavaScript, styled to function similarly to Trello. It's a single-page application that allows users to add tasks and drag them between different status boards, providing a simple and effective way to manage various tasks in daily life. 

## Technologies Used
- JavaScript
- HTML
- CSS
- Local Storage
- HTML Drag and Drop API

## Problem Statement
1. **Managing Application State:** One of the key challenges was effectively handling the state of the application, especially when dealing with the intricate interactions involved in dragging and dropping elements.

2. **Smooth Drag-and-Drop Functionality:** Implementing a seamless and user-friendly drag-and-drop functionality was a crucial aspect to provide a comfortable user experience.

3. **Task Storage and Status Management:** Storing tasks and their corresponding statuses across different boards, including backlog, progress, complete, and on-hold, required careful consideration and design.



## Solution

### Using Local Storage in JavaScript
1. **getSavedColumns() Function**:
    - This function retrieves data from **\`localStorage\`** using **\`getItem()\`**. If the data exists, it parses the JSON data and assigns it to the corresponding arrays.
    - If the data doesn't exist in **\`localStorage\`**, default values are assigned to the arrays.
2. **updateSavedColumns() Function**:
    - This function updates the data in **\`localStorage\`** using **\`setItem()\`**, by converting the arrays into JSON strings.
3. **createItemEl Function**:
    - This function is creating a new DOM element (the code snippet provided doesn't show what's being done with this element).

Note: **\`localStorage\`** can only store string values. When you want to save an array or an object, you need to convert it into a string using \`JSON.stringify\`.

### Using HTML Drag and Drop API
1. **Draggable Elements**: Elements are made draggable using the draggable attribute set to true.

2. **Drag Events**: The API provides events like dragstart, drag, and dragend that control the element's behavior during dragging.

3. **Drop Zones**: Drop zones are designated areas where draggable elements can be released. The dragover event is used to define valid drop zones.

## Learning 

This project is a powerful learning experience to enhance my understanding of JavaScript concepts and application development.

### 1. Using Local Storage in JavaScript

Learning to use `localStorage` in JavaScript is essential for storing data on the client side. It provides a way to save and retrieve information even after the user navigates away from the webpage or closes the browser. This is particularly useful for tasks like saving user preferences or storing temporary data.

### 2. Managing Array Deletions

When using the `delete` operator in JavaScript to remove an element from an array, it creates an undefined "hole" in the array without re-indexing the remaining elements. This can lead to unexpected behavior. To address this, it's recommended to use array methods like `filter` after deleting an element. This way, the array is properly restructured, and undefined elements are removed.

### 3. Handling `querySelectorAll` Results

When using `querySelectorAll` in the DOM to select elements, the returned result might look like an array but isn't a true JavaScript array. This can lead to issues when using array methods like `.map()`. To overcome this, you can convert the result into an actual array using `Array.from()`. This will enable you to use array methods without errors, providing a smoother experience when manipulating selected elements.
as detailed above.


