# APIJS
A simple user table app that fetches live user data from an API and displays it in a clean, responsive UI. Built using HTML, CSS, and JavaScript.


# Overview

This project is a simple User Listing App that fetches real user data from the public API:

https://jsonplaceholder.typicode.com/users

The API returns 10 fictional users, and this project displays them in a clean & modern table layout.

I created this project while learning Fetch API, JSON data handling, and HTML table rendering.
It is a great beginner exercise for understanding how data flows from an API into the UI.

Features
 Fetches live user data

Uses JavaScript fetch() to retrieve user information directly from the API.

 Clean and easy-to-read table UI

The layout is styled to be simple and similar to real-world admin dashboards.

Displays full user details

The table shows:

Id

Name

Username

Email

City

Phone

Website (clickable link)

Company name

🔹What I Learned

This project helped me understand:

🔹 Fetch API

How to make HTTP GET requests:

const response = await fetch(URL);
const data = await response.json();

🔹 JSON data parsing

How to work with nested objects like:

user.address.city
user.company.name

🔹 DOM manipulation

How to insert table rows dynamically:

row.innerHTML = `...`;
tableBody.appendChild(row);

🔹 Building a UI from API data

Mapping API fields to table columns.

✔ Pure HTML + CSS + JavaScript

No frameworks, no libraries — the goal was to understand everything from scratch.

/project
│
├── index.html  
└── README.md


# How It Works
1 Fetch users from API
const response = await fetch("https://jsonplaceholder.typicode.com/users");
const users = await response.json();

2️ Loop through the users
users.forEach(user => { ... });

3️ Insert rows into the table
row.innerHTML = `
  <td>${user.id}</td>
  <td>${user.name}</td>
  <td>${user.username}</td>
  ...
`;

4️ Add them to the UI
tableBody.appendChild(row);



# Future Improvements

Here are some ideas I may add later:

Search bar to filter users

Sort by name or email

Pagination for long lists

Dark mode

Loading spinner before API data appears

# Author

HimAnshNA

I built this project while learning how APIs work with JavaScript.
This is one of the first steps in my journey into web development with real data.

If you like this project

Feel free to star ⭐ the repo ...it helps a lot and motivates learning!
