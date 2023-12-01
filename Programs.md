# My Programs
Here are my Apps I use to create my LaTex Documents
## LaTex Editor
This might be controversial but I use VS Code as my LaTex Editor. I use the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) and the [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) Extensions to Tex and Spell Check my LaTex Documents.
I enrolled in a LaTex Course from my University and they recommended TexStudio or Overleaf. However I like to edit all my files in one Application. Therefore I looked for an Extension for VS Code and found this one. The setup is a bit more complicated as you need Perl and some extra Packages is you use MikTex like me. However it works really well and even Texes the Latex files twice if you use bib(la)tex.

The best feature however is the intellisense and autocomplete. You don't need to type
```latex
\begin{equation}
  E = mc^2
\end{equation}
```
All you need to do is type
```latex
\equation
```
and hit enter and it will create all the stuff you need automatically. Overall VS Code might be slower than TexStudio, but I'm lazy and like this one.
### Addition:
If you don't want Microsoft stealing your data with VS Code Telemetry just download VS Codium. I tried this one on my laptop and it works just as well as VS Code. VS Codium is based on the Open-Source framework that Microsoft uses for VS Code but they removed everything Telemetry related. (Please don't quote me on this and look it up yourself [here](https://vscodium.com/)
## Bibliography Database
Trying to write your bibliography file by hand is way too tideous for me so I use JabRef. Just look your sources up on e. g. Google Scholar and export for bib(la)tex and copy that into a new entry that JabRef creates. Simple and elegant. Don't forget to Tex your LaTex document twice tho.
