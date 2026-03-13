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

    class Resolution {
        Formal statement setting the debate topic
    }

    class Framework {
        Principles or standards for evaluation
    }

    class Claim {
        Assertion of belief or position
    }

    class Rebuttal {
        Response refuting opponent's point
    }

    class Turn {
        Argument reversing opponent's point
    }

    class Impact {
        Consequence or significance of argument
    }

    class Warrant {
        Logical justification linking evidence to claim
    }

    class Evidence {
        Statistics, examples, testimony
    }

    Resolution     "1"   -->   "1"     Framework          : "evaluated using"
    Resolution     "1"   -->   "1..*"  Claim              : "supported/denied by"

    Claim          "1"   -->   "0..1"  Impact
    Claim          "1"   -->   "0..1"  Turn
    Claim          "1"   -->   "0..1"  Warrant            : "justifies or proves"
    Claim          "1"   -->   "0..1"  Rebuttal           : "can be rebutted"

    Turn           "1"   -->   "0..1"  Claim
    Turn           "1"   -->   "0..1"  Impact             : "turns"

    Impact         "1"   ..>   "0..1"  Turn               : "impacts"

    Rebuttal       "1"   -->   "0..1"  Turn
    Rebuttal       "1"   -->   "0..1"  Claim
    Rebuttal       "1"   -->   "0..1"  Impact
    Rebuttal       "1"   -->   "0..1"  Warrant

    Warrant        "1"   -->   "0..1"  Claim              : "justifies or proves"
    Warrant        "1"   -->   "0..1"  Rebuttal           : "justifies or proves"

    Evidence       "*"   -->   "0..*"  Warrant            : "supports"

    note for Claim "Direction: Pro / Con (supports / denies Resolution)"
    ```
    </details>

### Title Feature Notes
Text
Additional paragraphs go here, also indented by 4 spaces.
    
 ### Text 2
<details>
    <summary>Collapsible Tech Section</summary>
    More technical content here (native HTML, no styling needed).
    
    ```mermaid
    ---
    title: Template Flow Diagram
    ---
    flowchart TD
        A[User opens Voting Box] --> B{Debate active?}
        B -->|Yes| C[Click 'New Vote']
        B -->|No| D[Error: Debate closed]
        C --> E[Enter proposal details]
        E --> F[Set options & duration]
        F --> G[Submit]
        G --> H[Vote listed & votable]
        style A fill:#C91616,stroke:#333
        style H fill:#C91616,stroke:#333
    ```
    </details>

=== "[ TECHNICAL NOTES ]"
    ### Title Technical Notes
    Text

