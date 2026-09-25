# Your Footprint Beyond the Portfolio Site, and What a Reviewer Actually Looks At

This article is for your own benefit - there's nothing to submit. It doesn't add to or change your Course Assignment requirements; check the Course Assignment Brief for what the CA submission itself must contain.

## 1. The reviewer's first two minutes

Lesson 1.1 lists what a good portfolio should contain. That's useful, but it's written from your side of the table. It's worth flipping it around once and asking: what does the person on the other side actually do?

Here is a short, fictional, but fairly typical example. Ingrid is a frontend lead at a small agency. She has fifteen applications for a junior position and one afternoon to go through them. This is roughly what happens with one of them.

> **0:00** - She opens the portfolio link from the application. The page loads, looks tidy, and she can see straight away what this person does. *[No verdict yet, but no reason to leave either.]*
>
> **0:20** - She skips the introduction and clicks the project that looks most interesting: a small tide-table app. *[She picks one project, not all of them. Whichever one she picks has to hold up on its own.]*
>
> **0:40** - The live demo works. She types in a place name, gets a result, resizes the window a bit. *[This is the "does it actually work" check. It takes seconds, and a broken link here often ends the visit.]*
>
> **1:05** - She clicks through to the GitHub repository. The README tells her what the app does and what it's built with, and there's a screenshot. *[She's checking that the code matches the story the portfolio told.]*
>
> **1:25** - She opens one JavaScript file at random and scrolls. Sensible names, some structure, nothing alarming. Then she glances at the commit list. *[She's not reviewing the code properly. She's looking for signs of care.]*
>
> **1:50** - She clicks the candidate's username to see what else is on their GitHub account. *[This is the part most students never think about - see section 2.]*
>
> **2:00** - She puts the application in the "talk to" pile.

Two things are worth noticing here.

**Nobody reads everything.** Reviewers sample. They pick one project, one file, one screen. You can't control which one they pick, so the practical goal is that there's nothing embarrassing anywhere they might click.

**A weak point rarely sinks you, but a broken one often does.** Slightly awkward CSS on one project is normal for a junior. A dead demo link, an empty README, or a repository that won't load tends to end the visit, because the reviewer has fourteen other applications waiting.

## 2. Your GitHub account is part of your portfolio

At 1:50, Ingrid left your portfolio and went to your GitHub account. From that moment, your carefully built portfolio site is no longer in charge of the story - your repository list is.

For most students after a year of study, that list looks something like this:

**Before:**

```
test
lesson-task-3
project-final
project-final-v2-NEW
css-course-assignment
js1-ca
untitled
tide-table-app
```

Nothing here is wrong, exactly. But a reviewer can't tell which of these matter, and "project-final-v2-NEW" invites questions you'd rather not answer.

A few small changes make a big difference:

- **Pin your best work.** GitHub lets you pin up to six repositories to the top of your profile. Pinned repositories are the first thing a visitor sees, so choose them on purpose.
- **Name repositories after what they are.** `tide-table-app` says something. `project-final` says nothing. You can rename a repository in its settings, and GitHub redirects the old URL.
- **Fill in the "About" box.** On every repository page there's a small "About" section (the gear icon on the right). Add a one-line description, the live website link, and a few topics (for example `javascript`, `css`, `accessibility`). It takes a minute per repository and makes your list readable at a glance.
- **Tidy away practice work.** Old lesson tasks and experiments don't need to be deleted, but they don't need to be public either. You can make a repository private, or archive it (Settings, then "Archive this repository"), which marks it clearly as read-only and finished.

**After:**

```
Pinned:
  tide-table-app        Search tide times for Norwegian harbours. Vanilla JS, fetch.
  rainy-days-shop       Responsive e-commerce front end for an outdoor clothing brand.
  quiz-game             Accessible browser quiz with keyboard support.

Other public repositories:
  css-grid-experiments  Small layout experiments while learning CSS Grid.
```

Same person, same work - but now the reviewer knows where to look.

## 3. The contribution graph: what it does and doesn't say

The grid of green squares on your GitHub profile gets a lot of attention online, and a fair amount of myth.

**What it shows:** days on which you made contributions, such as commits to a repository's default branch, opening issues or pull requests. Contributions to private repositories only appear if you've turned that on in your profile settings, and even then without any details.

**What it doesn't show:** how good any of that work was. A wall of dark green made of commits called "update" is not more impressive than a lighter graph with a few meaningful ones, and experienced reviewers know this.

**A common student problem:** commits only count towards your graph if the email address in your Git configuration is linked to your GitHub account. If you've committed from a work laptop, a school computer or a fresh setup with a different email, those commits may be missing from your graph entirely. You can check which email you're committing with by running:

```
git config user.email
```

If it isn't one of the addresses listed in your GitHub email settings, add it there, or change your Git configuration.

**Commit messages are part of the same picture.** When Ingrid glanced at the commit list at 1:25, she was reading your messages, not your code. Compare:

```
fix
update
more changes
final fix
```

with:

```
Add search by harbour name
Handle empty results with a friendly message
Fix layout overflow on narrow screens
Improve contrast on result cards
```

The second list tells a small story about how the project grew. It takes no extra time to write, only a habit.

## 4. Search for yourself

One last check, and the easiest one to forget: search for your own name, the way a reviewer might, in a private browser window.

What comes up? Is it your portfolio and GitHub, or an old gaming profile and a forum post from years ago? You can't control everything the internet has on you, but you can make sure the things you *do* control are easy to find and tell the same story:

- Use the same name, or recognisably the same handle, across your portfolio, GitHub and any other professional profiles.
- Make sure each place links to the others, so a reviewer who finds one can find the rest.
- If your GitHub username is something you chose at fifteen, consider whether it's worth changing now, before you start applying for jobs. Changing it later is possible, but old links to your profile will break.

### LinkedIn: claim your spot now

If you don't have a LinkedIn profile yet, the end of Year 1 is a good time to create one, even if you're not job-hunting yet. A plain profile that exists and is accurate is worth more than a perfect one you never get round to making. For now, three things are enough:

- **Use the same name** as on your portfolio and GitHub, so a reviewer can tell it's the same person.
- **Set a custom profile URL.** By default LinkedIn gives you an address ending in a string of numbers. You can change it in your public profile settings to something like `linkedin.com/in/your-name`, which looks better on a CV and is easier to type.
- **Link to your portfolio and GitHub** from the contact information section, so the three places point to each other.

Making LinkedIn actually work for you - a proper headline, an About section, featuring your work and building connections - is a bigger topic, and one you'll return to in Year 2.

## Self-check

None of this is required. But if you want a quick sense of how your footprint looks from the outside, try these:

- If someone opened a random project of mine right now, would the live link work and would the repository explain itself?
- Can a stranger tell from my repository list which three or four projects I'm proudest of?
- Does every public repository have a description in its "About" box?
- Are my recent commits showing up on my contribution graph?
- Would I be comfortable with a reviewer reading my last ten commit messages?
- When I search for my name, do my professional profiles come up, and do they link to each other?
