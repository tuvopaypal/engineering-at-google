# Software Engineering at Google

## Part 1. Thesis

### Chapter 1. What is Software Engineering

Within Google, we sometimes say, “Software engineering is programming integrated over time.”

One way to see the impact of time on a program is to think about the question, “What is the expected life span1 of your code?”

We’ve found that expertise and shared communication forums offer great value as an organization scales. As engineers discuss and answer questions in shared forums, knowledge tends to spread. New experts grow. If you have a hundred engineers writing Java, a single friendly and helpful Java expert willing to answer questions will soon produce a hundred engineers writing better Java code. Knowledge is viral, experts are carriers, and there’s a lot to be said for the value of clearing away the common stumbling blocks for your engineers.

In many organizations, whiteboard markers are treated as precious goods. They are tightly controlled and always in short supply. Invariably, half of the markers at any given whiteboard are dry and unusable. How often have you been in a meeting that was disrupted by lack of a working marker? How often have you had your train of thought derailed by a marker running out? How often have all the markers just gone missing, presumably because some other team ran out of markers and had to abscond with yours? All for a product that costs less than a dollar.

Google tends to have unlocked closets full of office supplies, including whiteboard markers, in most work areas. With a moment’s notice it is easy to grab dozens of markers in a variety of colors. Somewhere along the line we made an explicit trade-off: it is far more important to optimize for obstacle-free brainstorming than to protect against someone wandering off with a bunch of markers.

#### TL;DRs

-   “Software engineering” differs from “programming” in dimensionality: programming is about producing code. Software engineering extends that to include the maintenance of that code for its useful life span.
-   There is a factor of at least 100,000 times between the life spans of short-lived code and long-lived code. It is silly to assume that the same best practices apply universally on both ends of that spectrum.
-   Software is sustainable when, for the expected life span of the code, we are capable of responding to changes in dependencies, technology, or product requirements. We may choose to not change things, but we need to be capable.
-   Hyrum’s Law: with a sufficient number of users of an API, it does not matter what you promise in the contract: all observable behaviors of your system will be depended on by somebody.
-   Every task your organization has to do repeatedly should be scalable (linear or better) in terms of human input. Policies are a wonderful tool for making process scalable.
-   Process inefficiencies and other software-development tasks tend to scale up slowly. Be careful about boiled-frog problems.
-   Expertise pays off particularly well when combined with economies of scale.
-   “Because I said so” is a terrible reason to do things.
-   Being data driven is a good start, but in reality, most decisions are based on a mix of data, assumption, precedent, and argument. It’s best when objective data makes up the majority of those inputs, but it can rarely be all of them.
-   Being data driven over time implies the need to change directions when the data changes (or when assumptions are dispelled). Mistakes or revised plans are inevitable.

## Part II. Culture

### Chapter 2. How to Work Well on Teams

The vast majority of the work at Google (and at most companies!) doesn’t require genius-level intellect, but 100% of the work requires a minimal level of social skills. What will make or break your career, especially at a company like Google, is how well you collaborate with others.

Another common motivation for hiding your work is the fear that another programmer might take your idea and run with it before you get around to working on it. By keeping it secret, you control the idea.

If you spend all of your time working alone, you’re increasing the risk of unnecessary failure and cheating your potential for growth. Even though software development is deeply intellectual work that can require deep concentration and alone time, you must play that off against the value (and need!) for collaboration and review.

The chances of an early misstep are high. The more feedback you solicit early on, the more you lower this risk.3 Remember the tried-and-true mantra of “Fail early, fail fast, fail often.”

Bus factor (noun): the number of people that need to get hit by a bus before your project is completely doomed.

If you’re the only person who understands how the prototype code works, you might enjoy good job security—but if you get hit by a bus, the project is toast. If you’re working with a colleague, however, you’ve doubled the bus factor.

Hopefully most engineers recognize that it is better to be one part of a successful project than the critical part of a failed project.

Programmers work best in tight feedback loops: write a new function, compile. Add a test, compile. Refactor some code, compile. This way, we discover and fix typos and bugs as soon as possible after generating code.

We think the middle ground is really the best solution. Group teams of four to eight people together in small rooms (or large offices) to make it easy (and non-embarrassing) for spontaneous conversation to happen.

In many companies, the very act of wearing headphones is a common signal that means “don’t disturb me unless it’s really important.”

The Three Pillars of Social Interaction

Pillar 1: Humility
You are not the center of the universe (nor is your code!). You’re neither omniscient nor infallible. You’re open to self-improvement.

Pillar 2: Respect
You genuinely care about others you work with. You treat them kindly and appreciate their abilities and accomplishments.

Pillar 3: Trust
You believe others are competent and will do the right thing, and you’re OK with letting them drive when appropriate.

The moral is this: do not underestimate the power of playing the social game. It’s not about tricking or manipulating people; it’s about creating relationships to get things done. Relationships always outlast projects. When you’ve got richer relationships with your coworkers, they’ll be more willing to go the extra mile when you need them.

Even if you know you’re the wisest person in the discussion, don’t wave it in people’s faces. For example, do you always feel like you need to have the first or last word on every subject? Do you feel the need to comment on every detail in a proposal or discussion? Or do you know somebody who does these things?

In a professional software engineering environment, criticism is almost never personal—it’s usually just part of the process of making a better project. The trick is to make sure you (and those around you) understand the difference between a constructive criticism of someone’s creative output and a flat-out assault against someone’s character.

At Google, one of our favorite mottos is that “Failure is an option.” It’s widely recognized that if you’re not failing now and then, you’re not being innovative enough or taking enough risks. Failure is viewed as a golden opportunity to learn and improve for the next go-around.

A good postmortem should include the following:

-   A brief summary of the event
-   A timeline of the event, from discovery through investigation to resolution
-   The primary cause of the event
-   Impact and damage assessment
-   A set of action items (with owners) to fix the problem immediately
-   A set of action items to prevent the event from happening again
-   Lessons learned

Admitting that you’ve made a mistake or you’re simply out of your league can increase your status over the long run. In fact, the willingness to express vulnerability is an outward show of humility, it demonstrates accountability and the willingness to take responsibility, and it’s a signal that you trust others’ opinions. In return, people end up respecting your honesty and strength. Sometimes, the best thing you can do is just say, “I don’t know.”

When you’re writing software, however, you don’t need to be continually on the defensive—your teammates are collaborators, not competitors. You all have the same goal.

“Googleyness”—a set of attributes and behaviors that we look for that represent strong leadership and exemplify “humility, respect, and trust”:

-   Thrives in ambiguity: Can deal with conflicting messages or directions, build consensus, and make progress against a problem, even when the environment is constantly shifting.
-   Values feedback: Has humility to both receive and give feedback gracefully and understands how valuable feedback is for personal (and team) development.
-   Challenges status quo: Is able to set ambitious goals and pursue them even when there might be resistance or inertia from others.
-   Puts the user first: Has empathy and respect for users of Google’s products and pursues actions that are in their best interests.
-   Cares about the team: Has empathy and respect for coworkers and actively works to help them without being asked, improving team cohesion.
-   Does the right thing: Has a strong sense of ethics about everything they do; willing to make difficult or inconvenient decisions to protect the integrity of the team and product.

#### TL;DRs

-   Be aware of the trade-offs of working in isolation.
-   Acknowledge the amount of time that you and your team spend communicating and in interpersonal conflict. A small investment in understanding personalities and working styles of yourself and others can go a long way toward improving productivity.
-   If you want to work effectively with a team or a large organization, be aware of your preferred working style and that of others.

### Chapter 3. Knowledge Sharing

Information islands - Knowledge fragmentation that occurs in different parts of an organization that don’t communicate with one another or use shared resources. In such an environment, each group develops its own way of doing things.1 This often leads to the following:

-   Information fragmentation - Each island has an incomplete picture of the bigger whole.
-   Information duplication - Each island has reinvented its own way of doing something.
-   Information skew - Each island has its own ways of doing the same thing, and these might or might not conflict.

Single point of failure (SPOF) - A bottleneck that occurs when critical information is available from only a single person. This is related to bus factor, which is discussed in more detail in Chapter 2.

SPOFs can arise out of good intentions: it can be easy to fall into a habit of “Let me take care of that for you.” But this approach optimizes for short-term efficiency (“It’s faster for me to do it”) at the cost of poor long-term scalability (the team never learns how to do whatever it is that needs to be done). This mindset also tends to lead to all-or-nothing expertise.

All-or-nothing expertise - A group of people that is split between people who know “everything” and novices, with little middle ground. This problem often reinforces itself if experts always do everything themselves and don’t take the time to develop new experts through mentoring or documentation. In this scenario, knowledge and responsibilities continue to accumulate on those who already have expertise, and new team members or novices are left to fend for themselves and ramp up more slowly.

Parroting - Mimicry without understanding. This is typically characterized by mindlessly copying patterns or code without understanding their purpose, often under the assumption that said code is needed for unknown reasons.

Haunted graveyards - Places, often in code, that people avoid touching or changing because they are afraid that something might go wrong. Unlike the aforementioned parroting, haunted graveyards are characterized by people avoiding action because of fear and superstition.

Every expert was once a novice: an organization’s success depends on growing and investing in its people.

Personalized, one-to-one advice from an expert is always invaluable. Different team members have different areas of expertise, and so the best teammate to ask for any given question will vary. But if the expert goes on vacation or switches teams, the team can be left in the lurch. And although one person might be able to provide personalized help for one-to-many, this doesn’t scale and is limited to small numbers of “many.”

Documented knowledge, on the other hand, can better scale not just to the team but to the entire organization. Mechanisms such as a team wiki enable many authors to share their expertise with a larger group. But even though written documentation is more scalable than one-to-one conversations, that scalability comes with some trade-offs: it might be more generalized and less applicable to individual learners’ situations, and it comes with the added maintenance cost required to keep information relevant and up to date over time.

Tribal knowledge exists in the gap between what individual team members know and what is documented.

A human expert can synthesize their expanse of knowledge. They can assess what information is applicable to the individual’s use case, determine whether the documentation is still relevant, and know where to find it. Or, if they don’t know where to find the answers, they might know who does.

We find the Recurse Center’s social rules to be helpful here:

-   No feigned surprise (“What?! I can’t believe you don’t know what the stack is!”)
    -   Feigned surprise is a barrier to psychological safety and makes members of the group afraid of admitting to a lack of knowledge.
-   No “well-actuallys”
    -   Pedantic corrections that tend to be about grandstanding rather than precision.
-   No back-seat driving
    -   Interrupting an existing discussion to offer opinions without committing to the conversation.
-   No subtle “-isms” (“It’s so easy my grandmother could do it!”)
    -   Small expressions of bias (racism, ageism, homophobia) that can make individuals feel unwelcome, disrespected, or unsafe.

It doesn’t matter whether you’re new to a team or a senior leader: you should always be in an environment in which there’s something to learn. If not, you stagnate (and should find a new environment).

In fact, the more you know, the more you know you don’t know.

YAQS (“Yet Another Question System”) is a Google-internal version of a Stack Overflow–like website, making it easy for Googlers to link to existing or work-in-progress code as well as discuss confidential information.

Sometimes it’s really important to have a human to talk to, and in those instances, office hours can be a good solution.

This is particularly useful if the problem is still ambiguous enough that the engineer doesn’t yet know what questions to ask (such as when they’re just starting to design a new service) or whether the problem is about something so specialized that there just isn’t documentation on it.

The bad behavior of just a few individuals can make an entire team or community unwelcoming.

Knowledge sharing can and should be done with kindness and respect. In tech, tolerance—or worse, reverence—of the “brilliant jerk” is both pervasive and harmful, but being an expert and being kind are not mutually exclusive.

Leaders improve the quality of the people around them, improve the team’s psychological safety, create a culture of teamwork and collaboration, defuse tensions within the team, set an example of Google’s culture and values, and make Google a more vibrant and exciting place to work. Jerks are not good leaders.

Similar to peer bonuses are kudos: public acknowledgement of contributions (typically smaller in impact or effort than those meriting a peer bonus) that boost the visibility of peer-to-peer contributions.

A system in which people can formally and easily recognize their peers is a powerful tool for encouraging peers to keep doing the awesome things they do. It’s not the bonus that matters: it’s the peer acknowledgement.

go/ links

Setting up static analysis tools requires an upfront investment, but as soon as they are in place, they scale efficiently.

Around 1 to 2% of Google engineers are readability reviewers. All reviewers are volunteers, and anyone with readability is welcome to self-nominate to become a readability reviewer. Readability reviewers are held to the highest standards because they are expected not just to have deep language expertise, but also an aptitude for teaching through code review.

#### TL;DRs

-   Psychological safety is the foundation for fostering a knowledge-sharing environment.
-   Start small: ask questions and write things down.
-   Make it easy for people to get the help they need from both human experts and documented references.
-   At a systemic level, encourage and reward those who take time to teach and broaden their expertise beyond just themselves, their team, or their organization.
-   There is no silver bullet: empowering a knowledge-sharing culture requires a combination of multiple strategies, and the exact mix that works best for your organization will likely change over time.

### Chapter 4. Engineering for Equity

Bias Is the Default

All people have certain biases, and social scientists have recognized over the past several decades that most people exhibit unconscious bias, enforcing and promulgating existing stereotypes. Unconscious bias is insidious and often more difficult to mitigate than intentional acts of exclusion. Even when we want to do the right thing, we might not recognize our own biases.

The lack of representation of such users in our workforce1 means that we often do not have the requisite diversity to understand how the use of our products can affect underrepresented or vulnerable users.

One way to address these problems is to help the software engineering organization itself look like the populations for whom we build products.

Engineers should focus on people who are different than themselves, especially people who might attempt to use their products to cause harm. The most difficult users to consider are those who are disenfranchised by the processes and the environment in which they access technology. To address this challenge, engineering teams need to be representative of their existing and future users. In the absence of diverse representation on engineering teams, individual engineers need to learn how to build for all users.

If you are an engineering manager who wants to hire more women, don’t just focus on building a pipeline. Focus on other aspects of the hiring, retention, and progression ecosystem and how inclusive it might or might not be to women. Consider whether your recruiters are demonstrating the ability to identify strong candidates who are women as well as men.

Design for the user who will have the most difficulty using your product. Building for those with additional challenges will make the product better for everyone. Another way of thinking about this is: don’t trade equity for short-term velocity.

#### TL;DRs

-   Diversity is necessary to design properly for a comprehensive user base.
-   Inclusivity is critical not just to improving the hiring pipeline for underrepresented groups, but to providing a truly supportive work environment for all people.
-   Product velocity must be evaluated against providing a product that is truly useful to all users. It’s better to slow down than to release a product that might cause harm to some users.

### Chapter 5. How to Lead a Team

A Manager is a leader of people, whereas a Tech Lead leads technology efforts. Although the responsibilities of these two roles require similar planning skills, they require quite different people skills.

A boat without a captain is nothing more than a floating waiting room: unless someone grabs the rudder and starts the engine, it’s just going to drift along aimlessly with the current. A piece of software is just like that boat: if no one pilots it, you’re left with a group of engineers burning up valuable time, just sitting around waiting for something to happen (or worse, still writing code that you don’t need).

Google decided early on, however, that its software engineering managers should have an engineering background. This meant hiring experienced managers who used to be software engineers, or training software engineers to be managers (more on this later).

At the highest level, an engineering manager is responsible for the performance, productivity, and happiness of every person on their team—including their tech lead—while still making sure that the needs of the business are met by the product for which they are responsible. Because the needs of the business and the needs of individual team members don’t always align, this can often place a manager in a difficult position.

Most TLs are also individual contributors, which often forces them to choose between doing something quickly themselves or delegating it to a team member to do (sometimes) more slowly. The latter is most often the correct decision for the TL as they grow the size and capability of their team.

If you’ve spent the majority of your career writing code, you typically end a day with something you can point to—whether it’s code, a design document, or a pile of bugs you just closed—and say, “That’s what I did today.” But at the end of a busy day of “management,” you’ll usually find yourself thinking, “I didn’t do a damned thing today.”

Quantifying management work is more difficult than counting widgets you turned out, but just making it possible for your team to be happy and productive is a big measure of your job.

Another big reason for not becoming a manager is often unspoken but rooted in the famous “Peter Principle,” which states that “In a hierarchy every employee tends to rise to his level of incompetence.” Google generally avoids this by requiring that a person perform the job above their current level for a period of time (i.e., to “exceeds expectations” at their current level) before being promoted to that level.

“Above all, resist the urge to manage.” One of the greatest urges of the newly minted manager is to actively “manage” their employees because that’s what a manager does, right? This typically has disastrous consequences.

The cure for the “management” disease is a liberal application of “servant leadership,” which is a nice way of saying the most important thing you can do as a leader is to serve your team, much like a butler or majordomo tends to the health and well-being of a household. As a servant leader, you should strive to create an atmosphere of humility, respect, and trust.

Traditional managers worry about how to get things done, whereas great managers worry about what things get done (and trust their team to figure out how to do it).

A common saying at Google is that if you try to achieve an impossible goal, there’s a good chance you’ll fail, but if you fail trying to achieve the impossible, you’ll most likely accomplish far more than you would have accomplished had you merely attempted something you knew you could complete.

Failing fast is good because there’s not a lot at stake.

Every time there is a major production failure at Google, we perform a postmortem. This procedure is a way to document the events that led to the actual failure and to develop a series of steps that will prevent it from happening in the future.

Antipattern: Hire Pushovers

If you build a team of pushovers, you probably can’t take a vacation; the moment you leave the room, productivity comes to a screeching halt.

Instead, you should strive to hire people who are smarter than you and can replace you. This can be difficult because these very same people will challenge you on a regular basis (in addition to letting you know when you make a mistake). These very same people will also consistently impress you and make great things happen.

Antipattern: Ignore Low Performers

“Sometimes you get to be the tooth fairy, other times you have to be the dentist.”

We’ve seen team leaders do all the right things to build incredibly strong teams only to have these teams fail to excel (and eventually fall apart) because of just one or two low performers.

Sometimes, people miss expectations because they’re not working long enough or hard enough, but the most difficult cases are when someone just isn’t capable of doing their job no matter how long or hard they work.

Google’s Site Reliability Engineering (SRE) team has a motto: “Hope is not a strategy.” And nowhere is hope more overused as a strategy than in dealing with a low performer. Most team leaders grit their teeth, avert their eyes, and just hope that the low performer either magically improves or just goes away. Yet it is extremely rare that this person does either.

You can be sure that the team knows the low performer is there even if you’re ignoring them—in fact, the team is acutely aware of who the low performers are, because they have to carry them.

Ignoring low performers is not only a way to keep new high performers from joining your team, but it’s also a way to encourage existing high performers to leave. You eventually wind up with an entire team of low performers because they’re the only ones who can’t leave of their own volition.

How do you effectively coach a low performer? The best analogy is to imagine that you’re helping a limping person learn to walk again, then jog, then run alongside the rest of the team. It almost always requires temporary micromanagement, but still a whole lot of humility, respect, and trust—particularly respect. Set up a specific time frame (say, two months) and some very specific goals you expect them to achieve in that period. Make the goals small, incremental, and measurable so that there’s an opportunity for lots of small successes. Meet with the team member every week to check on progress, and be sure you set really explicit expectations around each upcoming milestone so that it’s easy to measure success or failure. If the low performer can’t keep up, it will become quite obvious to both of you early in the process. At this point, the person will often acknowledge that things aren’t going well and decide to quit; in other cases, determination will kick in and they’ll “up their game” to meet expectations.

Antipattern: Ignore Human Issues

Antipattern: Be Everyone’s Friend

Antipattern: Compromise the Hiring Bar

Steve Jobs once said: “A people hire other A people; B people hire C people.”

The cost of finding the appropriate person—whether by paying recruiters, paying for advertising, or pounding the pavement for references—pales in comparison to the cost of dealing with an employee who you never should have hired in the first place. This “cost” manifests itself in lost team productivity, team stress, time spent managing the employee up or out, and the paperwork and stress involved in firing the employee.

Antipattern: Treat Your Team Like Children

The IT department runs numerous “Tech Stops” that provide self-service areas that are like a mini electronics store. These contain lots of computer accessories and doodads (power supplies, cables, mice, USB drives, etc.) that would be easy to just grab and walk off with en masse, but because Google employees are being trusted to check these items out, they feel a responsibility to Do The Right Thing. Many people from typical corporations react in horror to hearing this, exclaiming that surely Google is hemorrhaging money due to people “stealing” these items. That’s certainly possible, but what about the costs of having a workforce that behaves like children or that has to waste valuable time formally requesting cheap office supplies? Surely that’s more expensive than the price of a few pens and USB cables.

The last part of losing the ego is a simple one, but many engineers would rather be boiled in oil than do it: apologize when you make a mistake.

Apologizing doesn’t cost money. People have enormous respect for leaders who apologize when they screw up, and contrary to popular belief, apologizing doesn’t make you vulnerable. In fact, you’ll usually gain respect from people when you apologize, because apologizing tells people that you are level headed, good at assessing situations, and—coming back to humility, respect, and trust—humble.

Another way of thinking about this is the maxim that the leader is always on stage. As a leader, your job is to inspire, but inspiration is a 24/7 job. Your visible attitude about absolutely everything—no matter how trivial—is unconsciously noticed and spreads infectiously to your team.

Some of us used to joke that if someone came in and told Bill that 19 of the company’s offices had been attacked by space aliens, Bill’s response would be, “Any idea why they didn’t make it an even 20?”

This brings us to another Zen management trick: asking questions. When a team member asks you for advice, it’s usually pretty exciting because you’re finally getting the chance to fix something. That’s exactly what you did for years before moving into a leadership position, so you usually go leaping into solution mode, but that is the last place you should be. The person asking for advice typically doesn’t want you to solve their problem, but rather to help them solve it, and the easiest way to do this is to ask this person questions.

Be a catalyst. One of the most common things a team leader does is to build consensus. This might mean that you drive the process from start to finish, or you just give it a gentle push in the right direction to speed it up.

Remove Roadblocks

You don’t need to know all the answers to help remove roadblocks, but it usually helps to know the people who do. In many cases, knowing the right person is more valuable than knowing the right answer.

One of the most difficult things to do as a TL is to watch a more junior team member spend 3 hours working on something that you know you can knock out in 20 minutes. Teaching people and giving them a chance to learn on their own can be incredibly difficult at first, but it’s a vital component of effective leadership.

One manager we know tells new team members, “I won’t lie to you, but I will tell you when I can’t tell you something or if I just don’t know.”

We strongly advise against using the compliment sandwich, not because we think you should be unnecessarily cruel or harsh, but because most people won’t hear the critical message, which is that something needs to change. It’s possible to employ respect here: be kind and empathetic when delivering constructive criticism without resorting to the compliment sandwich. In fact, kindness and empathy are critical if you want the recipient to hear the criticism and not immediately go on the defensive.

Every time a decision is made, it’s like a train coming through town—when you jump in front of the train to stop it, you slow the train down and potentially annoy the engineer driving the train. A new train comes by every 15 minutes, and if you jump in front of every train, not only do you spend a lot of your time stopping trains, but eventually one of the engineers driving the train is going to get mad enough to run right over you. So, although it’s OK to jump in front of some trains, pick and choose the ones you want to stop to make sure you’re stopping only the trains that really matter.

Track Happiness

The best leaders we’ve worked with have all been amateur psychologists, looking in on their team members’ welfare from time to time, making sure they get recognition for what they do, and trying to make certain they are happy with their work. One TLM we know makes a spreadsheet of all the grungy, thankless tasks that need to be done and makes certain these tasks are evenly spread across the team.

Our colleague Mekka starts his one-on-ones by asking his reports to rate their happiness on a scale of 1 to 10, and oftentimes his reports will use this as a way to discuss happiness in and outside of the office.

Unless you want to keep doing the exact same job for the rest of your career, seek to replace yourself.

Know when to make waves - You will (inevitably and frequently) have difficult situations crop up in which every cell in your body is screaming at you to do nothing about it.

Shield your team from chaos - When you step into a leadership role, the first thing you’ll usually discover is that outside your team is a world of chaos and uncertainty (or even insanity) that you never saw when you were an individual contributor. When I first became a manager back in the 1990s (before going back to being an individual contributor), I was taken aback by the sheer volume of uncertainty and organizational chaos that was happening in my company. I asked another manager what had caused this sudden rockiness in the otherwise calm company, and the other manager laughed hysterically at my naivete: the chaos had always been present, but my previous manager had shielded me and the rest of my team from it.

It’s easy to say “yes” to something that’s easy to undo. Really good leaders have a good sense for when something can be undone, but more things are undoable than you think (and this applies to both technical and nontechnical decisions).

You can increase intrinsic motivation by giving people three things: autonomy, mastery, and purpose.

Mastery in its basest form simply means that you need to give someone the opportunity to improve existing skills and learn new ones. Giving ample opportunities for mastery not only helps to motivate people, it also makes them better over time, which makes for stronger teams.13 An employee’s skills are like the blade of a knife: you can spend tens of thousands of dollars to find people with the sharpest skills for your team, but if you use that knife for years without sharpening it, you will wind up with a dull knife that is inefficient, and in some cases useless. Google gives ample opportunities for engineers to learn new things and master their craft so as to keep them sharp, efficient, and effective.

#### TL;DRs

-   Don’t “manage” in the traditional sense; focus on leadership, influence, and serving your team.
-   Delegate where possible; don’t DIY (Do It Yourself).
-   Pay particular attention to the focus, direction, and velocity of your team.

### Chapter 6. Leading at Scale

“The three Always of leadership”: Always Be Deciding, Always Be Leaving, Always Be Scaling.

#### Always Be Deciding

At this level, most of the decisions you’ll make are about finding the correct set of trade-offs.

At the highest level, your job as a leader—either of a single team or a larger organization—is to guide people toward solving difficult, ambiguous problems. By ambiguous, we mean that the problem has no obvious solution and might even be unsolvable. Either way, the problem needs to be explored, navigated, and (hopefully) wrestled into a state in which it’s under control. If writing code is analogous to chopping down trees, your job as a leader is to “see the forest through the trees” and find a workable path through that forest, directing engineers toward the important trees. There are three main steps to this process. First, you need to identify the blinders; next, you need to identify the trade-offs; and then you need to decide and iterate on a solution.

When you first approach a problem, you’ll often discover that a group of people has already been wrestling with it for years. These folks have been steeped in the problem for so long that they’re wearing “blinders”—that is, they’re no longer able to see the forest. They make a bunch of assumptions about the problem (or solution) without realizing it.

If you don’t frame your process as continuous rebalancing of trade-offs, your teams are likely to fall into the trap of searching for the perfect solution, which can then lead to what some call “analysis paralysis.” You need to make your teams comfortable with iteration. One way of doing this is to lower the stakes and calm nerves by explaining: “We’re going to try this decision and see how it goes. Next month, we can undo the change or make a different decision.” This keeps folks flexible and in a state of learning from their choices.

It’s not just your job to solve an ambiguous problem, but to get your organization to solve it by itself, without you present. If you can do that, it frees you up to move to a new problem (or new organization), leaving a trail of self-sufficient success in your wake.

Think about the last vacation you took that was at least a week long. Did you keep checking your work email? (Most leaders do.) Ask yourself why. Will things fall apart if you don’t pay attention? If so, you have very likely made yourself an SPOF. You need to fix that.

Being a successful leader means building an organization that is able to solve the difficult problem by itself. That organization needs to have a strong set of leaders, healthy engineering processes, and a positive, self-perpetuating culture that persists over time.

It’s also important to “manage up,” making sure your management chain understands what your group is doing and staying connected to the company at large. But often the most common and important answer to this question is: “I can see the forest through the trees.” In other words, you can define a high-level strategy. Your strategy needs to cover not just overall technical direction, but an organizational strategy as well. You’re building a blueprint for how the ambiguous problem is solved and how your organization can manage the problem over time. You’re continuously mapping out the forest, and then assigning the tree-cutting to others.

This is what good management is about: 95% observation and listening, and 5% making critical adjustments in just the right place.

Customers’ happiness requires just as much intense listening as your reports’ happiness.

#### TL;DRs

-   Always Be Deciding: Ambiguous problems have no magic answer; they’re all about finding the right trade-offs of the moment, and iterating.
-   Always Be Leaving: Your job, as a leader, is to build an organization that automatically solves a class of ambiguous problems—over time—without you needing to be present.
-   Always Be Scaling: Success generates more responsibility over time, and you must proactively manage the scaling of this work in order to protect your scarce resources of personal time, attention, and energy.

### Chapter 7. Measuring Engineering Productivity

At Google, we use the Goals/Signals/Metrics (GSM) framework to guide metrics creation.

-   A goal is a desired end result. It’s phrased in terms of what you want to understand at a high level and should not contain references to specific ways to measure it.
-   A signal is how you might know that you’ve achieved the end result. Signals are things we would like to measure, but they might not be measurable themselves.
-   A metric is proxy for a signal. It is the thing we actually can measure. It might not be the ideal measurement, but it is something that we believe is close enough.

Quality of the code

-   What is the quality of the code produced? Are the test cases good enough to prevent regressions? How good is an architecture at mitigating risk and changes?
    Attention from engineers
-   How frequently do engineers reach a state of flow? How much are they distracted by notifications? Does a tool encourage engineers to context switch?
    Intellectual complexity
-   How much cognitive load is required to complete a task? What is the inherent complexity of the problem being solved? Do engineers need to deal with unnecessary complexity?
    Tempo and velocity
-   How quickly can engineers accomplish their tasks? How fast can they push their releases out? How many tasks do they complete in a given timeframe?
    Satisfaction
-   How happy are engineers with their tools? How well does a tool meet engineers’ needs? How satisfied are they with their work and their end product? Are engineers feeling burned out?

#### TL;DRs

-   Before measuring productivity, ask whether the result is actionable, regardless of whether the result is positive or negative. If you can’t do anything with the result, it is likely not worth measuring.
-   Select meaningful metrics using the GSM framework. A good metric is a reasonable proxy to the signal you’re trying to measure, and it is traceable back to your original goals.
-   Select metrics that cover all parts of productivity (QUANTS). By doing this, you ensure that you aren’t improving one aspect of productivity (like developer velocity) at the cost of another (like code quality).
-   Qualitative metrics are metrics, too! Consider having a survey mechanism for tracking longitudinal metrics about engineers’ beliefs. Qualitative metrics should also align with the quantitative metrics; if they do not, it is likely the quantitative metrics that are incorrect.
-   Aim to create recommendations that are built into the developer workflow and incentive structures. Even though it is sometimes necessary to recommend additional training or documentation, change is more likely to occur if it is built into the developer’s daily habits.

## Part III. Processes

### Chapter 8. Style Guides and Rules

Rules are laws. They are not just suggestions or recommendations, but strict, mandatory laws. As such, they are universally enforceable—rules may not be disregarded except as approved on a need-to-use basis. In contrast to rules, guidance provides recommendations and best practices. These bits are good to follow, even highly advisable to follow, but unlike rules, they usually have some room for variance.

So why do we have rules? The goal of having rules in place is to encourage “good” behavior and discourage “bad” behavior.

When defining a set of rules, the key question is not, “What rules should we have?” The question to ask is, “What goal are we trying to advance?”

We recognize a number of overarching principles that guide the development of our rules, which must:

-   Pull their weight
-   Optimize for the reader
-   Be consistent
-   Avoid error-prone and surprising constructs
-   Concede to practicalities when necessary

Given the passage of time, our code will be read far more frequently than it is written. We’d rather the code be tedious to type than difficult to read.

We value “simple to read” over “simple to write.”

When a codebase is internally consistent in its style and norms, engineers writing code and others reading it can focus on what’s getting done rather than how it is presented.

Consistency also ensures resilience to time. As time passes, engineers leave projects, new people join, ownership shifts, and projects merge or split. Striving for a consistent codebase ensures that these transitions are low cost and allows us nearly unconstrained fluidity for both the code and the engineers working on it, simplifying the processes necessary for long-term maintenance.

There are roughly three categories into which all style guide rules fall:

-   Rules to avoid dangers
-   Rules to enforce best practices
-   Rules to ensure consistency

Guidance represents the collected wisdom of our engineering experience, documenting the best practices that we’ve extracted from the lessons learned along the way. Guidance tends to focus on things that we’ve observed people frequently getting wrong or new things that are unfamiliar and therefore subject to confusion. If the rules are the “musts,” our guidance is the “shoulds.”

Some of the useful references that we maintain internally include the following:

-   Language-specific advice for the areas that are generally more difficult to get correct (such as concurrency and hashing).
-   Detailed breakdowns of new features that are introduced with a language update and advice on how to use them within the codebase.
-   Listings of key abstractions and data structures provided by our libraries. This keeps us from reinventing structures that already exist and provides a response to, “I need a thing, but I don’t know what it’s called in our libraries.”

When it comes to the size of a given code change (i.e., the number of files affected and lines modified) we recommend that engineers favor smaller changes. Small changes are easier for engineers to review, so reviews tend to be faster and more thorough. They’re also less likely to introduce bugs because it’s easier to reason about the potential impact and effects of a smaller change. The definition of small, however, is somewhat nebulous. A change that propagates the identical one-line update across hundreds of files might actually be easy to review. By contrast, a smaller, 20-line change might introduce complex logic with side effects that are difficult to evaluate.

Many rules covering language usage can be enforced with static analysis tools.

#### TL;DRs

-   Rules and guidance should aim to support resilience to time and scaling.
-   Know the data so that rules can be adjusted.
-   Not everything should be a rule.
-   Consistency is key.
-   Automate enforcement when possible.

Many of our style guides have external versions, which you can find at https://google.github.io/styleguide. We cite numerous examples from these guides within this chapter.

### Chapter 9. Code Review

Some organizations have a select group of “gatekeepers” across the codebase that review changes.

It’s important to remember (and accept) that code itself is a liability. It might be a necessary liability, but by itself, code is simply a maintenance task to someone somewhere down the line. Much like the fuel that an airplane carries, it has weight, though it is, of course, necessary for that airplane to fly.

Specially named OWNERS files list usernames of people who have ownership responsibilities for a directory and its children.

A well-designed code review process and a culture of taking code review seriously provides the following benefits:

-   Checks code correctness
-   Ensures the code change is comprehensible to other engineers
-   Enforces consistency across the codebase
-   Psychologically promotes team ownership
-   Enables knowledge sharing
-   Provides a historical record of the code review itself

A study at IBM found that discovering defects earlier in a process, unsurprisingly, led to less time required to fix them later on.5 The investment in the time for code review saved time otherwise spent in testing, debugging, and performing regressions, provided that the code review process itself was streamlined to keep it lightweight. This latter point is important; code review processes that are heavyweight, or that don’t scale properly, become unsustainable.

To prevent the evaluation of correctness from becoming more subjective than objective, authors are generally given deference to their particular approach, whether it be in the design or the function of the introduced change. A reviewer shouldn’t propose alternatives because of personal opinion. Reviewers can propose alternatives, but only if they improve comprehension (by being less complex, for example) or functionality (by being more efficient, for example).

A code review is often the first test of whether a given change is understandable to a broader audience. This perspective is vitally important because code will be read many more times than it is written, and understanding and comprehension are critically important.

Unlike the deference reviewers should give authors regarding design decisions, it’s often useful to treat questions on code comprehension using the maxim “the customer is always right.”

Reviewers can assess how well this code lives up to the standards of the codebase itself during code review. A code review, therefore, should act to ensure code health.

Code review, when it works best, provides not only a challenge to an engineer’s assumptions, but also does so in a prescribed, neutral manner, acting to temper any criticism which might otherwise be directed to the author if provided in an unsolicited manner. After all, the process requires critical review (we in fact call our code review tool “Critique”), so you can’t fault a reviewer for doing their job and being critical. The code review process itself, therefore, can act as the “bad cop,” whereas the reviewer can still be seen as the “good cop.”

A Google engineer’s primary task is still programming, of course, but a large chunk of their time is still spent in code review.

At Google, we expect feedback from a code review within 24 (working) hours. If a reviewer is unable to complete a review in that time, it’s good practice (and expected) to respond that they’ve at least seen the change and will get to the review as soon as possible. Reviewers should avoid responding to the code review in piecemeal fashion. Few things annoy an author more than getting feedback from a review, addressing it, and then continuing to get unrelated further feedback in the review process.

As much as we expect professionalism on the part of the reviewer, we expect professionalism on the part of the author as well. Remember that you are not your code, and that this change you propose is not “yours” but the team’s.

“Small” changes should generally be limited to about 200 lines of code.

About 35% of the changes at Google are to a single file.

There is a tendency within the industry, and within individuals, to try to get additional input (and unanimous consent) from a cross-section of engineers. After all, each additional reviewer can add their own particular insight to the code review in question. But we’ve found that this leads to diminishing returns; the most important LGTM is the first one, and subsequent ones don’t add as much as you might think to the equation. The cost of additional reviewers quickly outweighs their value.

Some of the best modifications to a codebase are actually deletions! Getting rid of dead or obsolete code is one of the best ways to improve the overall code health of a codebase.

Inevitably, you will need to submit a change for a bug fix to your codebase. When doing so, avoid the temptation to address other issues. Not only does this risk increasing the size of the code review, it also makes it more difficult to perform regression testing or for others to roll back your change. A bug fix should focus solely on fixing the indicated bug and (usually) updating associated tests to catch the error that occurred in the first place.

#### TL;DRs

-   Code review has many benefits, including ensuring code correctness, comprehension, and consistency across a codebase.
-   Always check your assumptions through someone else; optimize for the reader.
-   Provide the opportunity for critical feedback while remaining professional.
-   Code review is important for knowledge sharing throughout an organization.
-   Automation is critical for scaling the process.
-   The code review itself provides a historical record.

### Chapter 10. Documentation

After all, you might write a document only once,1 but it will be read hundreds, perhaps thousands of times afterward; its initial cost is amortized across all the future readers. Not only does documentation scale over time, but it is critical for the rest of the organization to scale as well. It helps answer questions like these:

-   Why were these design decisions made?
-   Why did we implement this code in this manner?
-   Why did I implement this code in this manner, if you’re looking at your own code two years later?

Documentation is often so tightly coupled to code that it should, as much as possible, be treated as code. That is, your documentation should:

-   Have internal policies or rules to be followed
-   Be placed under source control
-   Have clear ownership responsible for maintaining the docs
-   Undergo reviews for changes (and change with the code it documents)
-   Have issues tracked, as bugs are tracked in code
-   Be periodically evaluated (tested, in some respect)
-   If possible, be measured for aspects such as accuracy, freshness, etc. (tools have still not caught up here)

One of the most important mistakes that engineers make when writing documentation is to write only for themselves.

Always try to identify a primary audience and write to that audience.

Another important audience distinction is based on how a user encounters a document:

-   Seekers are engineers who know what they want and want to know if what they are looking at fits the bill. A key pedagogical device for this audience is consistency. If you are writing reference documentation for this group—within a code file, for example—you will want to have your comments follow a similar format so that readers can quickly scan a reference and see whether they find what they are looking for.
-   Stumblers might not know exactly what they want. They might have only a vague idea of how to implement what they are working with. The key for this audience is clarity. Provide overviews or introductions (at the top of a file, for example) that explain the purpose of the code they are looking at. It’s also useful to identify when a doc is not appropriate for an audience. A lot of documents at Google begin with a “TL;DR statement” such as “TL;DR: if you are not interested in C++ compilers at Google, you can stop reading now.”

There are several main types of documents that software engineers often need to write:

-   Reference documentation, including code comments
-   Design documents
-   Tutorials
-   Conceptual documentation
-   Landing pages

Almost all code files at Google must contain a file comment.

All free functions, or public methods of a class, at Google must also contain a function comment describing what the function does. Function comments should stress the active nature of their use, beginning with an indicative verb describing what the function does and what is returned.

Often, the best time to write a tutorial, if one does not yet exist, is when you first join a team. (It’s also the best time to find bugs in any existing tutorial you are following.)

At Google, we often attach “freshness dates” to documentation. Such documents note the last time a document was reviewed, and metadata in the documentation set will send email reminders when the document hasn’t been touched in, for example, three months. Such freshness dates, as shown in the following example—and tracking your documents as bugs—can help make a documentation set easier to maintain over time, which is the main concern for a document:

```
freshness: { owner: `username` reviewed: '2019-02-27' }
```

#### TL;DRs

-   Documentation is hugely important over time and scale.
-   Documentation changes should leverage the existing developer workflow.
-   Keep documents focused on one purpose.
-   Write for your audience, not yourself.

### Chapter 11. Testing Overview

“Catching bugs” is only part of the motivation of writing tests. An equally important reason why you want to test your software is to support the ability to change. Whether you’re adding new features, doing a refactoring focused on code health, or undertaking a larger redesign, automated testing can quickly catch mistakes, and this makes it possible to change software with confidence.

At Google, we have determined that testing cannot be an afterthought. Focusing on quality and testing is part of how we do our jobs. We have learned, sometimes painfully, that failing to build quality into our products and services inevitably leads to bad outcomes. As a result, we have built testing into the heart of our engineering culture.

Investing in software tests provides several key benefits to developer productivity:

-   Less debugging. As you would expect, tested code has fewer defects when it is submitted. Critically, it also has fewer defects throughout its existence; most of them will be caught before the code is submitted. A piece of code at Google is expected to be modified dozens of times in its lifetime. It will be changed by other teams and even automated code maintenance systems. A test written once continues to pay dividends and prevent costly defects and annoying debugging sessions through the lifetime of the project. Changes to a project, or the dependencies of a project, that break a test can be quickly detected by test infrastructure and rolled back before the problem is ever released to production.
-   Increased confidence in changes. All software changes. Teams with good tests can review and accept changes to their project with confidence because all important behaviors of their project are continuously verified. Such projects encourage refactoring. Changes that refactor code while preserving existing behavior should (ideally) require no changes to existing tests.
-   Improved documentation. Software documentation is notoriously unreliable. From outdated requirements to missing edge cases, it is common for documentation to have a tenuous relationship to the code. Clear, focused tests that exercise one behavior at a time function as executable documentation. If you want to know what the code does in a particular case, look at the test for that case. Even better, when requirements change and new code breaks an existing test, we get a clear signal that the “documentation” is now out of date. Note that tests work best as documentation only if care is taken to keep them clear and concise.
-   Simpler reviews. All code at Google is reviewed by at least one other engineer before it can be submitted (see Chapter 9 for more details). A code reviewer spends less effort verifying code works as expected if the code review includes thorough tests that demonstrate code correctness, edge cases, and error conditions. Instead of the tedious effort needed to mentally walk each case through the code, the reviewer can verify that each case has a passing test.
-   Thoughtful design. Writing tests for new code is a practical means of exercising the API design of the code itself. If new code is difficult to test, it is often because the code being tested has too many responsibilities or difficult-to-manage dependencies. Well-designed code should be modular, avoiding tight coupling and focusing on specific responsibilities. Fixing design issues early often means less rework later.
-   Fast, high-quality releases. With a healthy automated test suite, teams can release new versions of their application with confidence. Many projects at Google release a new version to production every day—even large projects with hundreds of engineers and thousands of code changes submitted every day. This would not be possible without automated testing.

In some cases, you can limit the impact of flaky tests by automatically rerunning them when they fail. This is effectively trading CPU cycles for engineering time.

All tests should strive to be hermetic: a test should contain all of the information necessary to set up, execute, and tear down its environment. Tests should assume as little as possible about the outside environment, such as the order in which the tests are run. For example, they should not rely on a shared database.

We also strongly discourage the use of control flow statements like conditionals and loops in a test. More complex test flows risk containing bugs themselves and make it more difficult to determine the cause of a test failure.

As a very rough guideline, we tend to aim to have a mix of around 80% of our tests being narrow-scoped unit tests that validate the majority of our business logic; 15% medium-scoped integration tests that validate the interactions between two or more components; and 5% end-to-end tests that validate the entire system.

Test everything that you don’t want to break. We have a name for this general philosophy: we call it the Beyoncé Rule. Succinctly, it can be stated as follows: “If you liked it, then you shoulda put a test on it.”

Code coverage is a measure of which lines of feature code are exercised by which tests. If you have 100 lines of code and your tests execute 90 of them, you have 90% code coverage.

#### TL;DRs

-   Automated testing is foundational to enabling software to change.
-   For tests to scale, they must be automated.
-   A balanced test suite is necessary for maintaining healthy test coverage.
-   “If you liked it, you should have put a test on it.”
-   Changing the testing culture in organizations takes time.

### Chapter 12. Unit Testing

Google puts a lot of focus on test maintainability. Maintainable tests are ones that “just work”: after writing them, engineers don’t need to think about them again until they fail, and those failures indicate real bugs with clear causes.

A brittle test is one that fails in the face of an unrelated change to production code that does not introduce any real bugs.

Therefore, the ideal test is unchanging: after it’s written, it never needs to change unless the requirements of the system under test change.

Tests using only public APIs are, by definition, accessing the system under test in the same manner that its users would. Such tests are more realistic and less brittle because they form explicit contracts: if such a test breaks, it implies that an existing user of the system will also be broken. Testing only these contracts means that you’re free to do whatever internal refactoring of the system you want without having to worry about making tedious changes to tests.

If a method or class exists only to support one or two other classes (i.e., it is a “helper class”), it probably shouldn’t be considered its own unit, and its functionality should be tested through those classes instead of directly.

With state testing, you observe the system itself to see what it looks like after invoking with it. With interaction testing, you instead check that the system took an expected sequence of actions on its collaborators in response to invoking it.

Two high-level properties that help tests achieve clarity are completeness and conciseness. A test is complete when its body contains all of the information a reader needs in order to understand how it arrives at its result. A test is concise when it contains no other distracting or irrelevant information.

It can often be worth violating the DRY (Don’t Repeat Yourself) principle if it leads to clearer tests. Remember: a test’s body should contain all of the information needed to understand it without containing any irrelevant or distracting information.

Behaviors can often be expressed using the words “given,” “when,” and “then”: “Given that a bank account is empty, when attempting to withdraw money from it, then the transaction is rejected.”

When writing such tests, be careful to ensure that you’re not inadvertently testing multiple behaviors at the same time. Each test should cover only a single behavior, and the vast majority of unit tests require only one “when” and one “then” block.

Instead of being completely DRY, test code should often strive to be DAMP—that is, to promote “Descriptive And Meaningful Phrases.” A little bit of duplication is OK in tests so long as that duplication makes the test simpler and clearer.

### Chapter 13. Test Doubles

Fidelity refers to how closely the behavior of a test double resembles the behavior of the real implementation that it’s replacing.

A seam is a way to make code testable by allowing for the use of test doubles—it makes it possible to use different dependencies for the system under test rather than the dependencies used in a production environment.

Dependency injection is a common technique for introducing seams. In short, when a class utilizes dependency injection, any classes it needs to use (i.e., the class’s dependencies) are passed to it rather than instantiated directly, making it possible for these dependencies to be substituted in tests.

At Google, Guice and Dagger are automated dependency injection frameworks that are commonly used for Java code.

Stubbing is the process of giving behavior to a function that otherwise has no behavior on its own—you specify to the function exactly what values to return (that is, you stub the return values).

Stubbing is typically done through mocking frameworks to reduce boilerplate that would otherwise be needed for manually creating new classes that hardcode return values.

Interaction testing is sometimes called mocking. We avoid this terminology in this chapter because it can be confused with mocking frameworks, which can be used for stubbing as well as for interaction testing.

Preferring real implementations in tests is known as classical testing.

A real implementation is preferred if it is fast, deterministic, and has simple dependencies.

Parellelization of tests can also help reduce execution time. At Google, our test infrastructure makes it trivial to split up tests in a test suite to be executed across multiple servers. This increases the cost of CPU time, but it can provide a large savings in developer time.

A test is deterministic if, for a given version of the system under test, running the test always results in the same outcome; that is, the test either always passes or always fails. In contrast, a test is nondeterministic if its outcome can change, even if the system under test remains unchanged.

Rather than a catch-all replacement for a real implementation, stubbing is appropriate when you need a function to return a specific value to get the system under test into a certain state.

At Google, we’ve found that emphasizing state testing is more scalable; it reduces test brittleness, making it easier to change and maintain code over time.

The primary issue with interaction testing is that it can’t tell you that the system under test is working properly; it can only validate that certain functions are called as expected.

#### TL;DRs

-   A real implementation should be preferred over a test double.
-   A fake is often the ideal solution if a real implementation can’t be used in a test.
-   Overuse of stubbing leads to tests that are unclear and brittle.
-   Interaction testing should be avoided when possible: it leads to tests that are brittle because it exposes implementation details of the system under test.

### Chapter 14. Larger Testing

Larger tests are many things that small tests are not. They are not bound by the same constraints; thus, they can exhibit the following characteristics:

-   They may be slow. Our large tests have a default timeout of 15 minutes or 1 hour, but we also have tests that run for multiple hours or even days.
-   They may be nonhermetic. Large tests may share resources with other tests and traffic.
-   They may be nondeterministic. If a large test is nonhermetic, it is almost impossible to guarantee determinism: other tests or user state may interfere with it.

Fidelity is the property by which a test is reflective of the real behavior of the system under test (SUT).

Production itself is, naturally, the environment of highest fidelity in testing.

At Google, configuration changes are the number one reason for our major outages.

Hyrum’s Law is an important consideration here: even if we could test 100% for conformance to a strict, specified contract, the effective user contract applies to all visible behaviors, not just a stated contract. It is unlikely that unit tests alone test for all visible behaviors that are not specified in the public API.

Without clear ownership, a test rots.

There are particularly painful testing boundaries that might be worth avoiding. Tests that involve both frontends and backends become painful because user interface (UI) tests are notoriously unreliable and costly.

What follows is a list of different kinds of large tests that we use at Google, how they are composed, what purpose they serve, and what their limitations are:

-   Functional testing of one or more binaries
-   Browser and device testing
-   Performance, load, and stress testing
-   Deployment configuration testing
-   Exploratory testing
-   A/B diff (regression) testing
-   User acceptance testing (UAT)
-   Probers and canary analysis
-   Disaster recovery and chaos engineering
-   User evaluation

Exploratory testing2 is a form of manual testing that focuses not on looking for behavioral regressions by repeating known test flows, but on looking for questionable behavior by trying out new user scenarios. Trained users/testers interact with a product through its public APIs, looking for new paths through the system and for which behavior deviates from either expected or intuitive behavior, or if there are security vulnerabilities.

Exploratory testing is useful for both new and launched systems to uncover unanticipated behaviors and side effects. By having testers follow different reachable paths through the system, we can increase the system coverage and, when these testers identify bugs, capture new automated functional tests. In a sense, this is a bit like a manual “fuzz testing” version of functional integration testing.

One common approach we use for manual exploratory testing is the bug bash.

Probers should be used in any live system. If the production rollout process includes a phase in which the binary is deployed to a limited subset of the production machines (a canary phase), canary analysis should be used during that procedure.

Made popular by Netflix, chaos engineering involves writing programs that continuously introduce a background level of faults into your systems and seeing what happens.

#### TL;DRs

-   Larger tests cover things unit tests cannot.
-   Large tests are composed of a System Under Test, Data, Action, and Verification.
-   A good design includes a test strategy that identifies risks and larger tests that mitigate them.
-   Extra effort must be made with larger tests to keep them from creating friction in the developer workflow.

### Chapter 15. Deprecation

We refer to the process of orderly migration away from and eventual removal of obsolete systems as deprecation.

For long-running software ecosystems, planning for and executing deprecation correctly reduces resource costs and improves velocity by removing the redundancy and complexity that builds up in a system over time.

Deprecation is best suited for systems that are demonstrably obsolete and a replacement exists that provides comparable functionality. The new system might use resources more efficiently, have better security properties, be built in a more sustainable fashion, or just fix bugs.

In the long run, we’ve discovered that having multiple systems performing the same function also impedes the evolution of the newer system because it is still expected to maintain compatibility with the old one. Spending the effort to remove the old system can pay off as the replacement system can now evolve more quickly.

Code itself doesn’t bring value: it is the functionality that it provides that brings value. That functionality is an asset if it meets a user need: the code that implements this functionality is simply a means to that end.

Code itself carries a cost—the simpler the code is, while maintaining the same amount of functionality, the better.

The more users of a system, the higher the probability that users are using it in unexpected and unforeseen ways, and the harder it will be to deprecate and remove such a system.

Finally, funding and executing deprecation efforts can be difficult politically; staffing a team and spending time removing obsolete systems costs real money, whereas the costs of doing nothing and letting the system lumber along unattended are not readily observable.

The concept of designing systems so that they can eventually be deprecated might be radical in software engineering, but it is common in other engineering disciplines. Consider the example of a nuclear power plant.

In short, don’t start projects that your organization isn’t committed to support for the expected lifespan of the organization.

Advisory deprecations are those that don’t have a deadline and aren’t high priority for the organization (and for which the company isn’t willing to dedicate resources).

As our friends in SRE will readily tell you: “Hope is not a strategy.”

Compulsory deprecation: this kind of deprecation usually comes with a deadline for removal of the obsolete system: if users continue to depend on it beyond that date, they will find their own systems no longer work.

These sorts of important-not-urgent cleanup tasks are a great use of 20% time and provide engineers exposure to other parts of the codebase.

Deprecation can feel like the dirty work of cleaning up the street after the circus parade has just passed through town, yet these efforts improve the overall software ecosystem by reducing maintenance overhead and cognitive burden of engineers.

TL;DRs

-   Software systems have continuing maintenance costs that should be weighed against the costs of removing them.
-   Removing things is often more difficult than building them to begin with because existing users are often using the system beyond its original design.
-   Evolving a system in place is usually cheaper than replacing it with a new one, when turndown costs are included.
-   It is difficult to honestly evaluate the costs involved in deciding whether to deprecate: aside from the direct maintenance costs involved in keeping the old system around, there are ecosystem costs involved in having multiple similar systems to choose between and that might need to interoperate. The old system might implicitly be a drag on feature development for the new. These ecosystem costs are diffuse and difficult to measure. Deprecation and removal costs are often similarly diffuse.

## Part IV. Tools

### Chapter 16. Version Control and Branch Management

Trunk-based development relies heavily on testing and CI, keep the build green, and disable incomplete/untested features at runtime.

If the period between releases (or the release lifetime) for a product is longer than a few hours, it may be sensible to create a release branch that represents the exact code that went into the release build for your product. If any critical flaws are discovered between the actual release of that product into the wild and the next release cycle, fixes can be cherry-picked (a minimal, targeted merge) from trunk to your release branch.

#### TL;DRs

-   Use version control for any software development project larger than “toy project with only one developer that will never be updated.”
-   There’s an inherent scaling problem when there are choices in “which version of this should I depend upon?”
-   One-Version Rules are surprisingly important for organizational efficiency. Removing choices in where to commit or what to depend upon can result in significant simplification.
-   In some languages, you might be able to spend some effort to dodge this with technical approaches like shading, separate compilation, linker hiding, and so on. The work to get those approaches working is entirely lost labor—your software engineers aren’t producing anything, they’re just working around technical debts.
-   Previous research (DORA/State of DevOps/Accelerate) has shown that trunk-based development is a predictive factor in high-performing development organizations. Long-lived dev branches are not a good default plan.
-   Use whatever version control system makes sense for you. If your organization wants to prioritize separate repositories for separate projects, it’s still probably wise for interrepository dependencies to be unpinned/“at head”/“trunk based.” There are an increasing number of VCS and build system facilities that allow you to have both small, fine-grained repositories as well as a consistent “virtual” head/trunk notion for the whole organization.

### Chapter 17. Code Search

#### TL;DRs

-   Helping your developers understand code can be a big boost to engineering productivity. At Google, the key tool for this is Code Search.
-   Code Search has additional value as a basis for other tools and as a central, standard place that all documentation and developer tools link to.
-   The huge size of the Google codebase made a custom tool—as opposed to, for example, grep or an IDE’s indexing—necessary.
-   As an interactive tool, Code Search must be fast, allowing a “question and answer” workflow. It is expected to have low latency in every respect: search, browsing, and indexing.
-   It will be widely used only if it is trusted, and will be trusted only if it indexes all code, gives all results, and gives the desired results first. However, earlier, less powerful, versions were both useful and used, as long as their limits were understood.

### Chapter 18. Build Systems and Build Philosophy

In 2015, Google finally open sourced an implementation of Blaze named Bazel.

Fundamentally, all build systems have a straightforward purpose: they transform the source code written by engineers into executable binaries that can be read by machines. A good build system will generally try to optimize for two important properties:

-   Fast: A developer should be able to type a single command to run the build and get back the resulting binary, often in as little as a few seconds.
-   Correct: Every time any developer runs a build on any machine, they should get the same result (assuming that the source files and other inputs are the same).

Most major build systems in use today, such as Ant, Maven, Gradle, Grunt, and Rake, are task based.

The problem with such systems is that they actually end up giving too much power to engineers and not enough power to the system. Because the system has no idea what the scripts are doing, performance suffers, as it must be very conservative in how it schedules and executes build steps.

A build system’s primary task should be to build code. Engineers would still need to tell the system what to build, but the how of doing the build would be left to the system.

This is exactly the approach taken by Blaze and the other artifact-based build systems descended from it (which include Bazel, Pants, and Buck).

Bazel and some other build systems address this problem by requiring a workspace-wide manifest file that lists a cryptographic hash for every external dependency in the workspace.

Of course, it can still be a problem if a remote server becomes unavailable or starts serving corrupt data—this can cause all of your builds to begin failing if you don’t have another copy of that dependency available. To avoid this problem, we recommend that, for any nontrivial project, you mirror all of its dependencies onto servers or services that you trust and control. Otherwise you will always be at the mercy of a third party for your build system’s availability, even if the checked-in hashes guarantee its security.

TL;DRs

-   A fully featured build system is necessary to keep developers productive as an organization scales.
-   Power and flexibility come at a cost. Restricting the build system appropriately makes it easier on developers.
-   Build systems organized around artifacts tend to scale better and be more reliable than build systems organized around tasks.
-   When defining artifacts and dependencies, it’s better to aim for fine-grained modules. Fine-grained modules are better able to take advantage of parallelism and incremental builds.
-   External dependencies should be versioned explicitly under source control. Relying on “latest” versions is a recipe for disaster and unreproducible builds.

### Chapter 19. Critique: Google’s Code Review Tool

Code review is not for slowing others down; instead, it is for empowering others. Trusting colleagues as much as possible makes it work.

Larger changes are typically more difficult to understand than smaller ones. Optimizing the diff of a change is thus a core requirement for a good code review tool.

An LGTM stamp from a reviewer means that “I have reviewed this change, believe that it meets our standards, and I think it is okay to commit it after addressing unresolved comments.” An Approval stamp from a reviewer means that “as a gatekeeper, I allow this change to be committed to the codebase.”

TL;DRs

-   Trust and communication are core to the code review process. A tool can enhance the experience, but it can’t replace them.
-   Tight integration with other tools is key to great code review experience.
-   Small workflow optimizations, like the addition of an explicit “attention set,” can increase clarity and reduce friction substantially.

### Chapter 20. Static Analysis

Static analysis refers to programs analyzing source code to find potential issues such as bugs, antipatterns, and other issues that can be diagnosed without executing the program.

For example, static analysis can identify constant expressions that overflow, tests that are never run, or invalid format strings in logging statements that would crash when executed.

Static analysis tools at Google must scale to the size of Google’s multibillion-line codebase. To do this, analysis tools are shardable and incremental. Instead of analyzing entire large projects, we focus analyses on files affected by a pending code change, and typically show analysis results only for edited files or lines.

We generally focus on newly introduced warnings; existing issues in otherwise working code are typically only worth highlighting (and fixing) if they are particularly important (security issues, significant bug fixes, etc.). Focusing on newly introduced warnings (or warnings on modified lines) also means that the developers viewing the warnings have the most relevant context on them.

#### TL;DRs

-   Focus on developer happiness. We have invested considerable effort in building feedback channels between analysis users and analysis writers in our tools, and aggressively tune analyses to reduce the number of false positives.
-   Make static analysis part of the core developer workflow. The main integration point for static analysis at Google is through code review, where analysis tools provide fixes and involve reviewers. However, we also integrate analyses at additional points (via compiler checks, gating code commits, in IDEs, and when browsing code).
-   Empower users to contribute. We can scale the work we do building and maintaining analysis tools and platforms by leveraging the expertise of domain experts. Developers are continuously adding new analyses and checks that make their lives easier and our codebase better.

### Chapter 21. Dependency Management

Much of the difficulty stems from one problem: what happens when two nodes in the dependency network have conflicting requirements, and your organization depends on them both?

Meanwhile, C++ has nearly zero tolerance for diamond dependencies in a normal build, and they are very likely to trigger arbitrary bugs and undefined behavior (UB) as a result of a clear violation of C++’s One Definition Rule.

The de facto standard for “how do we manage a network of dependencies today?” is semantic versioning (SemVer). SemVer is the nearly ubiquitous practice of representing a version number for some dependency (especially libraries) using three decimal-separated integers, such as 2.4.72 or 1.1.4. In the most common convention, the three component numbers represent major, minor, and patch versions, with the implication that a changed major number indicates a change to an existing API that can break existing usage, a changed minor number indicates purely added functionality that should not break existing usage, and a changed patch version is reserved for non-API-impacting implementation details and bug fixes that are viewed as particularly low risk.

As your dependency network scales up, both in the size of each dependency and the number of dependencies (as well as any monorepo effects from having multiple projects depending on the same network of external dependencies), the compounded fidelity loss in SemVer will begin to dominate. These failures manifest as both false positives (practically incompatible versions that theoretically should have worked) and false negatives (compatible versions disallowed by SAT-solvers and resulting dependency hell).

There are two major ways that an innocuous and hopefully charitable act like “open sourcing a library” can become a possible loss for an organization. First, it can eventually become a drag on the reputation of your organization if implemented poorly or not maintained properly. As the Apache community saying goes, we ought to prioritize “community over code.” If you provide great code but are a poor community member, that can still be harmful to your organization and the broader community. Second, a well-intentioned release can become a tax on engineering efficiency if you can’t keep things in sync. Given time, all forks will become expensive.

Don’t release things without a plan (and a mandate) to support it for the long term.

#### TL;DRs

-   Prefer source control problems to dependency management problems: if you can get more code from your organization to have better transparency and coordination, those are important simplifications.
-   Adding a dependency isn’t free for a software engineering project, and the complexity in establishing an “ongoing” trust relationship is challenging. Importing dependencies into your organization needs to be done carefully, with an understanding of the ongoing support costs.
-   A dependency is a contract: there is a give and take, and both providers and consumers have some rights and responsibilities in that contract. Providers should be clear about what they are trying to promise over time.
-   SemVer is a lossy-compression shorthand estimate for “How risky does a human think this change is?” SemVer with a SAT-solver in a package manager takes those estimates and escalates them to function as absolutes. This can result in either overconstraint (dependency hell) or underconstraint (versions that should work together that don’t).
-   By comparison, testing and CI provide actual evidence of whether a new set of versions work together.
-   Minimum-version update strategies in SemVer/package management are higher fidelity. This still relies on humans being able to assess incremental version risk accurately, but distinctly improves the chance that the link between API provider and consumer has been tested by an expert.
-   Unit testing, CI, and (cheap) compute resources have the potential to change our understanding and approach to dependency management. That phase-change requires a fundamental change in how the industry considers the problem of dependency management, and the responsibilities of providers and consumers both.
-   Providing a dependency isn’t free: “throw it over the wall and forget” can cost you reputation and become a challenge for compatibility. Supporting it with stability can limit your choices and pessimize internal usage. Supporting without stability can cost goodwill or expose you to risk of important external groups depending on something via Hyrum’s Law and messing up your “no stability” plan.

### Chapter 22. Large-Scale Changes

The SREs who run Google’s production services have a mantra: “No Haunted Graveyards.” A haunted graveyard in this sense is a system that is so ancient, obtuse, or complex that no one dares enter it. Haunted graveyards are often business-critical systems that are frozen in time because any attempt to change them could cause the system to fail in incomprehensible ways, costing the business real money. They pose a real existential risk and can consume an inordinate amount of resources.

Nobody wants to be the network support engineer II who flipped the wrong bit!

#### TL;DRs

-   An LSC process makes it possible to rethink the immutability of certain technical decisions.
-   Traditional models of refactoring break at large scales.
-   Making LSCs means making a habit of making LSCs.

### Chapter 23. Continuous Integration

Continuous Integration, or CI, is generally defined as “a software development practice where members of a team integrate their work frequently. Each integration is verified by an automated build (including test) to detect integration errors as quickly as possible.” Simply put, the fundamental goal of CI is to automatically catch problematic changes as early as possible.

To minimize the cost of bugs, CI encourages us to use fast feedback loops.3 Each time we integrate a code (or other) change into a testing scenario and observe the results, we get a new feedback loop. Feedback can take many forms; following are some common ones (in order of fastest to slowest):

-   The edit-compile-debug loop of local development
-   Automated test results to a code change author on presubmit
-   An integration error between changes to two projects, detected after both are submitted and tested together (i.e., on post-submit)
-   An incompatibility between our project and an upstream microservice dependency, detected by a QA tester in our staging environment, when the upstream service deploys its latest changes
-   Bug reports by internal users who are opted in to a feature before external users
-   Bug or outage reports by external users or the press

Canarying—or deploying to a small percentage of production first—can help minimize issues that do make it to production, with a subset-of-production initial feedback loop preceding all-of-production.

Experiments and feature flags are extremely powerful feedback loops. They reduce deployment risk by isolating changes within modular components that can be dynamically toggled in production. Relying heavily on feature-flag-guarding is a common paradigm for Continuous Delivery.

Continuous Delivery (CD): a continuous assembling of release candidates, followed by the promotion and testing of those candidates throughout a series of environments—sometimes reaching production and sometimes not.

We don’t want to waste valuable engineer productivity by waiting too long for slow tests or for too many tests—we typically limit presubmit tests to just those for the project where the change is happening. We also run tests concurrently, so there is a resource decision to consider as well.

Hermetic tests: tests run against a test environment (i.e., application servers and resources) that is entirely self-contained (i.e., no external dependencies like production backends).

#### TL;DRs

-   A CI system decides what tests to use, and when.
-   CI systems become progressively more necessary as your codebase ages and grows in scale.
-   CI should optimize quicker, more reliable tests on presubmit and slower, less deterministic tests on post-submit.
-   Accessible, actionable feedback allows a CI system to become more efficient.

### Chapter 24. Continuous Delivery

Martin Fowler, in his book Continuous Delivery (aka CD), points out that “The biggest risk to any software effort is that you end up building something that isn’t useful. The earlier and more frequently you get working software in front of real users, the quicker you get feedback to find out how valuable it really is.”

A core tenet of Continuous Delivery (CD) as well as of Agile methodology is that over time, smaller batches of changes result in higher quality; in other words, faster is safer.

We focus on developing various aspects that deliver value independently en route to the end goal. Here are some of these:

-   Agility: Release frequently and in small batches
-   Automation: Reduce or remove repetitive overhead of frequent releases
-   Isolation: Strive for modular architecture to isolate changes and make troubleshooting easier
-   Reliability: Measure key health indicators like crashes or latency and keep improving them
-   Data-driven decision making: Use A/B testing on health metrics to ensure quality
-   Phased rollout: Roll out changes to a few users before shipping to everyone

A key to reliable continuous releases is to make sure engineers “flag guard” all changes.

Turning on a flag for 100% of your users all at once is not a great idea, so a configuration service that manages safe configuration rollouts is a good investment. Nevertheless, the level of control and the ability to decouple the destiny of a particular feature from the overall product release are powerful levers for long-term sustainability of the application.

Faster is cheaper, because having a predictable, frequent release train forces you to drive down the cost of each release and makes the cost of any abandoned release very low.

#### TL;DRs

-   Velocity is a team sport: The optimal workflow for a large team that develops code collaboratively requires modularity of architecture and near-continuous integration.
-   Evaluate changes in isolation: Flag guard any features to be able to isolate problems early.
-   Make reality your benchmark: Use a staged rollout to address device diversity and the breadth of the userbase. Release qualification in a synthetic environment that isn’t similar to the production environment can lead to late surprises.
-   Ship only what gets used: Monitor the cost and value of any feature in the wild to know whether it’s still relevant and delivering sufficient user value.
-   Shift left: Enable faster, more data-driven decision making earlier on all changes through CI and continuous deployment.
-   Faster is safer: Ship early and often and in small batches to reduce the risk of each release and to minimize time to market.

### Chapter 25. Compute as a Service

After doing the hard work of writing code, you need some hardware to run it. Thus, you go to buy or rent that hardware. This, in essence, is Compute as a Service (CaaS), in which “Compute” is shorthand for the computing power needed to actually run your programs.

The process of deploying a binary onto each of the 50+ machines and starting it there can easily be automated through a shell script, and then—if this is to be a reusable solution—through a more robust piece of code in an easier-to-maintain language that will perform the deployment in parallel (especially since the “50+” is likely to grow over time).

More interestingly, the monitoring of each machine can also be automated.

Current open source solutions in that space are, for instance, setting up a dashboard in a monitoring tool like Graphana or Prometheus.

A classical solution to isolation is the use of virtual machines (VMs). These, however, come with significant overhead in terms of resource usage (they need the resources to run a full operating system inside) and startup time (again, they need to boot up a full operating system). This makes them a less-than-perfect solution for batch job containerization for which small resource footprints and short runtimes are expected.

If your servers are pets, your maintenance burden will grow linearly, or even superlinearly, with the size of your fleet, and that’s a burden that no organization should accept lightly. On the other hand, if your servers are cattle, your system will be able to return to a stable state after a failure, and you will not need to spend your weekend nursing a pet server or container back to health.

What is serverless? In the Borg world, the way you run this code is that you stand up a replicated container, each replica containing a server consisting of framework code and your functions. If traffic increases, you will handle this by scaling up (adding replicas or expanding into new datacenters). If traffic decreases, you will scale down. Note that a minimal presence (Google usually assumes at least three replicas in each datacenter a server is running in) is required.

First note that a serverless architecture requires your code to be truly stateless.

#### TL;DRs

-   Scale requires a common infrastructure for running workloads in production.
-   A compute solution can provide a standardized, stable abstraction and environment for software.
-   Software needs to be adapted to a distributed, managed compute environment.
-   The compute solution for an organization should be chosen thoughtfully to provide appropriate levels of abstraction.

### Conclusion
