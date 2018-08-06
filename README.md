# MyReads Project

This project was created with a starter template for the final assessment project for Udacity's React Fundamentals course. The template provided a static example of the CSS and HTML markup that I used to implement the necessary React code that I needed to complete the project. I added interactivity to the project and made it dynamic.


## Installation and Running the Project

To install and use the project:

* **Zip-Download:** Download the repository as a zip-file, extract it, use Git Bash to change
into the project directory.
* **Clone the Repository:** Clone the repository with Git Bash to a directory of your choice: ```git clone https://github.com/DanielaKuester/Udacity-Project07-MyReadsApp/```.
* install all project dependencies with `npm install`
* start the development server with `npm start`
* ater running `npm start`, the React App should open automatically in your browser. If it doesn't, open `localport:3000` in your Browser.

## What You're Getting
```bash
├── CONTRIBUTING.md
├── README.md - This file.
├── SEARCH_TERMS.md # The whitelisted short collection of available search terms for you to use with your app.
├── package.json # npm package manager file. It's unlikely that you'll need to modify this.
├── public
│   ├── favicon.ico # React Icon, You may change if you wish.
│   └── index.html # DO NOT MODIFY
└── src
    ├── App.css # Styles for your app. Feel free to customize this as you desire.
    ├── App.js # This is the root of the app, containing dynamic code made with ReactJS.
    ├── App.test.js # Used for testing. Provided with Create React App. Testing is encouraged, but not required.
    ├── Book.js # The Book Component that helps to insert single books.
    ├── BooksAPI.js # A JavaScript API for the provided Udacity backend. Instructions for the methods are below.
    ├── BookshelfChanger.js # The Component that allows you to move a book to another shelf.
    ├── BookshelfTitle.js # The Component that lets you set the title of the shelf. After a future update, the user can interactively add a new bookhelf title.
    ├── Bookshelves.js # The Component that contains the bookshelves.
    ├── icons # Helpful images for your app. Use at your discretion.
    │   ├── add.svg
    │   ├── arrow-back.svg
    │   └── arrow-drop-down.svg
    ├── index.css # Global styles. You probably won't need to change anything here.
    ├── index.js # You should not need to modify this file. It is used for DOM rendering only.
    ├── Main.js # The Main page that shows the bookshelves.
    ├── SearchOpen.js # The Component that allows you to change to the search page.
    └── SearchPage.js # The SearchPage Component contains the search page with the search field and the books resulting from your search.
```


## Backend Server

To simplify the development process, Udacity provided a backend server to develop against. The provided file [`BooksAPI.js`](src/BooksAPI.js) contains the methods needed to perform necessary operations on the backend:

* [`getAll`](#getall)
* [`update`](#update)
* [`search`](#search)

### `getAll`

Method Signature:

```js
getAll()
```

* Returns a Promise which resolves to a JSON object containing a collection of book objects.
* This collection represents the books currently in the bookshelves in your app.

### `update`

Method Signature:

```js
update(book, shelf)
```

* book: `<Object>` containing at minimum an `id` attribute
* shelf: `<String>` contains one of ["wantToRead", "currentlyReading", "read"]  
* Returns a Promise which resolves to a JSON object containing the response data of the POST request

### `search`

Method Signature:

```js
search(query)
```

* query: `<String>`
* Returns a Promise which resolves to a JSON object containing a collection of a maximum of 20 book objects.
* These books do not know which shelf they are on. They are raw results only. You'll need to make sure that books have the correct state while on the search page.

## Important
The backend API uses a fixed set of cached search results and is limited to a particular set of search terms, which can be found in [SEARCH_TERMS.md](SEARCH_TERMS.md). That list of terms are the _only_ terms that will work with the backend, so don't be surprised if your searches for Basket Weaving or Bubble Wrap don't come back with any results.

## Original Repository

This project was made with the help of the starter code from the [Udacity MyReadsApp repository](https://github.com/udacity/reactnd-project-myreads-starter).

## Credits and Dependencies

* I used [Maeva's study jam](https://www.youtube.com/watch?v=i6L2jLHV9j8&feature=youtu.be) to understand many basic concepts of React for this project. I changed her code to suit my needs and made some parts of the project more complex by adding more components. I want to continue to work on the project after graduation, so I wanted to lay the foundation to make the project easier scalable. In my code, I have given credits to Maeva's study jam and when I used some of her code, I explained where you can find it in the video, what it does and what I changed.
* The [Udacity React lessons about controlled components](https://classroom.udacity.com/nanodegrees/nd001/parts/c3e7b0d6-ffef-4421-b5fc-6df10fd0a1ae/modules/82766b2b-1870-4904-aa90-8ccbe63928c5/lessons/14331e60-a548-4cfb-a326-054545da8927/concepts/fc3f11d3-8779-4d8a-8a23-1cd782f8ddf3) helped me to implement the basic version of the search function. I refined it with the help of Maeva's study jam mentioned above.
* The [React documentation about Conditionals](https://reactjs.org/docs/conditional-rendering.html) and Maeva's study jam helped me a lot to understand the ternary operator better. If you have any idea how I can rewrite SearchPage.js, lines 111-115 to a (properly working) if-else-statement, I am absolutely open to suggestions. (Yes, I am still working on the basics of programming. It is important to understand them!)

## Create React App

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md).

## Contributing

This repository is my project as a Udacity student. I am planning to work on the project and to update it in the future to document how my programming skills grow and develop. Therefore, I most likely will not accept pull requests.

For details, check out [CONTRIBUTING.md](CONTRIBUTING.md).


## License

This project uses the MIT License. For further information, see [LICENSE](LICENSE)