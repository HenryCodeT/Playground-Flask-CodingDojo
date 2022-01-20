# Playground-Flask-CodingDojo
### Python - Flask - Funsdamentals
### Install packages 
* ```pipenv install flask```
* ```pipenv shell```
* ```python server.py```
### project structure
| routs                                              | Funtions          | return                                             |
|----------------------------------------------------|-------------------|----------------------------------------------------|
| Localhost:5000/                                    | hola              | "hola mundo"                                       |
| Localhost:5000/play                                | play              | render_template("index.html", num=3)               |
| localhost:5000/play/```<int:num>```                | play_number       | render_tempalte("index.html", num=num)             |
| localhost:5000/play/```<int:num>/<string:color>``` | play_number_color | render_template("index.html", num=num, color=color |
