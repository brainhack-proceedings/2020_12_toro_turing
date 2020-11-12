---
# Please do not delete --- above :) 

# ========================================================================
# Automatically edited by GitHub actions, please do not modify     | START 
# ==============================================================
report_url: https://github.com/r03ert0/bptest

last_changed: 2020-11-12 17:58 UTC

auth_created: r03ert0
# ===============================================================  | END 

title:  'An automagical report generator for BrainHack Proceedings'
url: https://github.com/username/project_repository 
affiliations:
- id: aff1
  orgname: 'Research Lab 1, Organization 1'
  street: street_name_goes_here 
  postcode: post_code_goes_here
  city: Montreal
  state: Quebec
  country: Canada

author:
- initials: JD
  surname: Doe
  firstname: Jane
  email: janedoe@gmail.com
  affiliation: aff1
  corref: aff1

summary: It is suggested that a system of chemical substances, called morphogens, reacting together and diffusing through a tissue, is adequate to account for the main phenomena of morphogenesis. Such a system, although it may originally be quite homogeneous, may later develop a pattern or structure due to an instability of the homogeneous equilibrium, which is triggered off by random disturbances. Such reaction-diffusion systems are considered in some detail in the case of an isolated ring of cells, a mathematically convenient, though biologically unusual system. The investigation is chiefly concerned with the onset of instability. It is faund that there are six essentially different forms which this may take. In the most interesting form stationary waves appear on the ring. It is suggested that this might account, for instance, for the tentacle patterns on Hydra and for whorled leaves. A system of reactions and diffusion on a sphere is also considered. Such a system appears to account for gastrulation. Another reaction system in two dimensions gives rise to patterns reminiscent of dappling. It is also suggested that stationary waves in two dimensions could account for the phenomena of phyllotaxis. The purpose of this paper is to discuss a possible mechanism by which the genes of a zygote may determine the anatomical structure of the resulting organism. The theory does not make any new hypotheses; it merely suggests that certain well-known physical laws are sufficient to account for many of the facts. The full understanding of the paper requires a good knowledge of mathematics, some biology, and some elementary chemistry. Since readers cannot be expected to be experts in all of these subjects, a number of elementary facts are explained, which can be found in text-books, but whose omission would make the paper difficult reading.

tags:
  - tag1
  - tag2
  - tag3

# Please comment out the following 5 lines if you have no supplemental material.
supplemental:
  - name: Material 1
    url: https://osf.io 
  - name: Material 2 
    url: https://zenodo.org 

coi: Please add if there are competing interests. Otherwise, type None.

acknow: The authors would like to thank the organizers and attendees of OHBM Brainhack 2020.

contrib: JD and JJD wrote the software, JD performed tests, and JD and JJD wrote the report.

# Please comment out the following 4 lines if no reviewer has been assigned to you yet.
reviewers:
  - name: Agah
    surname: Karakuzu
    gh_handle: agahkarakuzu

# Show/hide the BinderHub (mybinder.org) badge
# Accepted values: true/false (case sensitive)
# -------------------------------------------
binder: true

# Enable/disable hypothes.is
# Accepted values: true/false (case sensitive)
hypothesis: true

# Please do not delete --- below :) 
---

# Introduction
The bibliography \code{report.bib} must respect \href{http://www.bibtex.org/Using/}{BibTeX} format. 
You can cite entries in your bibliography using their tags:

\begin{itemize}
  \item Cite an article: \cite{author:2010}
  \item Cite a GitHub repository: \cite{githubrepo:2020}
\end{itemize}

\smallskip
\noindent You can use \code{inline code highlight}. This paragraph shows how to add blank lines and how to start a paragraph without indentation.

Remember that this is a LaTex flavored markdown. Therefore, some characters must be used with an escape character within the text:

\code{\& \% \$ \# \_ \{  \} \textbackslash}


# Section
You can create additional sections as you prefer. Section title levels are determined by the number of hastags as in a traditional markdown file.

## Subsection
Subsection content goes here. You can create numerated lists:

\begin{enumerate}
  \item The labels consists of sequential numbers.
  \item The numbers starts at 1 with every call to the enumerate environment.
\end{enumerate}

### Equations & formulas
You can add mathematical formulas. Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{\pi/x}$.
\smallskip

\noindent You can also use plain LaTeX for equations. These equations are rendered by MathJax, you can right click on them and explore the rendering options available at your browser!

\begin{equation} \label{eq:1}
\hat f(\omega) = \int_{-\infty}^{\infty} f(x) e^{i\omega x} dx
\end{equation}

and refer to \ref{eq:1} from text.

### Hypothes.is 
We enabled \href{https://web.hypothes.is/}{hypothes.is} for the brainhack proceeding reports. This way, you can annotate, highlight and tag the content collaboratively! You may choose to share your insights with everyone, or keep them private.      

# Results
Figure files must be placed at the \code{figures} folder. You can include figures using the following block:

\begin{figure}[h!]

  \includegraphics[width=.47\textwidth]{brainhack.png}

  \caption{\label{Figure-1} Your caption goes here.}

\end{figure}

Note that \code{width=.47 \textbackslash textwidth} above sets scales the figure size in the PDF. To change attributes of the figures on the webpage, please see \code{/figures/figures.css}. 

To refer a figure in the text, you need to use the respective label defined in its caption: Fig. \ref{Figure-1}
