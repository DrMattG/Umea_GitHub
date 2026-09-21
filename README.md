# GitHub and Quarto for open and reproducible research

Materials for a hands-on workshop introducing GitHub and Quarto through a
small wildlife-research example.

The workshop is designed for researchers who are new to GitHub. No previous
experience with Git, GitHub or Quarto is required. We will use RStudio as the
main interface so that participants can concentrate on the workflow rather
than memorising terminal commands.

## Workshop aims

By the end of the workshop, participants should be able to:

- explain the difference between Git and GitHub;
- clone a GitHub repository to their computer;
- inspect, commit, push and pull changes using RStudio;
- create and render a reproducible Quarto report;
- use a parameter to generate different versions of a report; and
- recognise when branches, issues and pull requests are useful.

## Umeå workshop

The Umeå session is approximately 2.5 hours and focuses on three parts of the
larger workshop:

| Approximate time | Session | Main activity |
|---:|---|---|
| 10 min | Welcome and setup check | Confirm access to GitHub, Git, RStudio and Quarto |
| 20 min | GitHub without fear | Repositories, commits and the local–remote workflow |
| 45 min | Guided Git exercise | Clone, edit, inspect, commit, push and pull |
| 10 min | Break |  |
| 15 min | Quarto introduction | Combine narrative, code, results, figures and tables |
| 25 min | Quarto exercise | Edit and render a wildlife report |
| 15 min | Parameterised reports | Generate reports for different habitats |
| 10 min | Collaboration | Issues, branches and a pull-request demonstration |

Timings are approximate and may be adjusted to allow time for setup and
questions.

## Workshop materials

The `slides/` directory contains the complete set of workshop presentations:

1. **GitHub without fear** — repositories, commits, push and pull
2. **Quarto reports** — reproducible documents combining text and computation
3. **Collaboration** — issues, branches and pull requests


## Repository structure

```text
Open_wildlife_workshop/
├── slides/                       # Quarto source files for the slides
│   └── images/                   # Images used in the slide decks
├── wildlife_report_template.qmd  # Student Quarto exercise
├── index.qmd                     # Workshop website landing page
├── _quarto.yml                   # Quarto project configuration
├── style.css                     # Workshop website styling
├── Open_wildlife_workshop.Rproj  # RStudio project file
├── README.md                     # This file
└── LICENSE                       # Reuse licence
```

The `docs/` directory contains rendered website files. These are generated
from the source files and normally should not be edited by hand.

## Preparation

Before the workshop, please:

1. Create a free [GitHub account](https://github.com/signup).
2. Install [Git](https://git-scm.com/downloads).
3. Install a recent version of [R](https://cran.r-project.org/).
4. Install a recent version of
   [RStudio Desktop](https://posit.co/download/rstudio-desktop/).
5. Confirm that Quarto is available in RStudio.

Open the RStudio Terminal and run:

```bash
git --version
quarto check
```

Configure the name and email that Git will record with your commits:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Use the email address associated with your GitHub account.

## Getting the workshop materials

The repository can be cloned in RStudio:

1. On GitHub, click **Code** and copy the HTTPS repository URL.
2. In RStudio, select **File → New Project → Version Control → Git**.
3. Paste the repository URL.
4. Choose where to save the project and select **Create Project**.

The repository URL is:

```text
https://github.com/DrMattG/Umea_GitHub
```

## The Git workflow used in the workshop

We will repeatedly use this sequence:

```text
PULL → EDIT → INSPECT → COMMIT → PUSH
```

- **Pull** brings remote changes from GitHub to your computer.
- **Edit** means working on your local project files.
- **Inspect** checks exactly what has changed.
- **Commit** records a meaningful set of changes in the local Git history.
- **Push** sends your local commits to GitHub.

Example commit messages include:

```text
Add research interests to README
Create initial Quarto wildlife report
Parameterise report by habitat
Clarify instructions for rendering report
```

## Quarto exercise

Open `wildlife_report_template.qmd` in RStudio and click **Render**. The report
uses fictional wildlife-monitoring data and does not require access to an
external dataset.

## Further resources

- [Happy Git and GitHub for the useR](https://happygitwithr.com/)
- [Quarto documentation](https://quarto.org/docs/guide/)
- [GitHub documentation](https://docs.github.com/)
- [Software Carpentry: Version Control with Git](https://swcarpentry.github.io/git-novice/)

## Licence

The repository currently includes a [CC-BY 4.0 International](https://github.com/DrMattG/Umea_GitHub/LICENSE.md) licence. Check
that this is the licence you want before reusing or publishing the complete
workshop materials.
