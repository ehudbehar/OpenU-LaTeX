<blockquote align="right">“You know you're brilliant, but maybe you'd like to understand what you did 2 weeks from now.”</blockquote>
<p align="right">— <i>Linux kernel coding style guide</i></p>

## Theorems
We have three groups of theorems:
1. ruled (or framed) envs – הגדרה, משפט, למה, טענה, מסקנה
2. regular envs – דוגמה, דוגמאות, שאלה, שאלה עם רמז
3. end of volume envs – תשובה, רמז

The first groups needs an `\hrule` above and below each environment, the second need a glue of `\parskip` above the environment, and the third is a stacked list of environments one after the other.

When we say `\begin{corollary}...\end{corollary}`, we want TeX to insert something like this:
```
\theoremstyle{thms}% activate style
\newtheorem{corollary@thm}[definition]{מסקנה}
\newenvironment{corollary}[1][]%
  {\thmframe@open % macro that inserts the hrule above
  \begin{corollary@thm}[#1]}%
  {\end{corollary@thm}
  \thmframe@close} % hrule
```