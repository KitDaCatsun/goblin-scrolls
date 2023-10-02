# The Goblin Scrolls

The official Computer Science Scrolls.

## Downloading

Click [here](https://gitlab.com/kitdacatsun/goblin-scrolls/-/jobs/artifacts/master/download?job=build) to download the Scrolls in PDF form.

# Code Snippets

## Equations

For single equations:

```tex
\begin{equation*}
    \theta = \frac{l}{r}
\end{equation*}
```

For multiple, related, equations:

```tex
\begin{align*}
    \Re(a+bi) & = a \\
    \Im(a+bi) & = b
\end{align*}
```

If equations need to be referenced, remove the `*` and add a `label{eq:label}`. In aligned equations, use `\\nonumber` to only number select equations.

## Figures

```tex
\begin{figure}[htbp]
    \centering
    \includegraphics[width=0.75\textwidth]{ECMXXXX/images/image_name.jpg}
    \caption{Figure Caption}
    \label{fig:label}
\end{figure}
```

Consider producing a graph with `pgfplots` or an image with `tikz` instead of using an image.

## Tables

```tex
\begin{table}[htbp]
    \centering
    \begin{tabular}{ll}
        \toprule
        Header 1 & Header 2 \\
        \midrule
        Cell 1-1 & Cell 1-2 \\
        Cell 2-1 & Cell 2-2 \\
        Cell 3-1 & Cell 3-2 \\
        \bottomrule
    \end{tabular}
    \caption{Table Caption}
    \label{tab:label}
\end{table}
```

Consider aligning columns with `c` instead of `l` in some situations.

## References

To reference a label, use the `cleverref` package. `\cref{label}` inserts a reference, and `\Cref{label}` capitalises the first letter of the type. Multiple references can be made at once by separating the labels with commas: `\cref{label1, label2, ...}` or `\Cref{label1, label2, ...}`.

## Logical Arguments

```tex
    \begin{equation*}
        \begin{array}{r l}
                       & p \rightarrow q \\
                       & p               \\
            \cline{2-2}
            \therefore & q
        \end{array}
    \end{equation*}
```
