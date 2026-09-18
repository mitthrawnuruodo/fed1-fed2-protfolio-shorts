# What You Have to Show, and How Junior Interviews Actually Work

This article is for your own benefit - there's nothing to submit. It doesn't overlap with your Course Assignment requirements; check the Course Assignment Brief for what the CA submission itself must contain.

## 1. What you're actually walking away with

It is easy, especially near the end of a fast-paced course, to look at your CV next to a bachelor graduate's and feel like you are bringing nothing to the table. That is not accurate, and it is worth being precise about why.

**The qualification itself is real.** A fagskolegrad from an accredited fagskole (120 studiepoeng) is a protected title, sitting at level 5.2 in the Norwegian national qualifications framework. It is formal, documented education, not a course certificate. When you write applications, say so plainly rather than downplaying it.

**Job ads describe a wish list, not always a hard requirement.** A line like "bachelor's degree or equivalent experience" is frequently written by HR as a filter, not by the hiring manager as an absolute bar. That said, be realistic: some employers, particularly larger consultancies and parts of the public sector where pay grades are tied to formal education, genuinely do screen on degrees and will not look past it. Others, including a lot of the smaller product companies and agencies where juniors actually get hired, look at what you can build first and ask about paper credentials later. Frontend is a field where that second group is unusually large.

**Here is the reframe that matters most:** a bachelor graduate applying for their first developer job is also a junior with no professional experience. The degree does not remove that. What actually separates candidates at that stage is what they can show - deployed projects, code someone else can read, and the ability to talk through decisions in an interview. Both of you are building that same leg to stand on. You are not behind by default, you are just building it through a different path.

### Worked example: two ways of writing the same thing

**Generic (says nothing):**
> "Frontend developer with knowledge of HTML, CSS and JavaScript, looking for a junior role."

**Specific (shows the leg to stand on):**
> "Fagskole-educated frontend developer (120 studiepoeng, NKR level 5.2). Built and deployed three portfolio projects using React and vanilla JavaScript, including [specific project], where I [specific improvement or problem solved]. Comfortable working across HTML, CSS, JavaScript/TypeScript and version control in a team setting."

The second version does three things the first doesn't: names the qualification correctly, points at concrete evidence, and gives the reader something they could ask a follow-up question about. Use that as the template when you write your own LinkedIn summary or CV profile section - swap in your own projects and results.

### One more thing worth naming: AI and the junior job market

You will have heard some version of "AI is taking junior developer jobs." It is worth naming plainly rather than ignoring. Entry-level tech hiring has genuinely tightened over the past few years, and part of that is real: AI tools now handle a lot of the small, repetitive tasks (simple CRUD endpoints, boilerplate, basic bug fixes) that used to be a junior's bread and butter early on.

Two things worth knowing before you take that as a verdict on your prospects. First, the specific numbers you will see quoted online vary wildly and are often unreliable - a lot of that content is written to alarm rather than inform. Second, this is genuinely disputed even among people running large tech companies - some have argued publicly that writing off junior hiring is short-sighted, since it breaks the pipeline that produces senior developers later.

What is consistent across most credible accounts is this: the bar has moved from "can you write working code" toward "can you explain your reasoning, use AI tools without being dependent on them, and show judgement about what you built." That is exactly the same thing this section already told you to focus on - it just means it matters more now, not less.

### A brief word on soft skills

Alongside "can you code," most junior hiring conversations quietly test for a shorter list of things that have nothing to do with syntax:

- **Communication** - can you explain a technical decision to someone who wasn't there for it, without over-explaining or under-explaining.
- **Receiving feedback** - can you take a code review comment or a correction without getting defensive, and actually use it.
- **Working with others when things go sideways** - the group-work friction from lesson 1.1 is directly relevant here: most teams hit disagreement, uneven contribution, or communication breakdowns at some point, and how you handled it is a legitimate, useful thing to talk about in an interview rather than something to hide.
- **Asking for help at the right time** - not too early (before you've tried), not too late (after an hour of silently stuck).

None of this is abstract "soft skills training." It is the same behavioural-question material from section 2, just named explicitly here so you know it's being evaluated, not just the code you write.

## 2. How junior developer interviews actually work

The peer mock interview you are doing for your Course Assignment is a good exercise, but it only simulates one format: someone asking you prepared questions face to face. Real junior interviews usually involve a mix of the following, and it helps to know what each one is actually testing.

**Live coding or pairing.** You are given a small problem and asked to solve it while the interviewer watches, sometimes with them asking questions as you go. The point is almost never "did you produce the perfect answer." It is whether you can think out loud, ask clarifying questions before diving in, and recover calmly when you get stuck, rather than going quiet.

**Take-home tasks.** A small piece of work you complete on your own time and then discuss afterwards. A reasonable one is scoped, time-boxed (a few hours, clearly stated), and paid or at minimum clearly described as an assessment exercise. Be cautious of anything open-ended, unpaid, and effectively asking for free production work - that is a fair thing to push back on or decline.

**Structure or "how would you build this" questions.** For juniors, this is rarely a full system-design question. It is more often "how would you structure the components on this page" or "how would you organise the state here." They want to hear your reasoning, not a textbook answer.

**Behavioural questions.** Usually framed as "tell me about a time when...". The STAR structure (Situation, Task, Action, Result) is the simplest way to answer these without rambling: what was the situation, what were you responsible for, what did you actually do, what happened as a result. This is also the easiest way to turn group-project friction from your course into a genuinely good answer, instead of a complaint about a teammate.

### Worked example: an annotated live-coding exchange

Below is a short, fictional transcript of a candidate handling a live-coding question reasonably well. Notes in brackets point out what is working.

> **Interviewer:** Can you build a small component that shows a list of items, and lets the user filter them by typing in a search box?
>
> **Candidate:** Sure. Before I start, can I check - should this filter as they type, or only when they submit? And is there a data source already, or should I hardcode a small array for this? *[Clarifying questions before writing code - this is a strong opening, not a stalling tactic.]*
>
> **Interviewer:** Filter as they type, and yes, just hardcode a small array.
>
> **Candidate:** Okay, I'll set up a state variable for the search text, and derive the filtered list from it rather than storing a separate filtered array. That way I don't need to keep two things in sync. *[Explaining the approach before typing - lets the interviewer follow the reasoning, not just the code.]*
>
> *[A minute passes. The candidate's filter is case-sensitive and they notice.]*
>
> **Candidate:** Actually, hang on, this is case-sensitive right now, that's probably not what you'd want in a real search box. Let me lower-case both sides of the comparison. *[Caught and fixed their own mistake out loud instead of hoping no one noticed. This is a good sign to an interviewer, not a bad one.]*

None of this required the candidate to be flawless. What made it a good example was narrating the thinking, asking before assuming, and treating a mistake as something to fix rather than something to hide.

### Self-check before you'd be ready

You don't need a perfect score on this, but if most of these feel shaky, that's worth practising before an interview:

- I can explain what my last project does and why I made the main structural decisions, without looking at notes.
- I can name one thing I would do differently on a recent project, and why.
- I can talk through a bug I fixed and how I found it, not just that I fixed it.
- I'm comfortable saying "I'm not sure, let me think" out loud instead of going silent.
- I can describe one piece of group or course friction using Situation, Task, Action, Result, in under a minute.

## 3. Practising without needing a classmate

You do not need another developer to practise any of this. The questions below are for handing to literally anyone - a friend, a parent, a former colleague, someone from a Noroff alumni group - along with the short rubric underneath, so they can give you useful feedback without any development background.

**Questions to use:**
1. Tell me about a project you're proud of. What does it do, and what was your role in it?
2. Tell me about a time something didn't go to plan on a project or in a group. What happened, and what did you do?
3. What's something you'd do differently if you built that project again?
4. Talk me through how you'd explain what "responsive design" means to someone who isn't a developer.
5. Why are you interested in this kind of work?

**What your reviewer should listen for (no technical knowledge required):**
- Did they answer with a specific example, or stay vague and general?
- Could you follow the story - beginning, what they did, what happened?
- Did they sound like they understood their own answer, or like they were reciting something memorised?
- Would you want to ask a follow-up question? (If yes, that's usually a good sign - it means they said something concrete.)

Recording yourself answering these out loud and listening back afterwards works just as well if you would rather not involve anyone else at all.

## 4. A short note on your first offer

Here is advice that will not sound as exciting as "always negotiate," but is more honest for a first job: if the offer is fair and not exploitative, take it.

Most entry-level candidates do not negotiate their first offer at all, and for a junior role the base salary itself is often the least flexible part of what is on the table - there usually is not much room to move, and pushing hard on it can read oddly for a first job. That does not mean you have no options.

A reasonable approach:
- If something about the offer seems genuinely low or unfair compared to what similar junior roles pay, it is fine to ask about it once, calmly, at the offer stage - not during the interview itself.
- Otherwise, the more useful question is simply: "Is this something we can revisit once my probationary period (prøvetid) ends?" This signals that you expect to prove yourself, costs you nothing to ask, and sets a natural, low-pressure point to actually have the conversation later, once you have something concrete to point to.
- The same applies to non-salary things worth asking about: start date, remote or hybrid days, equipment.

This will not feel as assertive as some of the "negotiate everything" advice you will find online. That advice is mostly written for candidates with leverage - multiple offers, in-demand specialised skills, or a few years of experience already. As a first-time junior candidate, you generally do not have that leverage yet, and pretending otherwise can work against you. You will have it on your second job.
