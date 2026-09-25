# Write the README First, and Write It for Three Readers

This article is for your own benefit - there's nothing to submit. It doesn't replace the README templates used in your Course Assignment; check the Course Assignment Brief for what those READMEs must contain. This is about the thinking behind a good README, and a habit worth taking with you into future projects.

## 1. Your README has three readers

Lesson 1.2 describes what a README should contain. A useful way to decide *how* to write each part is to remember that three quite different people will read it, each looking for something different.

**The skimmer.** A recruiter, a hiring developer, a teacher. They will give your README around thirty seconds. They want to know what the project is, whether it works, and what it's built with. They will look at the first screenful and the screenshot, and very probably nothing else.

**The builder.** Another developer who wants to run your code, review it, or build on it. They'll skip your introduction and go straight to how to get it running and how it's organised. If that part is missing or wrong, they give up.

**Future you.** Six months from now you'll open this repository and have forgotten why the code is structured the way it is, what the known problems were, and how to start it. You are the reader most likely to actually need the README, and the one most often forgotten.

A good README serves all three, in that order: the skimmer's answers at the top, the builder's details in the middle, and notes for future you towards the end.

### Worked example: writing for nobody versus writing for three readers

Imagine a small plant-watering tracker: a vanilla JavaScript app where you register your house plants and it reminds you which ones need water.

**Written for nobody:**

```
# plant-app

This is my project. It is made with HTML, CSS and JavaScript.

## Installation
npm install
npm start
```

The skimmer doesn't learn what it does. The builder gets instructions that are simply wrong - this project has no `package.json`, so `npm install` does nothing useful. That section was copied from a template written for a different kind of project.

**Written for three readers:**

```
# Plant Watering Tracker

Keep track of which house plants need water today. Add a plant, set how
often it needs watering, and the app shows what's due.

![The plant list, with two plants marked as due today](docs/screenshot.png)

**Live demo:** [link]
**Built with:** HTML, CSS, vanilla JavaScript (ES modules), localStorage

## Running it locally

No build step or dependencies. Because the app uses ES modules, it needs
to be served over HTTP rather than opened directly as a file - for
example with the Live Server extension in VS Code.

## Project structure

- `js/storage.js` - reading and writing plants to localStorage
- `js/schedule.js` - works out which plants are due
- `js/render.js` - builds the plant list in the DOM

## Known limitations

- Data is stored per browser, so plants don't sync between devices.
- Dates are calculated in local time, which can be off by a day around
  midnight.
```

The skimmer gets their answers in the first few lines. The builder gets instructions that actually work, including the one detail that trips people up: module scripts are blocked by the browser when a page is opened straight from the file system. And future you gets a note of where things live and what was left unfinished.

Notice what is *not* there: no installation steps that don't apply, no empty "Contributing" section. A template is a checklist of things to consider, not a list of headings you must keep.

## 2. Try writing it first

Most people write the README last, once the project is finished and they're tired of it. There's an old idea, usually credited to GitHub co-founder Tom Preston-Werner in a short 2010 blog post called "Readme Driven Development", that turns this around: write the README *before* you write the code.

The point isn't documentation. It's planning. When you have to describe in plain language what your project does, who it's for and how someone uses it, you're forced to make decisions you'd otherwise put off until they become problems halfway through the build.

### Worked example: a README written before any code

Here's a first draft for a reading-list app, written before a single line of JavaScript:

```
# Reading List

A simple page for keeping track of books I want to read, am reading,
and have finished.

## What it does
- Add a book with a title and author.
- Move a book between "Want to read", "Reading" and "Finished".
- See how many books are in each list.

## Not in scope (yet)
- Searching for books online or fetching cover images.
- User accounts or syncing between devices.
- Ratings or reviews.
```

Writing this took ten minutes, and it already did three useful jobs:

- **It set the scope.** "Fetching cover images" sounded fun, but writing it down made it obvious that it would double the size of the project. Moving it to "Not in scope (yet)" was a decision, not something forgotten.
- **It shaped the code.** Three lists with books moving between them suggests one array of books, each with a `status` property, rather than three separate arrays. That's a structural choice made before any code existed.
- **It gave a definition of done.** When all three items under "What it does" work, the first version is finished. That makes it much easier to actually finish.

Once the project is built, you update the README to match reality, add a screenshot and the live link, and most of the writing is already done.

This works especially well for your own side projects, where there is no brief telling you what to build and it's easy to keep adding features forever.

## 3. A few Markdown features worth knowing

GitHub renders README files using GitHub Flavored Markdown, which supports a few things beyond headings and lists that make a README easier to read.

**Relative image paths, with real alt text.** Keep screenshots in the repository (for example in a `docs` or `images` folder) and link to them relatively. Write alt text that describes what the image shows, just as you would on a web page:

```
![Search results showing high and low tide times for Bergen](docs/results.png)
```

**Collapsible sections.** For long content most readers can skip, such as a detailed changelog or setup notes for an unusual environment, you can use HTML's `details` element:

```
<details>
<summary>Notes on testing in older browsers</summary>

Content here only shows when the reader clicks the summary.

</details>
```

The empty lines around the content matter - without them, the Markdown inside won't be rendered.

**Alerts.** GitHub supports highlighted callout boxes for things the reader really shouldn't miss:

```
> [!NOTE]
> The live demo uses sample data and resets every night.

> [!WARNING]
> Clearing your browser data will delete all saved plants.
```

The available types are `NOTE`, `TIP`, `IMPORTANT`, `WARNING` and `CAUTION`. Use them sparingly - if everything is highlighted, nothing is.

**Heading structure.** GitHub builds an outline of your README from its headings, available from the list icon at the top of the file view. A sensible hierarchy (one `#` title, then `##` sections, then `###` subsections, without skipping levels) makes that outline useful, and follows the same rule you'd follow for headings on an accessible web page.

## Try this

Nothing here is required, but if you'd like to try the ideas out:

- Pick one of your existing projects and read its README three times, once as each reader. What is each of them missing?
- Check the setup instructions in one of your READMEs actually work, by following them exactly on a fresh clone of the repository.
- Next time you start a side project, spend ten minutes writing a README with "What it does" and "Not in scope (yet)" before you open your code editor, and see whether it changes what you build.
