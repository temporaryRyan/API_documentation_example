# API_documentation_example
This is an example of a table used to document endpoints in an API project

## API Endpoints

| Method       | URL | Result |
| :--- |:---| :---|
|GET| `localhost:3000/`| Returns a list of all quotes in the database|
|GET | `localhost:3000/quotes`| Returns a list of all quotes in the database|
|GET | `localhost:3000/quotes/38`| Returns all information related to quote with ID=38|
|GET | `http://localhost:3000/quotes/search/?author=Abraham Lincoln`| Returns all quotes in database where author is Abraham Lincoln|
|GET | `http://localhost:3000/quotes/search/?content=Four score...` | Returns quote with content "Four score..."|
|GET|`http://localhost:3000/quotes/random`|Returns a random quote from the database|
|POST|`http://localhost:3000/quotes/?author=Abraham Lincoln&content=Four score...`|Adds quote to database. Author:Abraham Lincoln, Content: "Four score...". If POST is succesfull, returns database object for newly created quote.|
|PUT/PATCH|`http://localhost:3000/quotes/38?author=Joe Biden`|Updates the author for a quote with ID=38. If PUT/PATCH is succesfull, returns database object for newly updated quote.|
|DELETE|`http://localhost:3000/quotes/38`|Deletes the quote with ID=38 from database|
