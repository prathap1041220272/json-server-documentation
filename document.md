# JSON Documnet server

> For getting JSON response from an API, we do need a server.
> To create a server, right now, there are lots of packages are available.
> We use json-server package. So let us install that package.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.


### Installation

Installation on windows
```sh
 npm install -g json-server
```
``
or
``
Installation on ubuntu

```sh
$ sudo npm install -g json-server
```



### Create JSON file

Now we need to create a folder in that folder, create one file called ``db.json``. Let us add the following data inside a ``db.json`` file.

```sh
{
    "books": [
    {
        "id": "1",
        "name": "A song of ice and fire",
        "author": "George RR Martin"
    },
    {
        "id": "2",
        "name": "Harry Potter",
        "author": "JK Rowling"
    },
    {
        "id": "3",
        "name": "Anna Karenina",
        "author": "Leo Tolstoy"
    },
    {
        "id": "4",
        "name": "Great Expectations",
        "author": "Charles Dickens"
    },
    {
        "id": "5",
        "name": "Middlemarch",
        "author": "George Eliot"
    }]
}
```

Now, we need to start a JSON server that serves this data. So go to the terminal and type the following command.
```sh
json-server --watch db.json --port 4000
```
``
Now, you can access all the books on this URL: http://localhost:4000/books
``
