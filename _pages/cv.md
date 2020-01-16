---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
% "ModernCV" CV and Cover Letter
% LaTeX Template
% Version 1.11 (19/6/14)
%
% This template has been downloaded from:
% http://www.LaTeXTemplates.com
%
% Original author:
% Xavier Danaux (xdanaux@gmail.com)
%
% License:
% CC BY-NC-SA 3.0 (http://creativecommons.org/licenses/by-nc-sa/3.0/)
%
% Important note:
% This template requires the moderncv.cls and .sty files to be in the same 
% directory as this .tex file. These files provide the resume style and themes 
% used for structuring the document.
%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%----------------------------------------------------------------------------------------
%	PACKAGES AND OTHER DOCUMENT CONFIGURATIONS
%----------------------------------------------------------------------------------------


\documentclass[11pt,a4paper,sans]{moderncv} % Font sizes: 10, 11, or 12; paper sizes: a4paper, letterpaper, a5paper, legalpaper, executivepaper or landscape; font families: sans or roman


\moderncvstyle{classic} % CV theme - options include: 'casual' (default), 'classic', 'oldstyle' and 'banking'
\moderncvcolor{purple} % CV color - options include: 'blue' (default), 'orange', 'green', 'red', 'purple', 'grey' and 'black'

\usepackage{lipsum} % Used for inserting dummy 'Lorem ipsum' text into the template

\usepackage[scale=0.8]{geometry} % Reduce document margins
%\setlength{\hintscolumnwidth}{3cm} % Uncomment to change the width of the dates column
\setlength{\makecvtitlenamewidth}{10cm} % For the 'classic' style, uncomment to adjust the width of the space allocated to your name


%----------------------------------------------------------------------------------------
%	NAME AND CONTACT INFORMATION SECTION
%----------------------------------------------------------------------------------------

\firstname{Pierre} % Your first name
\familyname{COLOMBO} % Your last name

% All information in this block is optional, comment out any lines you don't need
\title{PhD student in NLP}
\address{Paris 75013}{FRANCE}
\mobile{(+33) 650118518}
\email{colombo.pierre@gmail.com,pierre.colombo@telecom-paris.fr}
\homepage {Website: https://pierrecolombo.github.io/}
% \homepage {Scholar: www.linkedin.com/in/pierre-colombo}
% \homepage {LinkedIn: www.linkedin.com/in/pierre-colombo}
% \homepage{www.linkedin.com/in/pierre-colombo} {LinkedIn} % The first argument is the url for the clickable link, the second argument is the url displayed in the template - this allows special characters to be displayed such as the tilde in this example
% \homepage{https://pierrecolombo.github.io/}{Homepage}
%\extrainfo{DOB: September 15, 1997}
%\photo[70pt][0.4pt]{pictures/House} % The first bracket is the picture height, the second is the thickness of the frame around the picture (0pt for no frame)
%\quote{"A witty and playful quotation" - John Smith}
%----------------------------------------------------------------------------------------
\usepackage{bibentry}
\begin{document}
 \nobibliography{bib}
  \bibliographystyle{unsrt}
\makecvtitle % Print the CV title
%----------------------------------------------------------------------------------------
%	EDUCATION SECTION
%----------------------------------------------------------------------------------------
I am a first year PhD student in the SSA group at Telecom Paris and IBM in Paris. My PhD focuses on Deep Learning and Representation Learning applied to Natural Language and Dialog.
\section{Education}

\cventry{2018--2021}{Phd Student}{}{}{\textit{Department of Computer Science, Telecom Paris, Paris, France}}{}
\cventry{2016--2018}{MSC in Computer Science}{}{}{\textit{Department of Computer Science, EPFL, Lausanne, Switzerland}}{}
\cventry{2014--2018}{MSC in Applied Mathematics}{}{}{\textit{Department of Computer Science, CentraleSupelec, Paris, France}}{}
\cventry{2012--2014}{Preparatory School MPSI - MP*}{}{}{\textit{Lycee Condorcet, Paris, France}}{}



%----------------------------------------------------------------------------------------
%	INTERESTS SECTION
%----------------------------------------------------------------------------------------


% \renewcommand{\listitemsymbol}{-~} % Changes the symbol used for lists
% \cvlistdoubleitem{Piano}{}
% \cvlistitem{Baseball}

%----------------------------------------------------------------------------------------
%	Achievements SECTION
%----------------------------------------------------------------------------------------

\section{Experience}
\cvitem{2019}{6 Month - Lab Associate at \textbf{Disney Research, Los Angeles (USA)} working on Dialog Generation.}
\cvitem{2017-2018}{6 Month - Research Student at \textbf{IBM Research, Zurich (Swizerland)} Thesis entitled : Deciphering gene deregulation in cancer development using deep learning.}
\cvitem{2017}{6 Month - Research Student at \textbf{Swisscom Research, Lausanne (Swizerland)} working on chatbots.}
\cvitem{2016-2017}{12 Month - Teaching Assistant at \textbf{EPFL}, Lausanne (Swizerland) helping student to solve mathematics and physic exercises during exercise sessions.}
\cvitem{2017}{6 Month - Lab Assistant in the \textbf{Quantum Physic Department of EPFL, Lausanne (Swizerland)} developing various sensors algorithms (Python/C++).}
\cvitem{2017}{6 Month - Research Intern at \textbf{Procter \& Gamble, Frankfurt (Germany)}, development and implementation of a secure application (Android and IOs) to enable a smartphone user to update a toothbrush over-the-air.}
\cvitem{2014-2018}{20 Months - Software Consultant at \textbf{Supelec \& EPFL Junior Enterprise}, debugging web applications developed with Symphony 2 for the French Army, and developing several websites (\url{http://www.volumina-medical.ch/}).}
\cvitem{2014}{2 Months - Intern at \textbf{Safran Paris (France)}.}
% \runsubsection{Safran, Paris}
% \location{June. 2015 -- July. 2015}

% \runsubsection{Swisscom, Lausanne}
% \location{Feb. 2017 -- June 2017}
% \vspace{\topsep} % Hacky fix for awkward extra vertical space
% \begin{tightemize}
% \item  \href{https://github.com/fearnleymartin/knowledge-base/blob/master/Docs/report.pdf}{Machine Learning Intern working on chatbot}. Data obtain from web scraping. Machine Learning algorithms such LSTM, word2vec, PageRank have been used for information retrieval purposes.
% \item \textbf{Tools :}  Scrapy, Databases (Neo4j, Solr), tensorflow, TF-IDF
% \end{tightemize}
% \sectionsep


% \runsubsection{EPFL, Lausanne}
% \location{Feb. 2017 -- June 2017}
% \vspace{\topsep} % Hacky fix for awkward extra vertical space
% \begin{tightemize}
% \item  Development of various sensors algorithms (Python).
% \end{tightemize}
% \sectionsep


% \runsubsection{EPFL, Lausanne}
% \location{Sept. 2016 -- Dec. 2016}
% \vspace{\topsep} % Hacky fix for awkward extra vertical space
% \begin{tightemize}
% \item  Helping student to solve mathematics and physic exercises during exercise sessions.
% \end{tightemize}
% \sectionsep


% \runsubsection{Procter \& Gamble, Frankfurt}
% \location{June. 2016 -- Sept. 2016}
% \vspace{\topsep} % Hacky fix for awkward extra vertical space
% \begin{tightemize}
% \item Android \& IOS developer :  development and implementation of a secure application (Android and IOs) to enable a smartphone user to update a toothbrush over-the-air.
% \item \textbf{Tools :} Java, Swift, Cryptography
% \end{tightemize}


% \sectionsep
% \runsubsection{Supelec \& EPFL Junior Enterprise}
% \location{Sept. 2014 -- Nov. 2017}
% \vspace{\topsep} % Hacky fix for awkward extra vertical space
% \begin{tightemize}
% \item Debug a web application developed with Symphony 2 for the French Army.
% \item Development of several websites (\url{http://www.volumina-medical.ch/})
% \end{tightemize}
% \sectionsep


% \runsubsection{Safran, Paris}
% \location{June. 2015 -- July. 2015}


% \cvitem{Present}{Currently working in the Sponsorship team of  \textbf{TEDx IGDTU} one of the 36 team members in the university}
% \cvitem{Present} {Pursuing \textbf{Microsoft Authorized Certification } course in \textbf{Cross Platform Mobile App Development}}
% \cvitem{2017-18}{Headed the Enactus IGDTU as the\textbf{Project Leader}of Dharini project impacting the lives of \textbfup{1,500 underprivileged women}directly and indirectly}

% \cvitem{2017-18}{Fecilitated as the top 20 teams in \textbf{Enactus National Competition} for exceptional entrepreneurial action and social impact in field of \textbf{Menstrual Hygiene} and upliftment of \textbf{Rohingaya community} organised by KPMG India}
% \cvitem{2016-2017}{Recipient of the \textbf{Director's Special Award } and headed the student council as 'Prefect' of the school}
% \cvitem{2013}{ Felicitated with the prestigious \textbf{Aqua Award} for movie making on water conservation organised by the PVR CineArt and the Aqua Foundation}
% \cvitem{2014}{\textbf{State Winner of French Spell Bee}, Advanced Level organised by Paris based Le Frehindi Organisation}




%----------------------------------------------------------------------------------------
%	AWARDS SECTION
%----------------------------------------------------------------------------------------
%\section{Certifications}

%\cventry{April 2015 -- April 2017}{Certified LabVIEW Associate Developer}{\textsc{National Instruments}}{}{}{}


%----------------------------------------------------------------------------------------
%	Research SECTION
%----------------------------------------------------------------------------------------


%----------------------------------------------------------------------------------------
%	Techincal Projects SECTION
%----------------------------------------------------------------------------------------





%----------------------------------------------------------------------------------------
%	Course Projects SECTION
%----------------------------------------------------------------------------------------

\section{Publications}
  \begin{enumerate}
    \item \bibentry{DBLP:journals/corr/abs-1908-11215}
    \item \bibentry{DBLP:journals/corr/abs-1904-02793}
    \item \bibentry{DBLP:journals/corr/abs-1908-11216}
    \item \bibentry{DBLP:conf/wassa/WitonCMK18}
  \end{enumerate}


\section{Patents}
%----------------------------------------------------------------------------------------
%	Institute Positions SECTION
%----------------------------------------------------------------------------------------
  \begin{enumerate}
    \item Affect Driven Dialog Generation, Ashutosh Modi, Mubbasir Kapadia, Douglas A. Fidaleo, James R. Kennedy, Wojciech Witon and Pierre Colombo, US Patent Pending, A framework for Affective Conversational System
  \end{enumerate}


\section{Languages}

\cvitemwithcomment{English}{ Business fluent}{}
\cvitemwithcomment{French}{Native speaker}{}
\cvitemwithcomment{German}{Upper intermediate}{}
\section{Languages}

\cvitemwithcomment{Sport}{Handball, Athletics: marathons, ultra-trails}{}
\cvitemwithcomment{Music}{Studied music theory and trumpet for 12 years at conservatoire}{}
\cvitemwithcomment{Volunteer Work}{In charge of a Student Group which helps youths living in disadvantaged areas.}{}
\end{document}



