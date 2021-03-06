---
# Please do not delete --- above :) 

# ========================================================================
# Automatically edited by GitHub actions, please do not modify     | START 
# ==============================================================
report_url: https://github.com/r03ert0/bptest

last_changed: 2020-11-15 13:49 UTC

auth_created: r03ert0
# ===============================================================  | END 

title:  'The Chemical Basis of Morphogenesis'
url: https://github.com/r03ert0/bptest 
affiliations:
- id: aff1
  orgname: 'University of Manchester'
  city: Manchester
  country: United Kingdom

author:
- initials: AT
  surname: Turing
  firstname: Alan
  email: alan.turing@manchester.ac.uk
  affiliation: aff1
  corref: aff1

summary: It is suggested that a system of chemical substances, called morphogens, reacting together and diffusing through a tissue, is adequate to account for the main phenomena of morphogenesis. Such a system, although it may originally be quite homogeneous, may later develop a pattern or structure due to an instability of the homogeneous equilibrium, which is triggered off by random disturbances. Such reaction-diffusion systems are considered in some detail in the case of an isolated ring of cells, a mathematically convenient, though biologically unusual system. The investigation is chiefly concerned with the onset of instability. It is faund that there are six essentially different forms which this may take. In the most interesting form stationary waves appear on the ring. It is suggested that this might account, for instance, for the tentacle patterns on Hydra and for whorled leaves. A system of reactions and diffusion on a sphere is also considered. Such a system appears to account for gastrulation. Another reaction system in two dimensions gives rise to patterns reminiscent of dappling. It is also suggested that stationary waves in two dimensions could account for the phenomena of phyllotaxis. The purpose of this paper is to discuss a possible mechanism by which the genes of a zygote may determine the anatomical structure of the resulting organism. The theory does not make any new hypotheses; it merely suggests that certain well-known physical laws are sufficient to account for many of the facts. The full understanding of the paper requires a good knowledge of mathematics, some biology, and some elementary chemistry. Since readers cannot be expected to be experts in all of these subjects, a number of elementary facts are explained, which can be found in text-books, but whose omission would make the paper difficult reading.

tags:
  - Morphogenesis
  - Development
  - Simulation

supplemental:
  - name: Original manuscript
    url: https://www.jstor.org/stable/92463

coi: The author certifies he has no affiliations with or involvement in any organization or entity with any financial interest in the subject matter or materials discussed in this manuscript.

acknow: The author would like to thank Ada Lovelace for her insightful comments on the nature of intelligence and the mind.

contrib: AT wrote the software, performed tests, and wrote the report.

binder: false

hypothesis: false

# Please do not delete --- below :) 
---

# 1. A model of the embryo. Morphogens.

In this section a mathematical model of the growing embryo will be described. This model will be a simplification and an idealization, and consequently a falsification. It is to be hoped that the features retained for discussion are those of greatest importance in the present state of knowledge.
The model takes two slightly different forms. In one of them the cell theory is recognized but the cells are idealized into geometrical points. In the other the matter of the organism is imagined as continuously distributed. The cells are not, however, completely ignored, for various physical and physico-chemical characteristics of the matter as a whole are assumed to have values appropriate to the cellular matter.
With either of the models one proceeds as with a physical theory and defines an entitycalled 'the state of the system'. One then describes how that state is to be determined from the state at a moment very shortly before. With either model the description of the state consists of two parts, the mechanical and the chemical. The mechanical part of the state describes the positions, masses, velocities and elastic properties of the cells, and the forces between them. In the continuous form of the theory essentially the same information is given in the form of the stress, velocity, density and elasticity of the matter. The chemical part of the state is given (in the cell form of theory) as the chemical composition of each separate cell; the diffusibility of each substance between each two adjacent cells rnust also be given. In the continuous form of the theory the concentrations and diffusibilities of each substance have to be given at each point. In determining the changes of state one should take into account

\begin{enumerate}
  \item The changes of position and velocity as given by Newton's laws of motion.
  \item The stresses as given by the elasticities and motions, also taking into account the
osmotic pressures as given from the chemical data.
  \item The chemical reactions.
  \item The diffusion of the chemical substances. The region in which this diffusion is possible is given from the mechanical data.
\end{enumerate}

This account of the problem omits many features, e.g. electrical properties and the internal structure of the cell. But even so it is a problem of formidable mathematical complexity. One cannot at present hope to make any progress with the understanding of such systems except in very simplified cases. The interdependence of the chemical and mechanical data adds enormously to the difficulty, and attention will therefore be confined, so far as is possible, to cases where these can be separated. The mathematics of elastic solids is a welldeveloped subject, and has often been applied to biological systems. In this paper it is proposed to give attention rather to cases where the mechanical aspect can be ignored and the chemical aspect is the most significant. These cases promise greater interest, for the characteristic action of the genes themselves is presumably chemical. The systems actually to be considered consist therefore of masses of tissues which are not growing, but within which certain substances are reacting chemically, and through which they are diffusing.

These substances will be called morphogens, the word being intended to convey the idea of a form producer. It is not intended to have any very exact meaning, but is simply the kind of substance concerned in this theory. The evocators of Waddington provide a good example of morphogens \cite{waddington1940organisers}.These evocators diffusing into a tissue somehow persuade it to develop along different lines from those which would have been followed in its absence. The genes themselves may also be considered to be morphogens. But they certainly form rather a special class. They are quite indiffusible. Moreover, it is only by courtesy that genes can be regarded as separate molecules. It would be more accurate (at any rate at mitosis) to regard them as radicals of the giant molecules known as chromosomes. But presumably these radicals act almost independently, so that it is unlikely that serious errors will arise through regarding the genes as molecules. Hormones may also be regarded as quite typical morphogens. Skin pigments may be regarded as morphogens if desired. But those whose action is to be considered here do not come squarely within any of these categories.

The function of genes is presumed to be purely catalytic. They catalyze the production of other morphogens, which in turn may only be catalysts. Eventually, presumably, the chain leads to some morphogens whose duties are not purely catalytic. For instance, a substance might break down into a number of smaller molecules, thereby increasing the osmotic pressure in a cell and promoting its growth. The genes might thus be said to influence the anatomical form of the organism by determining the rates of those reactions which they catalyze. If the rates are assumed to be those determined by the genes, and if a comparison of organisms is not in question, the genes themselves may be eliminated from the discussion. Likewise any other catalysts obtained secondarily through the agency of the genes may equally be ignored, if there is no question of their concentrations varying. 

There may, however, be some other morphogens, of the nature of evocators, which cannot be altogether forgotten, but whose role may nevertheless be subsidiary, from the point of view of the formation of a particular organ. Suppose, for instance, that a 'leg-evocator' morphogen were being produced in a certain region of an embryo, or perhaps diffusing into it, and that an attempt was being made to explain the mechanism by which the leg was formed in the presence of the evocator. It would then be reasonable to take the distribution of the evocator in space and time as given in advance and to consider the chemical reactions set in train by it. That at any rate is the procedure adopted in the few examples considered here.

# 2. Mathematical background required

The greater part of this present paper requires only a very moderate knowledge of mathematics. What is chiefly required is an understanding of the solution of linear differential equations with constant coefficients. (This is also what is chiefly required for an understanding of mechanical and electrical oscillations.) The solution of such an equation takes the form of a sum $\sum{A e^{bt}}$, where the quantities $A$, $b$ may be complex, i.e. of the form $\alpha + i \beta$, where $\alpha$ and $\beta$ are ordinary (real) numbers and $i = \sqrt{-1}$. It is of great importance that the physical significance of the various possible solutions of this kind should be appreciated, for instance, that

\begin{enumerate}
  \item Since the solutions will normally be real one can also write them in the form $R \sum {A e^{bt}}$ or $\sum {A e^{bt}}$ ($R$ means 'real part of').
  \item That if $A = A' e^{i \psi}$ and $b = \alpha + i \beta$, where $A'$, $\alpha$, $\psi$, are real, then $R A e^{bt} = A' e^{\alpha t} cos (\beta t+ \psi)$.
\end{enumerate}

Thus each such term represents a sinusoidal oscillation if $\alpha = 0$, a damped oscillation if $\alpha < 0$, and an oscillation of ever-increasing amplitude if $\alpha>0$. 

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
