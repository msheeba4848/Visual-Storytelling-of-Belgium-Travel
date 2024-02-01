# Assignment: Write a data driven story

<div>

> **Note**
>
> Please read all the instructions here carefully before proceeding.

</div>

## Assignment overview

For this assignment, you will write a short data-driven story thinking
about the ideas discussed this week in class. You will use the [provided
dataset](#the-dataset). You will create the visualizations to support
your story.

- 3 to 5 vizs
- focus on author driven
- read the segel/heer paper and choose a genre (warnign, some genres may
  be more complicated to imeplement)

This [Harvard Business Review blog
post](https://online.hbs.edu/blog/post/data-storytelling) provides a
good summary of the components required for data storytelling:

- **Data:** Thorough analysis of accurate, complete data serves as the
  foundation of your data story. Analyzing data using descriptive,
  diagnostic, predictive, and prescriptive analysis can enable you to
  understand its full picture.
- **Narrative:** A verbal or written narrative, also called a storyline,
  is used to communicate insights gleaned from data, the context
  surrounding it, and actions you recommend and aim to inspire in your
  audience.
- **Visualizations:** Visual representations of your data and narrative
  can be useful for communicating its story clearly and memorably. These
  can be charts, graphs, diagrams, pictures, or videos.

[This article by a company called
Toughspot](https://www.thoughtspot.com/data-trends/best-practices/data-storytelling)
provides a series of steps to follow to create a data story:

- Find the story within the data
- Consider your audience
- Determine what data matters
- Analyze the data and find insights
- Identify the most effective data visualizations
- Provide context
- Structure your story
- Edit until the story is clear and concise

<div>

> **Warning**
>
> A reminder that all work is personal work. You may discuss topics but
> you may not use code from other students and colleagues without
> attribution. Any code that you use from other sources like the
> internet must be cited with the appropriate hyperlink or other
> reference.

</div>

## The dataset

The dataset is described in the [paper contained in the `src-data/`
directory](src-data/paper.pdf). All of the files described in the paper
(the survey results and metadata for various countries and years.) Read
the paper.

## Story and visualization requirements

- The story should be between one and two pages long (500 to 1,000 words
  since it’s a single HTML page.)
- It is up to you to decide what data to use and what to focus on.
- Choose one or more genres described in [Segel and Heer’s Narrative
  Visualization: Telling Stories with Data
  paper.](http://vis.stanford.edu/files/2010-Narrative-InfoVis.pdf) for
  your story. **Note:** Some of the genres may be more difficult to
  implement for a proper experience. You may develop your own CSS
  templates to implement more complex stories, and that decision is up
  to you.
- The story must be *author-driven*, **not** *reader-driven*.
- There must be a minimum of three visualizations and a maximum of five
  and they must be connected to the story. MV Note: each should be a
  different view?
- Your visualizations must:
  - have a caption (using the chunk option `fig-cap`) describing the
    purpose of the visualization within the context of the story
  - be properly labeled, with axes labeled and units shown
  - have any necessary annotations to help the viewer understand
  - have a title
  - use the themes you’ve developed, or improvements to them that you
    have developed
- Separate your sections with a level 2 header (`## ...`).
- Make sure to spell and grammar check

## Submission and technical notes

- The final deliverable must be a rendered Quarto HTML document called
  named `my_submission.html` at the root level. The corresponding Quarto
  document must be called `my_submission.qmd`.
- You may use `R`, `Python`, or `Observable` at your discretion
- Use the `code/` directory for all your work (except the Quarto
  document.) Keep your code organized and commented. You may write a
  `README.md` file within the `code/` subdirectory to provide additional
  insight and context about your work.
- You do not need to do everything in the single Quarto file at the root
  level. You can work on the visualizations, data processing, etc. in
  individual `R` or `Python` scripts, or in other Quarto documents in
  the `code/` directory.
- When you render the Quarto file, you can include your other documents
  in the `code/` directory in one of two ways:
  - Including a script in a chunk by using a code chunk that looks like
    this:

    ```` markdown
    ```{r}
    #| echo: true
    #| eval: true 
    #| file: code/myscript.R
    ```
    ````

  - Including other Quarto documents (not scripts) by using the
    following notation: `{{< include code/name-of-qmd.qmd >}}`

## Rubric

| Component                | Excellent                                                                                                                                               | Satisfactory                                                                                                                         | Unsatisfactory                                                                                                |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Breadth of Exploration   | More than 3 questions were initially asked, and target substantially different portions/aspects of the data.                                            | At least 3 questions were initially asked of the data, but there is some overlap between questions.                                  | Fewer than 3 initial questions were posed of the data.                                                        |
| Depth of Exploration     | A sufficient number of follow-up questions were asked to yield insights that helped to more deeply explore the initial questions.                       | Some follow-up questions were asked, but they did not take the analysis much deeper than the initial questions.                      | No follow-up questions were asked after answering the initial questions.                                      |
| Data Quality             | Data quality was thoroughly assessed with extensive profiling of fields and records.                                                                    | Simple checks were conducted on only a handful of fields or records.                                                                 | Little or no evidence that data quality was assessed.                                                         |
| Visualizations           | More than 10 visualizations were produced, and a variety of marks and encodings were explored. All design decisions were both expressive and effective. | At least 10 visualizations were produced. The visual encodings chosen were largely effective and expressive, but some errors remain. | Several ineffective or inexpressive design choices are made. Fewer than 10 visualizations have been produced. |
| Data Transformation      | More advanced transformation were used to extend the dataset in interesting or useful ways.                                                             | Simple transforms (e.g., sorting, filtering) were primarily used.                                                                    | The raw dataset was used directly, with little to no additional transformation.                               |
| Captions                 | Captions richly describe the visualizations and contextualize the insight within the story.                                                             | Captions do a good job describing the visualizations, but could be better connected to the story.                                    | Captions are missing, overly brief, or shallow.                                                               |
| Writing                  | Writing is xxxxx. S                                                                                                                                     | Writing is xxxxxxx                                                                                                                   | Writing is xxxxx.                                                                                             |
| Story                    | The story is engaging and understandable. The audience learns something new.                                                                            | The story is good.                                                                                                                   | The story has no logical beginning or end.                                                                    |
| Creativity & Originality | You exceeded the parameters of the assignment, with original insights or a particularly engaging design.                                                | You met all the parameters of the assignment.                                                                                        | You met most of the parameters of the assignment.                                                             |
