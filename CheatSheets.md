# LaTex cheat sheets
While writing my physics protocol I often got stuck when writing my equations. No I did not forget how to spell mu (as in micrometer). Furthermore I dont know all the stuff you need to create a graph with pgfplots, so I often turned to online cheat sheets. In this file I will list all of my favorite cheat sheets for your comfort. Just click on the headings to get to the website.
## [Mathematical Symbols](https://en.wikipedia.org/wiki/List_of_mathematical_symbols_by_subject)
Writing equations with greek letters I can't remember I needed to look them up. Not only are all greek letters in here, but most symbols you need for an equation like a plusminus symbol are to be found on this site. It's one of my favourites as it is not only rich in content but only very readable and structured. I love wikipedia :)
## [The Basics as one cheat sheet](https://quickref.me/latex)
A very readable and compact summary of all the stuff you need for a basic LaTex document. This is basically the Wikipedia one but with the inclusion of most enviroments like an array. A good site to have bookmarked if you still need some basic stuff.
## [LaTex Quickstart](http://tug.ctan.org/info/latex-refsheet/LaTeX_RefSheet.pdf)
This one is a summary of almost every basic function of LaTex in one document. It is very densly packed and mostly text so don't skim this pdf too quickly. Being one of my first sites I used as a cheat sheet I can recommend it with a good concience. You can copy the document into your LaTex file and just edit it. Or just copy single sections as this one goes over most stuff one by one - organized in section - and compiles it as one LaTex document in the end. However soon you'll realize you don't need to look up most stuff you used in here as it is very basic and LaTex is rather easy to get into. So long story short: Easy Introduction, but not that much more.
## [Pgf-Plots](https://github.com/hengxin/cheat-sheets/blob/master/latex/latex-pgfplots-cheat-sheet.md)
One of my favorite packages to use in LaTex is this one. With this you can create beautiful graphs in LaTex. The reason I started learning LaTex were those beautiful aligned graphs and I was not dissapointed when I started using this package. However I'm not skilled enough to create a graph from scratch, so I just modify the examples provided from [Overleaf](https://www.overleaf.com/learn/latex/Pgfplots_package). Just look into it and enjoy the beautiful graphs ;)
### Example
This is one graph I used in my phsics protocol.
```latex
\begin{figure}[h!]
    \centering
    \begin{tikzpicture}
        \begin{axis}[
            title={Stromstärke im Verhältnis zur Spannung},
            xlabel={Spannung [V]},
            ylabel={Stromstärke [mA]},
            xmin=0, xmax=20,
            ymin=0, ymax=20.1,
            xtick={0,2.5,5,7.5,10,12.5,15,17.5,20},
            ytick={0,2.5,5,7.5,10,12.5,15,17.5,20},
            legend pos=north west,
            ymajorgrids=true,
            grid style=dashed,
        ]
            
        \addplot[
            color=blue,
            mark=square,
            ]
            coordinates {
            (0,0)(0.5,1.6)(0.5,1.6)(1,2.6)(1.5,3)(2,3.7)(4,5.7)(6,7.3)(8,8.8)(10,10.1)(12,11.3)(14,12.5)(16,13.6)(18,14.6)(20,15.6)
            };
    
        \addplot[
            color=orange,
            mark=triangle,
            ]
            coordinates {
            (0,0)(0.5,0.5)(1,1)(1.5,1.49)(2,2)(4,4)(6,6)(8,8)(10,10.02)(12,12.03)(14,14.04)(16,16.05)(18,18.09)(20,20.1)         
            };
            \legend{Glühbirne, Widerstand}
                
        \end{axis}
        \end{tikzpicture}
    \caption{I-U-Diagramm}\label{U-I}
\end{figure}
```
![image](https://github.com/templeosuser/latexonlinetools/assets/151489154/f47fc41f-4329-405b-b6e4-59a9db3acc0b)

The Graph in its full glory.
