---
# pandoc main.md -H preamble.tex -t beamer -o main.pdf --slide-level=2
title:
- Pandoc Tutorial
author: 
- Do Hoang
date: \today{}
institute: 
-  The Code Cousins
theme:
- Ilmenau
colortheme:
- default 
innertheme:
- circles 
header-includes:
- \newcommand{\hideFromPandoc}[1]{#1}
- \hideFromPandoc{
    \let\Begin\begin
    \let\End\end
  }
mainfont: sfdefault
toc: 
- true
---
# Section heading 1 slide
## Slide 1 of Section 1 
- This is a list 
- Another list item
- etc,...

![Image example](arduino.png){ width=50% }

# Section heading 2
## Slide 2 of Section 2

\Begin{columns}
\Begin{column}{0.5\textwidth}

- Arduino UNO:
	- Microcontroller board
	- Provides electricity to the sensors
	- Collects data directly from the sensors
	- Delivers the data

\End{column}
\Begin{column}{0.5\textwidth}

![Arduino UNO-R3](arduino.png)

\End{column}
\End{columns}