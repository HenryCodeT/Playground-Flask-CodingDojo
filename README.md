# Playground-Flask-CodingDojo
### Python - Flask - Funsdamentals
### Install packages 
* ```pipenv install flask```
* ```pipenv shell```
* ```python server.py```
### project structure
| routs | Funtions | return |
|---|---|---|
| Localhost:5000/ | init_checkerboard() | render_template("index.html",number_rows=8, number_colums=8,color1="black",color2="red") |
| Localhost:5000/```rows``` | hange_rows(rows) | render_template("index.html",number_rows=rows, number_colums=8,color1="black",color2="red") |
| localhost:5000/```rows/colums``` | change_rows_colums(rows,colums) | render_template("index.html",number_rows=rows, number_colums=colums,color1="black",color2="red") |
| localhost:5000/```/rows/colums/color1``` | change_rows_colums_color(rows,colums,color1) | render_template("index.html",number_rows=rows, number_colums=colums,color1=color1,color2="red") |
| localhost:5000/```/rows/colums/color1/color2``` | hange_rows_colums_colors(rows,colums,color1,color2) | render_template("index.html",number_rows=rows, number_colums=colums,color1=color1,color2=color2) |
### jinja
```<body>
    <h1 style="background-color:{{color1}};color:{{color2}};">***CheckerBoard***</h1>
    <main class="main">
        {% for i in range(0,number_rows) %}
        <div class="row ">
            {% for x in range(0,number_colums) %}
            <div class="block" style="background-color:{% if (i+x) is even %}{{color1}};{% else %}{{color2}};{% endif %}">
            </div>
            {% endfor %}
        </div>
        {% endfor %}    
    </main>
</body>```
