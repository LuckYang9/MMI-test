# MMI-test
\documentclass{article}
\usepackage[utf8]{inputenc}

\title{Research on Silicon based Multimode Interference Couplers}
\author{Yunhong Yang }
\date{December 2023}


\usepackage{natbib}
\usepackage{graphicx}
\usepackage{amsmath}

\begin{document}

\maketitle

\section{Introduction}
The on-chip mode multiplexing system carries transmitted signals in multiple intrinsic modes, which can effectively improve the bandwidth of system transmission and has the advantages of small size and high integration. Building on-chip mode multiplexing systems requires many basic components, among which multi-mode power dividers can simultaneously achieve power allocation across multiple modes through multiple ports, with high requirements for port power consistency, bandwidth characteristics, low loss characteristics, and so on.\citep{adams1995hitchhiker}


\section{simulation}
To reduce the size, we can use only the first three modes to excite, which can reduce the width to 2.6 microns. At this point, symmetric interference only generates 0 and 2nd order modes, and the effective refractive index is calculated.n0=3.257201 and n1=3.216834. L=19.2microns. The corresponding MMI length should be 7.2 microns.At x=3L/8, the light intensity will be uniform divided into two parts.





\begin{figure}[h!]
\centering
\includegraphics[scale=0.6]{fig.1.png}
\caption{MMI profile}
\label{fig:MMIprofile}
\end{figure}

Scanning the length of the mmi to find the best advantage, it was ultimately found that the spectral effect is best at a length of 4.21 microns.

\begin{figure}[h!]
\centering
\includegraphics[scale=0.4]{fig.2.png}
\caption{MMI Length}
\label{fig:MMILength}
\end{figure}


Scan the width of the input and output taper to obtain the most effective value.

\begin{figure}[h!]
\centering
\includegraphics[scale=0.4]{fig.3.png}
\caption{Taper Width}
\label{fig:Taper Width}
\end{figure}

\section{Conclusion}
After careful simulation scanning, it was finally found that the range was between 0.85-0.9 microns. The best effect is achieved when the MMI length is 4.21 microns. The transmittance of each output reaches 0.48 or above.



\bibliographystyle{plain}
\bibliography{references}

\end{document}
