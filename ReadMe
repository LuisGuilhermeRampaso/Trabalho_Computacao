
# Explorando o Universo Gráfico com OpenGL: Uma Introdução Prática

Este repositório contém os exemplos práticos desenvolvidos como parte do trabalho "Explorando o Universo Gráfico com OpenGL: Uma Introdução Prática". Os exemplos utilizam a linguagem Python com as bibliotecas `PyOpenGL` e `glfw`.

## ✅ Requisitos

Instale as bibliotecas necessárias com:

```bash
pip install PyOpenGL PyOpenGL_accelerate glfw
```

---

## 🪟 1. Criação de uma Janela com GLFW

```python
import glfw
from OpenGL.GL import *

def main():
    if not glfw.init():
        return
    window = glfw.create_window(640, 480, "Minha Janela OpenGL", None, None)
    if not window:
        glfw.terminate()
        return
    glfw.make_context_current(window)
    while not glfw.window_should_close(window):
        glClear(GL_COLOR_BUFFER_BIT)
        glfw.swap_buffers(window)
        glfw.poll_events()
    glfw.terminate()

main()
```

---

## 🔺 2. Desenhando Primitivas (Ponto, Linha e Triângulo)

```python
import glfw
from OpenGL.GL import *

def draw_shapes():
    glBegin(GL_POINTS)
    glVertex2f(0.0, 0.0)
    glEnd()

    glBegin(GL_LINES)
    glVertex2f(-0.5, -0.5)
    glVertex2f(0.5, -0.5)
    glEnd()

    glBegin(GL_TRIANGLES)
    glVertex2f(0.0, 0.5)
    glVertex2f(-0.5, -0.5)
    glVertex2f(0.5, -0.5)
    glEnd()

def main():
    if not glfw.init():
        return
    window = glfw.create_window(640, 480, "Primitivas OpenGL", None, None)
    if not window:
        glfw.terminate()
        return
    glfw.make_context_current(window)
    while not glfw.window_should_close(window):
        glClear(GL_COLOR_BUFFER_BIT)
        draw_shapes()
        glfw.swap_buffers(window)
        glfw.poll_events()
    glfw.terminate()

main()
```

---

## 🎨 3. Usando Cores nas Primitivas

```python
def draw_colored_shapes():
    glBegin(GL_TRIANGLES)
    glColor3f(1.0, 0.0, 0.0)  # Vermelho
    glVertex2f(0.0, 0.5)
    glColor3f(0.0, 1.0, 0.0)  # Verde
    glVertex2f(-0.5, -0.5)
    glColor3f(0.0, 0.0, 1.0)  # Azul
    glVertex2f(0.5, -0.5)
    glEnd()
```

---

## 🔄 4. Transformações Geométricas

```python
from OpenGL.GL import *
from OpenGL.GLU import *

def draw_transformed_triangle():
    glPushMatrix()

    # Translação
    glTranslatef(0.5, 0.0, 0.0)

    # Rotação
    glRotatef(45, 0, 0, 1)

    # Escala
    glScalef(0.5, 0.5, 1.0)

    glBegin(GL_TRIANGLES)
    glColor3f(1.0, 1.0, 0.0)
    glVertex2f(0.0, 0.5)
    glVertex2f(-0.5, -0.5)
    glVertex2f(0.5, -0.5)
    glEnd()

    glPopMatrix()
```
