# - Hello-Word1
# - Luis Angel Rios Jasso
# - Carrera: ITD
# - Origen: CDMX
## - Equipo -
➡️Yo simon

# **SemanaTec**

#2. Tipos de letras
**bold**
*Italic*
>Block

>Hola

>Adios


#3. Lista enumerada
1. Gorditas de cuidad victoria
2. Corundas de Morelia
3. Tortas de la Barda, Tampico
4. La parroquía, Veracruz
5. Tacos Alfaro, Centrito Valle
6. Chilaquiles TEC - ITEMS

#4. Vista con Viñetas
- Tacos Gúero 
- Tacos la Morelense
- Tacos el Porton

#5. Codigo
```python
from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```
#6. regla
---

#7. link

-[freegames](https://grantjenks.com/docs/freegames/#)
-[rockconten](https://rockcontent.com/es/blog/que-son-los-gifs/)


#8. Imagenes

![Magdalena Contreras](https://imgs.search.brave.com/4Sm352_t4IyC6Krv4jzfAD0nIc7U3XUJlMVpzPN_odY/rs:fit:500:0:0/g:ce/aHR0cHM6Ly9tZXhp/Y29jaXR5LmNkbXgu/Z29iLm14L3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDE0LzEwL2Zv/cm8tZGUtbGEtY3Vs/dHVyYS1kZS1sYS1t/YWdkYWxlbmEtY29u/dHJlcmFzLmpwZw)

#9. tabla 
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

#10. Lista de Equipo

- [x] Luis Angel Rios Jasso
