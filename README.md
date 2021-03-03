# A LaTeX template for assignement

## Layout

You can use :
* ```\matiere}{Math}``` To edit the subject name
* ```\titre}{Assignment 5}``` To edit the assignment name
* ```\auteur}{Your Name}```
* ```\ladate}{}``` If you want to include a date

## Questions

### New questions

* ```\question``` A new question
* ```\questionnobar``` A new question without delimiter
* ```\subquestion``` A new subquestion
* ```\subquestionnobar```  A new subquestion without delimiter

### Numbering

If you want to change the way the questions are numbered, you can use :
```\questionformat}{x}``` Where x can be : **A I 1**
```\subquestionformat}{y}``` Where x can be : **A a I i 1**

If you don't want the questions to appear as "Question", you can rename them using : ```\questionname}{New Name}```
For instance : ```\questionname}{Problem}```

If you want, you can change the numbering system for a specific question using :
* ```\question[x]``` Where x can be : **A I 1**
* ```\subquestion[y]``` Where x can be : **A a I i 1**

## Environnement

You can create environment using :
```
\begin{notation}
<test goes here>
\end{notation}
```

Custom environment includes :
* ```eq``` : Equation
* ```res``` : Results
* ```prop``` : Property
* ```notation``` : Notation
* ```hypo``` : Hypothesis
* ```conclusion``` : Conclusion

You can add a ```*``` to remove numbers.

If you want to add a title, you can use :

```
\begin{eq}[Equation title]
<text goes here>
\end{eq}
```

## Maths

### Shortcuts

* ```\sqfr{a}{b}``` = ```\sqrt{\frac{#1}{#2}}```
* ```\inv{a}``` = ```\frac{1}{a}```
* ```\invfr{a}``` = ```\frac{1}{\sqrt{a}}```
* ```\dpi``` = ```\frac{\pi}{2}```
* ```\ei{x}``` = ```e^{i x}```
* ```\w``` = ```\omega```

### Functions
* ```\s{x}``` = ```\sin\left(x\right)```
* ```\c{x}``` = ```\cos\left(x\right)```

### Vectors
* ```\vec{x}``` = ```\overrightarrow{x}```
* ```\ux``` = ```\overrightarrow{u_x}```
* ```\uy``` = ```\overrightarrow{u_y}```
* ```\uz``` = ```\overrightarrow{u_z}```
* ```\utheta``` = ```\overrightarrow{u_{\theta}}```
* ```\uphi``` = ```\overrightarrow{u_{\varphi}}```
* ```\ur``` = ```\overrightarrow{u_r}```
* ```\ex``` = ```\overrightarrow{e_x}```
* ```\ey``` = ```\overrightarrow{e_y}```
* ```\ez``` = ```\overrightarrow{e_z}```
* ```\etheta``` = ```\overrightarrow{e_{\theta}}```
* ```\ephi``` = ```\overrightarrow{e_{\varphi}}```
* ```\er``` = ```\overrightarrow{e_r}```

### Units

You can write x using scientific notation. For instance : x=1,24e-3.

* ```\speed{x}``` = ```\SI{x}{\metre\per\second}```
* ```\stiff{x}``` = ```\SI{x}{\newton\per\meter}```
* ```\pulse{x}``` = ```\SI{x}{\radian\per\second}```
* ```\metre{x}``` = ```\SI{x}{\metre}```
* ```\temps{x}``` = ```\SI{x}{\second}```
* ```\force{x}``` = ```\SI{x}{\newton}```

### Differential calcul
* ```\do``` = ```\mathrm{d}```
* ```\deriv{f}{x}``` = ```\frac{\mathrm{d}f}{\mathrm{d}x}```
* ```\deriv{f}{x}``` = ```\frac{\mathrm{d}^2f}{\mathrm{d}^2x}```
* ```\drond{f}{x}``` = ```\frac{\partial f}{\partial x}```
* ```\drond{f}{x}``` = ```\frac{\partial^2 f}{\partial x^2}```
* ```\dx``` = ```\mathrm{d}x```
* ```\dy``` = ```\mathrm{d}y```
* ```\dz``` = ```\mathrm{d}z```
* ```\dt``` = ```\mathrm{d}t```







