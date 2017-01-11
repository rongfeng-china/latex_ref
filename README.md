# latex_ref
Create a refs.bib file with all the BibTeX entries, which are easily available from Google Scholar or similar

Create a “dummy” .tex file with the following entries:

\documentclass{article}
\begin{document}
\nocite{*}
\bibliography{refs}
\bibliographystyle{plain}
\end{document}

Now, do the following:

$ latex dummy
$ bibtex dummy
$ bibtex dummy
$ latex dummy

You will see a dummy.bbl file containing all your BibTeX entries in \bibitem format.
