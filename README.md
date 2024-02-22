# typst-liuthesis

A [Typst](https://typst.app/) template for writing a bachelor's or master's
thesis at Linköping University (LiU). Based on
[liuthesis](https://gitlab.liu.se/olale55/liuthesis), and specifically
`demo_student_thesis.tex`.

I made this for my master's thesis, so it does not support all features of
`liuthesis` and may contain a number of bugs.

## Usage

Place this repo in a folder called `typst-liuthesis` in your Typst project.

The template can then be used as follows. See `template.typ` for an explanation
of each parameter.

```typst
#import "typst-liuthesis/template.typ": *

#show: liu.with(
  title: [LiU Thesis],
  subtitle: [A thesis template for Linköping University.],
  titleSwedish: [LiU Thesis],
  subtitleSwedish: [En mall för uppsatser vid Linköpings universitet.],
  authors: (
    "An Author",
    "Another Author"
  ),
  abstract: [This is the abstract.],
  bibliography-file: "references.bib",
  supervisor: "My Supervisor",
  examiner: "My Examiner",
)
```
