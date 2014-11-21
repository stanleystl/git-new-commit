#Comum aos dois participantes:#

1) Fork o repositório

### PARTICIPANTE 1: ###

**BUG-FIX**

1) Adicione as linhas de código que estão faltando para que ele execute corretamente logo após a linha "BUG-FIX" no início.

    import sys
    import turtle

2) Execute o exemplo e veja se está rodando.

    $ python example.py

3) Comite para o repositório. Descreva o melhor possível o que foi feito. 

    $ Git add example.py
    $ Git new-commit
    $ Git push

**NEW-FEATURE**

1) Adicione o código abaixo logo após o comentário "NEW-FEATURE". Este código adiciona 6 novos quadrados ao canvas com cores diferentes de espessura e tamanhos pré-definidos.  

    colors = ['red', 'orange', 'yellow', 'green', 'blue', 'violet']
    t.pensize(3)
    for i, color in enumerate(colors):
    	square(t, (screen_y / 2) / 10 * (i+1), color)

2) Comite para o repositório. Descreva o melhor possível o que foi feito. 

    $ Git add example.py
    $ Git new-commit
    $ Git push

### PARTICIPANTE 2: ###

**OPTIMIZATION**

0) Faça um pull das modificações
    
    $ Git pull

1) Analise o histórico recente de commits.

	$ Git log

1) Execute o exemplo e veja se está funcionando corretamente. 

    $ python example.py

2) Adicione o código abaixo logo após o comentário "OPTIMIZATION". Este código aumenta a velocidade de desenho para o maior possível.

    t.speed(0)

3) Execute o aplicativo e analise as mudanças.

    $ python example.py 
    
4) Comite para o repositório. Descreva o melhor possível o que foi feito. 
    
    $ Git add example.py
    $ Git new-commit
    $ Git push

5) Modifique o código logo após a linha "BUG INSERIDO" conforme abaixo. Mude a posição de screen_x / 2 e screen_y / 2 para screen_x / 4 e screen_y / 4. 
    
    t.forward(screen_x / 4)
    t.right(90)
    t.forward(screen_y / 4)
    t.setheading(180)

6) Execute o aplicativo e analise as mudanças. Veja que o quadrado não mais será desenhado na parte central. Consideramos como um bug inserido hipoteticamente sem a percepção do desenvolvedor.

7) Comite para o repositório. Descreva o melhor possível o que foi feito sem caracterizar como um bug inserido e sim como uma optimização. 
    
    $ Git add example.py
    $ Git new-commit
    $ Git push

### PARTICIPANTE 1: ###

0) Faça um pull das modificações
    
    $ Git pull

1) Analise o histórico de commits. 

2) Execute o aplicativo e analise as mudanças.

    $ python example.py 

3) Tente consertar o que está errado baseado apenas no que pode tirar de conclusões do histórico

4) Conserte o código e comite. 

	$ Git add example.py
    $ Git new-commit
    $ Git push





