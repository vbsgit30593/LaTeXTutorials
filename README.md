# LaTeXTutorials
Some basic kickstarter stuff for LaTeX beginners
Info


\documentclass[]{article}
* File starts with a \
    * Article here specifies the type of article
        * If beamer then slides
        * If exam - used to create tests and quizzes
* [] are for optional arguments
    * Like font size
        * \documentclass[11pt]{article}

##################################
\begin{document}
Hello! This is my first \LaTeX\ document
\end{document}

The letter X is actually a greek letter Chi which sounds like K!! 

\begin{document}
Hello! This is my first \LaTeX\ document.

A rectangle has side lengths of (x+1) and (x+3)
\end{document}
##################################

Hard return - empty line to move text to newline
This creates a new paragraph
* Indented

\begin{document}
Hello! This is my first \LaTeX\ document.\\
A rectangle has side lengths of (x+1) and (x+3)
\end{document}

Soft return - \\ at the end of the line

A rectangle has side lengths of $(x+1)$ and $(x+3)$
Math mode
The equation $A(x) = x^2 + 4x + 3$ gives the area of the rectangle

Displayed Math mode
* In displayed mode, everything will be in its own line
$${A(x) = x^2 + 4x + 3}$$

Two dollar signs

Inline math mode
* Single dollar sign - Same line
##################################
Linebreaks
$$\frac{x}{y}$$
About $\frac{2}{3}$ of the glass is full.\\[16pt]
About $\displaystyle\frac{2}{3}$ of the glass is full.

#########################################

Brackets

The distributive property states that $a(b + c) = ab + ac$, $\forall a,b,c \in \mathbb{R}$.
\parindent 0px - don’t indent

$$2\left(\frac{1}{x^2 - 1}\right)$$
* For bigger brackets
$$2\left(\frac{1}{x^2 - 1}\right)$$
$$2\left[\frac{1}{x^2 - 1}\right]$$
$$2\left\{\frac{1}{x^2 - 1}\right\}$$


￼

$$2\left \langle \frac{1}{x^2 - 1}\right \rangle$$

$$\left. \frac{dy}{dx}\right|_{x=1}$$


Tables
\begin{tabular}{cccccc}. Or {llll} or {rrrr}
* Center aligned


Tables:\\[6pt]
\begin{tabular}{|c||c|c|c|c|c|}
\hline
$x$ & 1 & 2 & 3 & 4 & 5\\ \hline
$f(x)$ & 10 & 11 & 12 & 13 & 14 \\ \hline
\end{tabular}


￼
\begin{table}[H]
\centering
\def\arraystretch{1.5}

To adjust size of columns

\caption{Table of entries}
To add table captions

\begin{tabular}{|l|p{4in}|}
* Specifies that the column is a paragraph of a particular size
* 


Arrays
\begin{align}
5x^2 -9=x+3\\
5x^2 - x - 12 = 0
\end{align}

\begin{align}
5x^2 -9&=x+3\\
5x^2 - x - 12 &= 0\\
&=12+x-5x^2
\end{align}

& is used to keep = inline
Numbering follows

\begin{align*}
5x^2 -9&=x+3\\
5x^2 - x - 12 &= 0\\
&=12+x-5x^2
\end{align*}

Align* stops numbering


Creating lists

\begin{enumerate}
\begin{itemize}

\begin{enumerate}[A.]
* Use A B C D rather than 1 2 3 4

\begin{enumerate}\setcounter{enumi}{5}
* Start from 6

\begin{enumerate}
\item[] pencil
\item[] calculator
\item[] ruler
\item[] notebook
\end{enumerate}

item[] Skips numbering

Working with text formatting

This will produce \textit{italicized} text

This will produce \textbf{bold face} text

This will produce \textsc{small caps} text

This will produce \texttt{typewriter font} text

Please visit my linkedin url \texttt{www.linkedin.com/in/vaibhavsingh299}

Please visit my linkedin url \url{http://www.linkedin.com/in/vaibhavsingh299}

Please visit my linkedin url \href{http://www.linkedin.com/in/vaibhavsingh299}{Mylinkedin}


￼

Font sizes

Please excuse my dear aunt Sally

Please excuse my \begin{large}dear aunt Sally\end{large}

Please excuse my \begin{Large}dear aunt Sally\end{Large}

Please excuse my \begin{LARGE}dear aunt Sally\end{LARGE}

Please excuse my \begin{huge}dear aunt Sally\end{huge}

Please excuse my \begin{Huge}dear aunt Sally\end{Huge}

Please excuse my \begin{normalsize}dear aunty Sally\end{normalsize}

Please excuse my \begin{small}dear aunty Sally\end{small}

Please excuse my \begin{scriptsize}dear aunty Sally\end{scriptsize}

Please excuse my \begin{tiny}dear aunty Sally\end{tiny}

￼


Titles, author, date

\title{Working with text formatting}
\author{Vaibhav Singh}
\date{\today}
\begin{document}
\maketitle

Text justification
\begin{center}This line is centered\end{center}

\begin{flushleft}This line is left justified\end{flushleft}

\begin{flushright}This line is right justified\end{flushright}

Sections and subsections
\section{Linear Functions}
	\subsection{Slope intercept form}
		\subsubsection{Example 1}
		\subsubsection{Example 2}
	\subsection{Standard form}
	\subsection{Point slope form}

Table of contents

\tableofcontents
Needs to be compiled twice

Working with packages

\documentclass[10pt, letterpaper]{article}
\documentclass[10pt, a4paper]{article}

\usepackage{fullpage}
* To use the full page and eliminate extra margin

\usepackage[margin=1in]{geometry}
* 1 inch margins

\usepackage[top=1in, bottom=1in, left=0.75in, right=0.75in, paperwidth=5in, paperheight=7in]{geometry}

Macros
\def\eq1{y=\dfrac{x}{3x^2 + x + 1}}

Including images 
\usepackage{graphicx}

\includegraphics[scale=1]{pennstate}
* The file is pennstate.png but we don’t need to specify the extension
%\includegraphics[scale=1]{pennstate}
%\includegraphics[width=3.5in, height=4in]{pennstate}
\begin{center}
\includegraphics[width=0.4 \textwidth]{pennstate}
\end{center}


\begin{figure}[h]   %here
\includegraphics[width=0.4 \textwidth]{pennstate}
\end{figure}

\usepackage{float}


Image centering with location set to here
\begin{figure}[H]
\centering
\includegraphics[width=0.4 \textwidth]{pennstate}\\
\caption{This is a caption}
\end{figure}




