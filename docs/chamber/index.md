# Debate Chamber Overview
??? warning "Support Notice"
    The **User Guide** is currently undergoing major re-construction, which we are aiming to complete by the end of April 2026. In the meantime please email [support@debate.report](mailto:support@debate.report)

    Thank you for your patience, and your ongoing interest in **debate.report**. We are aiming to build a world-class debate platform, and to encourage many more people to engage in meaningful debate. The platform essentially turns debating into a fun and enjoyable game for the participants, and which helps participants and the audience alike to develop and sharpen their critical-thinking skills and to come to an informed position on the important issues of the day. 

    the Debate Report Team, March 2026

---

## Introduction to the Chamber

### Debate Structure
As in most debate forums, the debates here have a formal structure which ensures a fair hearing For and Against, and a clear understanding of what is being argued. The debate.report platform ensures the integrity of the debate structure, allowing the you, the debater, to focus on what is really important - getting your points across and making them stick. 

Each debate comprises a resolution statmenet and a collection of other types of statements which are related to each other in a specific way to preserve their logical purpose. For example, the resolution should always have at least two claims attached to it, one For and the other Against, and each claim should have evidence to back it up connected to the claim via a Warrant which lays out the reasons why the evidence backs up the claim. A rebuttal statement can be lodged against most types of statement, except the resolution and the framework statement. The discussion point is not really part of the argument but simply a request for clarity, a question, or a comment. As such they also cannot be rebutted. There are more details about the different types of statement below.

If everyone follows this formal structure then the debates are much easier to read and understand, and so the <b>debate.report</b> enforces the structure for everyone’s benefit. Here is a graphical representation of the structure applied on the platform.

 <details>
    <summary>Debate Structure Diagram</summary>
    Here is a diagram that shows how the different types of statement relate to each other in an argument

    ```mermaid
    ---
    title: Debate Structure Diagram
    ---
    classDiagram
    direction TB

    class RESOLUTION {
        a formal statement that sets
        the topic for the debate
        which one side affirms
        and the other side negates
    }

    class FRAMEWORK {
        set of principles or standards
        used to evaluate the resolution
        explaining why a particular
        perspective is the best
    }

    class CLAIM {
        an assertion made by a debater
        stating a belief or position
        supported by evidence
    }

    class REBUTTAL {
        response to an opponent
        argument, where a debater
        either disagrees or refutes
        a claim, warrant or impact
    }

    class TURN {
        an argument that reverses
        the meaning or effect
        of an opponent's argument
    }

    class IMPACT {
        the consequence or significance
        of the argument, quantifying
        or evaluating how the outcome
        affects people or society
    }

    class WARRANT {
        provides the logical reason
        or justification for why
        the statement is true,
        explaining the connection  
    }

    class EVIDENCE {
        serves as the support for
        the warrant, taking the form
        of statistics, specific examples,
        testimony, or expert opinion
    }

    RESOLUTION     "1"   -->   "1"     FRAMEWORK          : "evaluated using"
    RESOLUTION     "1"   -->   "1..*"  CLAIM              : "supported or denied by"

    CLAIM          "1"   -->   "0..1"  IMPACT
    CLAIM          "1"   -->   "0..1"  TURN
    CLAIM          "1"   -->   "0..1"  WARRANT            : "justifies or proves"
    CLAIM          "1"   -->   "0..1"  REBUTTAL           : "can be rebutted"

    TURN           "1"   -->   "0..1"  CLAIM              : "turns"
    TURN           "1"   -->   "0..1"  IMPACT             : "turns"

    IMPACT         "1"   ..>   "0..1"  TURN               : "impacts"

    REBUTTAL       "1"   -->   "0..1"  TURN               : "rebutts"
    REBUTTAL       "1"   -->   "0..1"  CLAIM              : "disagrees or disproves"
    REBUTTAL       "1"   -->   "0..1"  IMPACT             : rebutts
    REBUTTAL       "1"   -->   "0..1"  WARRANT            : rebutts

    WARRANT        "1"   -->   "0..1"  CLAIM              : "justifies or proves"
    WARRANT        "1"   -->   "0..1"  REBUTTAL           : "justifies or proves"

    EVIDENCE       "*"   -->   "0..*"  WARRANT            : "supports"
    ```
    </details>


## Statement Types
### Resolution
A resolution statement in a debate serves as the central proposition that defines the topic and the specific stance to be argued, acting as the foundation for the entire discussion. It is typically a clear, concise, and balanced statement that presents a specific issue, often framed as a policy change, a factual claim, or a value judgment. The resolution sets the scope and focus of the debate, guiding the arguments and evidence presented by both sides.

The resolution is usually structured with a prefix (like "Resolved:", "This house believes that", or "Be it resolved") followed by a subject (the main topic) and a predicate (the specific claim or stance).

For example, *"Resolved: The United States federal government should adopt a universal health care system"*.
This format clearly establishes the position the affirmative team must defend and the position the negative team must oppose.

In a policy debate, the affirmative team proposes a specific plan to implement the resolution, while the negative team argues against the plan's solvency, feasibility, or desirability. In a scientific debate, the affirmative team proposes reasons why the resolution is true, which the negative team argues why it is false.

The rules for using Resolutions (sometimes called a motion or proposal) are:

- One Resolution statement is crafted by the debate moderator to clearly set out the intentions or findings to be debated. The ensuing debate will then determine the level of support for it. The resolution remains fixed throughout the debate to maintain fairness and structure.
- If the moderator wishes to change a resolution they must create a new one and request debaters to consider the new resolution and whether they want to transfer their arguments from the old one to the new one. The old resolution can then be closed.
- A Resolution can have the following types of statement attached to it: claim, framework

### Framework
A framework statement in a debate functions as the lens or set of criteria through which the judge evaluates the arguments presented during the round and ultimately determines the winner. It establishes the rules for judging by specifying how the impacts of the arguments should be prioritized and compared. Without a framework, the judge might rely on subjective judgment, such as which side was more convincing, leading to unpredictable and potentially biased outcomes. By proposing a framework, debaters essentially define how the ballot should be filled out, re-writing the implicit rule of "whoever convinces me wins" into a more structured standard.

A framework typically consists of two main parts: the method for evaluating the round (the rules) and the justification for why the judge should use that method (the warrant). Common frameworks include 

- ***cost-benefit analysis***, which weighs the advantages and disadvantages of a position
- ***utilitarianism***, which prioritizes the greatest good for the greatest number
- ***human rights***, which emphasizes moral obligations to uphold dignity
- ***national security***, which focuses on the safety of the United States.

The framework should be relevant to the resolution and support the debater's case, often being constructed to nullify the opponent's arguments and make the debater's own case easier to defend.

Debaters can argue for their framework using three types of arguments: 

- ***resolution-specific arguments***, which use the wording or intent of the resolution to justify the framework
- ***internal arguments***, which assess the fairness and practicality of the framework for the round, such as whether it places an unfair burden on one side
- ***external arguments***, which consider the broader implications of adopting a framework, such as whether it promotes a realistic or educational debate environment.

A strong framework is one that is fair, supports the debater's case, and is easy to defend.

The rules for using Frameworks are:

- One Framework statement can be attached to a Resolution. Any views or parameters necessary to frame the debate should be described in the framework statement. 
- A Framework cannot be attached to any other type of statement, only to the Resolution.

### Claim
A claim statement in a debate is a clear, arguable assertion that defines a central point of contention, serving as a foundation for an entire argument. It is a single statement of controversy that both the pro-side and con-side must debate, with the pro-side arguing for its acceptance and the con-side arguing for its rejection, thereby challenging the current status quo.

The claim must be specific, unbiased, and phrased as a statement rather than a question to ensure a focused pro-versus-con debate environment. It is essential that the claim is debatable, not merely a fact, and that it invites discussion by taking a strong, defensible position.

There can be any number of claims for a resolution, and a claim can be either for or against the resolution. 

The rules for using Claims 

- There should be at least two claims associated with a resolution, to create the cases for and against. 
- If a debater wants to create a new claim they should check existing claims to make sure someone else hasn't already made the claim. If necessary a debater can add a discussion point or attach new evidence to an existing claim rather than creating a new, perhaps only slightly different, claim. The debate structure will be much easier to understand if everyone adopts this principle.
- Each claim should have evidence to back it up and also a warrant to describe the reasons why the evidence backs up the claim. A claim should also have an impact statement. Finally, a claim my have a rebuttal statement posted against it, and may have a discussion point raised on it.

### Rebuttal
In a public forum debate, a rebuttal statement is a short statement that directly responds to an argument presented by the opposing team. The primary purpose of the rebuttal is to dismantle the opponent's case by explaining why the opponents arguments are flawed or invalid, and providing evidence or logical reasoning to support this. 
A high-quality rebuttal should include ogical reasoning, evidence, or a "turn" that reverses the opponent's argument to support the rebuttor's own position.
As well as rebutting the opponent's arguments, the rebuttor should also add claims, warrants and evidence of their own to support the case against the resolution.
The rebuttal process is crucial as it allows debaters to engage directly with their opponents' claims, weaken their case, and ultimately persuade the judge that their side is more valid.
A rebuttal may actually disprove the opposition's claim, in which case it is called a refutation.

### Turn
In a public forum debate, a turn is a response that argues the opponent's own argument actually supports the speaker's side instead of theirs. It is a strategic move where a debater concedes part of the opponent's argument but then explains how that concession leads to a conclusion favorable to their own position.
 There are two primary types of turns: link turns and impact turns.
A link turn challenges the causal connection within the opponent's argument, asserting that the link leads to the opposite outcome. This type of turn is usually applied to the claim statement which (on the debate.report platform) should include the links.
An impact turn argues that the consequence (impact) the opponent claims is actually negative for them or positive for the speaker's side, effectively reversing the value of the impact.
For example, if an opponent argues that a policy leads to economic recession (a negative impact), an impact turn would claim that the recession is actually beneficial, perhaps by stimulating innovation or forcing necessary economic reforms.
It is crucial to note that a turn is distinct from a non-unique or a de-link, which merely argue that the opponent's argument is flawed or irrelevant, rather than transforming it into offensive material for the speaker's side.

### Impact
In a public forum debate, an impact statement explains the significance or consequence of an argument, answering the question "Why does this matter?"
It is the final result of a cause-and-effect relationship that demonstrates the value or importance of the argument to the resolution.
The impact clarifies the ultimate harm or benefit that results from the argument, such as economic decline leading to poverty or war.
Effective impact statements are crucial for judges to understand which consequences are most important to weigh.


### Evidence
An evidence statement in a debate is specific, verifiable information that strengthens or proves an argument. It typically consists of a citation containing reference details like the author, date, and source, followed by a section of the author's original text, often underlined or highlighted to indicate the portion read during the debate. This evidence serves as a foundation for the reasons provided to support a claim, helping to compel the audience to accept the argument.

The evidence is used to justify the claim, and its significance must be explained via an associated warrant which
show how the evidence supports the argument.

The rules for using Evidence statements are:

- Evidence can include facts, statistics, examples, studies, testimonials, or analogies, and it must be properly attributed to an authoritative source to be valid. A link to the source can be included in the statement. Debaters are responsible for the validity of all evidence they introduce, and it must be presented accurately, without distortion, clipping, or misrepresentation.

### Warrant
An evidence statement in a debate is specific, verifiable information that strengthens or proves an argument. It typically consists of a citation containing reference details like the author, date, and source, followed by a section of the author's original text, often underlined or highlighted to indicate the portion read during the debate. This evidence serves as a foundation for the reasons provided to support a claim, helping to compel the audience to accept the argument.

The evidence is used to justify the claim, and its significance must be explained via an associated warrant which
show how the evidence supports the argument.

## Participating in a Debate

### Starting and Closing a Debate

To start a new debate you need to have the Moderator role, this allows you to create new resolutions. 
Once created, anyone with the debater role, including the moderator, can create arguments for and against the resolution. Currently debates remain open indefinitely, but coming soon is the ability to close a debate either manually or after a set period of time, i.e. anything from hours to months. Once a debate is closed it will still be visible but no more debating or voting will take place unless it is subseqently  re-opened by the moderator.

### Private Debates

Currently all resolutions are visible to everyone on the platform, although soon moderators will be able to create private debates. Private debates will be useful for organisations or communities who don’t want people outside seeing their debates. And even families who wish to encourage healthy debate and discussion within the family will be able to use private debates to get the conversations going, e.g. to explore the big questions around moving house, or just deciding where to go on holiday!

### Moderating the Debate

Moderators must monitor the arguments and discussions for and against their resolutions and report any potential infringements of the platform terms & conditions to the platform administrator. 
Content owners will be alerted to any suspected infringment and can appeal to the System Administrator.
Coming early in 2026 will be an automated monitoring system which will make it easier to catch and remove dodgy content. 

## Creating the Arguments

As a debater, your role is to construct persuasive arguments, For or Against, to engage your opponents, and to vote thoughtfully. Follow these steps to excel:
Unsubscribe from these emails

### Understand the Debate Structure

Resolution: The debate’s central topic (e.g., “Artificial intelligence benefits society”). Moderators create resolutions; debaters argue For or Against. Sometimes known as the proposition or motion.
Framework: Usually supplied by the debate moderator to lay out the approach to the debate (e.g., ethical, economic, or social lens).
Argument Components:

- ***Claim***: A specific point supporting your side (e.g., “AI improves healthcare efficiency”).
- ***Warrant***: The reasoning behind your claim (e.g., “AI diagnostics reduce errors”).
- ***Evidence***: Credible data or sources (e.g., a study showing AI’s diagnostic accuracy).
- ***Impact Statement***: Why your claim matters to the resolution (e.g., “Better healthcare saves lives, supporting AI’s benefits”).
- ***Rebuttal***: Counterarguments to challenge opposing claims. May actually refute an argument, i.e. prove it wrong
- ***Turn***: A statement (with reasoning/warrant) that says an argument on one side, if true, actually supports the other side

### Joining a Debate
First, register for one of three roles:

***Moderator***: Creates debate resolutions and ensures content complies with platform rules.
***Debater***: Builds arguments (frameworks, claims, warrants, evidence, impact statements), posts rebuttals, creates discussion points, and votes on arguments with a rationale.
***Voter***: Votes and comments on the veracity of arguments but does not otherwise participate in the debate.

If you simply wish to follow what’s going on then you do not need to register and you will still be able to observe most of the debate content, but you will not have access to voting comments or be able to vote or contribute any arguments.[/li]

Once registered, browse open resolutions or use the search function to find topics of interest, choose a side (For or Against) and review existing arguments to understand the discussion. Then proceed below...

### Crafting Effective Arguments

***Understand the Framework*** (if defined by the moderator) and decide on your perspective (e.g., “I’ll argue from a public health standpoint”).
***Make Clear Claims***: If you wish to make a claim relating to the resolution, make sure it is specific and concise (e.g., “AI reduces diagnostic errors” rather than “AI is good”).
***Support with Warrants***: Explain why your claim is valid using logic or reasoning.
***Provide Evidence***: Use credible sources to back up your claim (e.g., academic studies, reputable news, or expert opinions). Cite sources clearly.
***Highlight Impacts***: Connect your argument to the resolution’s bigger picture.
***Keep It Civil***: Avoid inflammatory language or personal attacks to comply with platform rules.

### Posting Rebuttals and Discussion Points

- ***Rebuttal***: Directly challenge opposing arguments by questioning their claims, or warrants. Be specific (e.g., “The opponent’s study is outdated; newer data shows…”).
- ***Comments and Chat***: Use these to ask clarifying questions or highlight nuances without advancing your contention (e.g., “Can you clarify how AI impacts rural healthcare?”).
- Check your tone to ensure respectful engagement.

### Voting on Arguments

- ***Review arguments*** carefully before voting For or Against.
- Provide a ***short rationale*** (e.g., “I voted For because the evidence is recent and compelling”).
- ***Monitor notifications*** for updates to debates you’ve voted on. Reassess your vote if new arguments or evidence emerge.

### Managing Your Content

- Check your posts to see if others have rebutted or asked questions that you may wish to reply. Coming by the end of 2025 you can opt to receive automated alerts of this activity, but until then you should perform regular checks.
- Regularly check your posts to ensure they haven’t been flagged for violations. You should be also allerted by email
- If content is removed, review the moderation notice and use the appeals process if you believe it was removed unfairly.
- Avoid repeated violations to prevent account suspension.

## Assessing the Resolution Outcome
All votes are automatically aggregated upwards through the argument hierarchy, so that participants and viewers can see the level of support for and against each statement, taking into account the support for all supporting statements. Ultimately all votes are accumulated at the resolution level so which indicates the overall support for and against it. 
In a future release it will be possible to view the change in support of time for any resolution, but currently the platform shows the current level of support, in real-time as voting occurs.

## Tips for Success

- ***Research Thoroughly***: Use reliable sources to strengthen your evidence. Cross-check facts to avoid misinformation.
- ***Be Concise***: Clear, focused arguments are more persuasive than lengthy ones.
- ***Engage Respectfully***: Address ideas, not people. This keeps debates productive and compliant with rules.
- ***Stay Active***: Revisit debates to add new arguments or respond to rebuttals, as debates remain open for months.
- ***Learn from Others***: Read high-quality arguments from experienced debaters to improve your skills.
- ***Track Votes***: Monitor how your arguments are received to refine your approach.


## Common Pitfalls to Avoid

- ***Weak Evidence***: Relying on unverified or biased sources undermines your credibility.
- ***Ignoring Opponents***: Failing to address rebuttals weakens your position.
- ***Off-Topic Posts***: Stay focused on the resolution to avoid content removal.
- ***Overly Emotional Arguments***: Passion is great, but prioritize logic and evidence.
- ***Neglecting Notifications***: Missing updates may cause you to overlook new arguments that challenge your vote.
- ***Fallacy***: i.e. a statement that is based on invalid inference or reasoning. Either missing one that attacks your side, or getting caught using one can weaken your standing. Common types of fallacy include: Red Herring - where an argument is irrelevant to the debate and is used to distract or deflect, Post Hoc - assuming that sequence implies causation, Ad Hominem - attacking a debater rather than the arguments. If you spot a fallacy be sure rebut it so that others can also notice it. There are many more types of fallacy and a study of them (outside the scope of this Guide) will be very helpful to your debating skill.
 

## Example: Building an Argument

***Resolution***: “Remote work should be the standard for all industries.”
***Framework***: Economic and social benefits

*Side: For*

- ***Claim***: Remote work increases employee productivity.
- ***Warrant***: Flexible schedules allow workers to optimize their peak performance hours.
- ***Evidence***: A 2023 study by Stanford found a 13% productivity increase in remote workers.
- ***Impact***: Higher productivity boosts company profits and employee satisfaction, supporting remote work as a standard.
- ***Rebuttal (to opponent)***: The opponent claims remote work harms collaboration, but studies show virtual tools like Zoom maintain effective teamwork.

## Platform Etiquette and Compliance

- ***Follow Terms and Conditions***: Avoid hate speech, misinformation, or irrelevant content. All content is monitored for compliance with debate.report's Terms and Conditions. Violating content will be removed with the debater notified and directed to the appeals process. Repeated violations may lead to temporary or permanent account suspension.[/size]
- ***Appeal Respectfully***: If content is removed, use the appeals process calmly and provide evidence for your case.
- ***Stay Engaged***: Repeatedly ignoring notifications or posting low-effort content may flag your account as inactive or non-compliant.


# Conclusion

***debate.report*** offers a unique opportunity to hone your debating skills, engage with diverse perspectives, and contribute to meaningful discussions. As a new debater, focus on building clear, evidence-based arguments, engaging respectfully, and staying active in debates. By following this guide, you’ll develop confidence and make valuable contributions to the platform. Happy debating!

*Note*: For platform-specific issues or subscription details, contact our support team.
