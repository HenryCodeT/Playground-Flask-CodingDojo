# Playground-Flask-CodingDojo
### Python - Flask - Funsdamentals
### Install packages 
* ```pipenv install Flask```
* ```pipenv shell```
* ```python server.py```
### project structure
| routs                                              | Funtions    | return                      |
|----------------------------------------------------|-------------|-----------------------------|
| Localhost:5000/                                    | hola        | "Hello World!"              |
| Localhost:5000/dojo                                | dojo        | "Dojo!"                     |
| localhost:5000/say/<string:name>                   | show_string | "Hello {name}!"             |
| localhost:5000/repeat/<int:number>/<string:string> | repeat      | "'{string}' {number} times" |
