# Repositorio de Cursos

## Curso de LaTex para principiantes.

**Código básico**

```latex
\documentclass{article}
%\usepackage[spanish]{babel}
\usepackage[utf8]{inputenc} % nos ayuda a escribir tildes y acentos
\usepackage{enumitem}
\title{Our First Document}
\author{Alfonso Fajardo}
\date{}

\begin{document}
% This is a comment
\maketitle % inserta los datos del título
\section{Introductory section} % crea una sección
This is the introductory section of this document
\subsection{Second level subsection} % crea una subsección
This is the second level subsection
\subsubsection{Thirthlevel subsection}
This is the thirth livel subsection
% Bold
this \textbf{word} is in \textbf{bold} font. \\
% Italic
My name \emph{Alfonso Fajardo} is in \emph{italic} \\
%Underline
this \underline{word} will be \underline{underlined}.
% insertar lineas en blanco tambien puede hacerse dejando una en blanco

\noindent hola a todos % no indent evitará que haya un espacio al principio de la linea
Este documuento pertenece a "Alfonso" \\ % las comillas estarán mal acomodadas 
``Esta es la forma correcta de poner comillas" \\
`Así se ponen las comillas sencillas'

% Bullet form
\begin{itemize}
\item first text
\item Second text
\item Third text
\end{itemize}

% Number list
\begin{enumerate}
\item First
\begin{enumerate}
\item first level first line
\item first level second line
\item first level thirth line
\end{enumerate}
\item Second
\item Third
\end{enumerate}

% describir algunos items
\begin{description}
\item [Kate] Some detail 
\item [Christina] Some detail
\end{description}

% Be sure that enumitem package is loaded.to prevent item separation line you can do:
\begin{description}[noitemsep] % pay attention to this line
\item [Kate] Some detail 
\item [Christina] Some detail
\end{description}

%alignment options
\begin{description}[align=right]

\item [Kate] Some detail 
\item [Christina] Some detail
\end{description}
% Create tables
\noindent \begin{tabular}{cc}
Entity & Description \\% & sign separetes elements from different collums
A & This is A \\
B & This is B\\
\end{tabular}

% Create table  with lines 
\begin{tabular}{|c|c|}
\hline
Entity & Description \\
\hline % linea horizontal
A & this is A \\
\hline
A & this is B \\
\hline
\end{tabular}


%doble lines
\begin{tabular}{||c||c||}
\hline\hline
Entity & Description \\
\hline\hline % linea horizontal
A & this is A \\
\hline\hline
A & this is B \\
\hline\hline\hline% Doble lines table
\end{tabular}

% Table environment
This is the table with the floating environtment
\vspace{0.5cm}
\begin{table}[p]
\caption{This is my first table}
\begin{centering}
\begin{tabular}{||c||c||}
\hline\hline
Entity & Description \\
\hline\hline % linea horizontal
A & this is A \\
\hline\hline
A & this is B \\
\hline\hline\hline% Doble lines table
\end{tabular}


\end{centering}
\label{first_table}
\end{table}

% Refer to table

I want to refer to my table which is Table ~\ref{first_table}


\end{document}

% Advance table techinques

```
