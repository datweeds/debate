# Debate Chamber Overview
??? warning "Support Notice"
    The **User Guide** is currently undergoing major re-construction, which we are aiming to complete by the end of April 2026. In the meantime please email [support@debate.report](mailto:support@debate.report)

    Thank you for your patience, and your ongoing interest in **debate.report**. We are aiming to build a world-class debate platform, and to encourage many more people to engage in meaningful debate. The platform essentially turns debating into a fun and enjoyable game for the participants, and which helps participants and the audience alike to develop and sharpen their critical-thinking skills and to come to an informed position on the important issues of the day. 

    the Debate Report Team, March 2026

---

## Introduction to Debating

Welcome to debate.report, an online platform for structured, asynchronous debates on diverse topics. This guide is designed for new debaters to help you navigate the platform, understand the roles in the debating process, and to help you build effective arguments and have your voice heard. Whether you're new to debating or transitioning to online formats, this guide will equip you with the essentials to participate confidently.

### Why Debate?
Debating hones critical thinking, forces you to see both sides, and teaches you to articulate ideas —skills that cut through the noise of our info-saturated world. In politics, law, or even online arguments, it’s a tool for reasoning and persuasion. Plus, it’s a democratic cornerstone: societies need to debate openly to engender trust and commitment. In 2025, with polarized discourse and AI stirring the pot, debating’s role in fostering clarity and mutual understanding is more crucial than ever.

### Who Should Debate?
The short answer is – everyone! In truth though, it takes time and attention to follow and digest argument reasoning, evaluate the evidence, and consider opions. So not everyone can participate in all debates. So, choose your battles wisely and argue for what matters most to you. These are the debates you will research and consider carefully. For the other topics, you can at least read the summaries and vote on the arguments, based on what understanding you glean from them. 

### Are my Contributions Private or Public?
Presently all debating is conducted in private and all contributions and votes are anonymous. In a future release you will be able to opt-in to make your contributions public, meaning others will be able to associate your profile with your contributions and voting. This ‘public profile’ feature is expected early 2026.

## The Debating Process
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

Note - a discussion point can be posted against any type of statement although the lines are not represented on the diagram to allow the other lines of association to be clearer.

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
an assertion made by a debater, stating a belief or position (that needs to be supported by evidence)

### Rebuttal
response to an opponent's argument, where a debater either disagrees or refutes a claim, warrant or impact, often by providing counter-evidence or demonstrating flaws to the logic

### Tur
an argument that reverses the meaning or effect of an opponent's argument, showing that their point actually supports the opposing side 

### Impac
the consequence or significance of the argument, quantifying or evaluating how the outcome affects people or society, and explaining why the argument matters.

### Evidence
serves as the support for the warrant, taking the form of statistics, specific examples, testimony, or expert opinion, and is used to compel the audience to accept the reason

### Warrant - provides the logical reason or justification for why the statement is true, explaining the connection between the statement and the evidence  



