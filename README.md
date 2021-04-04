# A LaTeX template for assignement

## Layout

You can use :
* ```\newcommand{\matiere}{Math}``` To edit the subject name
* ```\newcommand{\titre}{Assignment 5}``` To edit the assignment name
* ```\newcommand{\auteur}{Your Name}```
* ```\newcommand{\ladate}{}``` If you want to include a date

## Questions

### New questions

* ```\question``` A new question
* ```\questionnobar``` A new question without delimiter
* ```\subquestion``` A new subquestion
* ```\subquestionnobar```  A new subquestion without delimiter

### Numbering

If you want to change the way the questions are numbered, you can use :
```\newcommand{\questionformat}{x}``` Where x can be : **A I 1**
```\newcommand{\subquestionformat}{y}``` Where x can be : **A a I i 1**

If you don't want the questions to appear as "Question", you can rename them using : ```\questiontype{New Name}```.
For instance : ```\questiontype{Problem}```

You can also add a custom title to a question using ```\questionname{Title}```.
For instance : ```\questionname{Beginner's Guide}```

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

## Listing

If you want to include code in your document, use :
```
\begin{figure}
    \begin{lstlisting}[style=Python]
        print("Hello World")
    \end{lstlisting}
\end{figure}
```
The two styles currently supported are : "Matlab" and "Python". You can add optional caption or label to the listing. If you want to import code from a file, use :

``` \lstinputlisting[caption={My code},label={lst:name}]{path/to/file}```


## Maths

### Shortcuts

* ```\sqfr{a}{b}``` = ```\sqrt{\frac{#1}{#2}}```
* ```\inv{a}``` = ```\frac{1}{a}```
* ```\invfr{a}``` = ```\frac{1}{\sqrt{a}}```
* ```\dpi``` = ```\frac{\pi}{2}```
* ```\demi``` = ```\frac{1}{2}```
* ```\ei{x}``` = ```e^{i x}```
* ```\w``` = ```\omega```

### Functions
* ```\s{x}``` = ```\sin\left(x\right)```
* ```\c{x}``` = ```\cos\left(x\right)```

### Integrals
* ```\int``` = Top and Bottom limits
* ```\inte``` = Side limits

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
* ```\length{x}``` = ```\SI{x}{\metre}```
* ```\time{x}``` = ```\SI{x}{\second}```
* ```\force{x}``` = ```\SI{x}{\newton}```

### Differential calcul
* ```\d``` = ```\mathrm{d}```
* ```\deriv{f}{x}``` = ```\frac{\mathrm{d}f}{\mathrm{d}x}```
* ```\deriv{f}{x}``` = ```\frac{\mathrm{d}^2f}{\mathrm{d}^2x}```
* ```\drond{f}{x}``` = ```\frac{\partial f}{\partial x}```
* ```\ddrond{f}{x}``` = ```\frac{\partial^2 f}{\partial x^2}```
* ```\dddrond{f}{x}{y}``` = ```\frac{\partial^2 f}{\partial x\partial y}```
* ```\dx``` = ```\mathrm{d}x```
* ```\dy``` = ```\mathrm{d}y```
* ```\dz``` = ```\mathrm{d}z```
* ```\dr``` = ```\mathrm{d}r```
* ```\dt``` = ```\mathrm{d}t```
* ```\df``` = ``` \mathrm{d}f```
* ```\dv``` = ``` \mathrm{d}V```
* ```\ds``` = ``` \mathrm{d}S```
* ```\dphi``` = ``` \mathrm{d}\phi```
* ```\drho``` = ``` \mathrm{d}\rho```
* ```\dtau``` = ``` \mathrm{d}\tau```
* ```\dtheta``` = ``` \mathrm{d}\theta```
