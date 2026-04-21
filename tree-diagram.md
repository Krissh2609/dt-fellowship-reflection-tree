# Reflection Tree — Visual Diagram

```mermaid
flowchart TD
    START([START\nGood evening...]) --> A1_OPEN

    A1_OPEN[/"Q: Today's weather report?"\nSunny/Cloudy/Stormy/Foggy/]
    A1_OPEN -->|Sunny/Cloudy| A1_Q1_HIGH
    A1_OPEN -->|Stormy/Foggy| A1_Q1_LOW

    A1_Q1_HIGH[/"Q: When something went well,\nwhat made it happen?"/]
    A1_Q1_HIGH -->|Prepared/Adjusted| A1_Q2_AGENCY
    A1_Q1_HIGH -->|Helped/Lucky| A1_Q2_LUCK

    A1_Q1_LOW[/"Q: When things got difficult,\nwhere did your mind go?"/]
    A1_Q1_LOW -->|Looked for control| A1_Q2_AGENCY
    A1_Q1_LOW -->|Stuck/Blamed/Wondered| A1_Q2_STUCK

    A1_Q2_AGENCY[/"Q: When things didn't go\nas planned, what did you do?"/]
    A1_Q2_AGENCY --> A1_R_INT

    A1_Q2_STUCK[/"Q: Was there a moment where\nyou had a choice?"/]
    A1_Q2_STUCK -->|Yes - made call/didn't act/looking back| A1_R_EXT_GROW
    A1_Q2_STUCK -->|Not sure I saw any| A1_R_EXT_STUCK

    A1_Q2_LUCK[/"Q: Something you did\nthat helped today?"/]
    A1_Q2_LUCK -->|Energy/Clear/Patient| A1_R_INT
    A1_Q2_LUCK -->|Not sure| A1_R_EXT_GROW

    A1_R_INT(["REFLECT:\nYou stayed in the driver's seat"])
    A1_R_EXT_GROW(["REFLECT:\nYou just noticed there was\na choice somewhere in there"])
    A1_R_EXT_STUCK(["REFLECT:\nWas there one moment where\nyour response was yours to choose?"])

    A1_R_INT --> BRIDGE_1_2
    A1_R_EXT_GROW --> BRIDGE_1_2
    A1_R_EXT_STUCK --> BRIDGE_1_2

    BRIDGE_1_2{{"BRIDGE: Now let's shift\nfrom how you handled it\n— to what you gave"}}
    BRIDGE_1_2 --> A2_OPEN

    A2_OPEN[/"Q: In one interaction today,\nwhich felt more true?"/]
    A2_OPEN -->|Could offer| A2_Q1_CONTRIB
    A2_OPEN -->|Would get/Autopilot| A2_Q1_ENT
    A2_OPEN -->|Getting through it| A2_Q1_NEUTRAL

    A2_Q1_CONTRIB[/"Q: Did you do something\nbeyond what was expected?"/]
    A2_Q1_CONTRIB -->|Helped/Extra effort| A2_Q2_CONTRIB_DEEP
    A2_Q1_CONTRIB -->|Sort of/Wanted to| A2_Q2_CONTRIB_SOFT

    A2_Q1_ENT[/"Q: Did you feel you deserved\nmore than you received?"/]
    A2_Q1_ENT -->|Yes, bothered/let go| A2_Q2_ENT
    A2_Q1_ENT -->|Briefly/No| A2_Q2_CONTRIB_SOFT

    A2_Q1_NEUTRAL[/"Q: Who else was\nin the room with you?"/]
    A2_Q1_NEUTRAL -->|Colleague/Customer| A2_Q2_CONTRIB_DEEP
    A2_Q1_NEUTRAL -->|Manager/Alone| A2_Q2_CONTRIB_SOFT

    A2_Q2_CONTRIB_DEEP[/"Q: What was driving\nthe extra effort?"/]
    A2_Q2_CONTRIB_DEEP -->|Wanted to/Right thing| A2_R_CONTRIB
    A2_Q2_CONTRIB_DEEP -->|Hoped noticed/Unsure| A2_R_MIXED

    A2_Q2_CONTRIB_SOFT[/"Q: Something you could have\ndone but didn't?"/]
    A2_Q2_CONTRIB_SOFT -->|Stretched/Did act| A2_R_CONTRIB
    A2_Q2_CONTRIB_SOFT -->|Noticed/Didn't notice| A2_R_MIXED

    A2_Q2_ENT[/"Q: Did someone else give\nmore than they received?"/]
    A2_Q2_ENT -->|Yes/Probably| A2_R_ENT_GROW
    A2_Q2_ENT -->|Maybe/No| A2_R_ENT

    A2_R_CONTRIB(["REFLECT:\nYou gave without keeping score"])
    A2_R_MIXED(["REFLECT:\nA lean toward giving"])
    A2_R_ENT_GROW(["REFLECT:\nYou noticed someone else's contribution"])
    A2_R_ENT(["REFLECT:\nLead with one action\nbefore you start counting"])

    A2_R_CONTRIB --> BRIDGE_2_3
    A2_R_MIXED --> BRIDGE_2_3
    A2_R_ENT_GROW --> BRIDGE_2_3
    A2_R_ENT --> BRIDGE_2_3

    BRIDGE_2_3{{"BRIDGE: One last shift.\nFrom what you gave\n— to who you saw"}}
    BRIDGE_2_3 --> A3_OPEN

    A3_OPEN[/"Q: Whose experience comes\nto mind besides your own?"/]
    A3_OPEN -->|No one - about me| A3_Q1_SELF
    A3_OPEN -->|Specific colleague| A3_Q1_COLLEAGUE
    A3_OPEN -->|Team/Customer| A3_Q1_WIDE

    A3_Q1_SELF[/"Q: Was there anyone who\nhad a harder time?"/]
    A3_Q1_SELF -->|Yes/Maybe/No bandwidth| A3_Q2_SELF_GROW
    A3_Q1_SELF -->|Everyone fine| A3_Q2_SELF

    A3_Q1_COLLEAGUE[/"Q: Did you do anything\nwith that awareness?"/]
    A3_Q1_COLLEAGUE -->|Checked in/Helped| A3_Q2_ALTRO
    A3_Q1_COLLEAGUE -->|Noticed, didn't act| A3_Q2_COLLEAGUE_PASSIVE

    A3_Q1_WIDE[/"Q: Was your work connected\nto something that matters to them?"/]
    A3_Q1_WIDE -->|Direct line| A3_Q2_ALTRO
    A3_Q1_WIDE -->|Fuzzy/Not directly| A3_Q2_WIDE_SOFT

    A3_Q2_SELF[/"Q: What does success\nlook like for you?"/]
    A3_Q2_SELF -->|My job/Career| A3_R_SELF
    A3_Q2_SELF -->|Team/People/Larger| A3_R_GROW

    A3_Q2_SELF_GROW[/"Q: If you'd noticed earlier,\nwhat might you have done?"/]
    A3_Q2_SELF_GROW -->|Asked/Shared| A3_R_GROW
    A3_Q2_SELF_GROW -->|Helped| A3_R_ALTRO
    A3_Q2_SELF_GROW -->|Not my place| A3_R_SELF

    A3_Q2_ALTRO[/"Q: When you act beyond your\nown interests, what makes it worth it?"/]
    A3_Q2_ALTRO --> A3_R_ALTRO

    A3_Q2_COLLEAGUE_PASSIVE[/"Q: What usually stops you\nfrom reaching out?"/]
    A3_Q2_COLLEAGUE_PASSIVE -->|Fear/Assumed/Habit| A3_R_GROW
    A3_Q2_COLLEAGUE_PASSIVE -->|Time| A3_R_SELF

    A3_Q2_WIDE_SOFT[/"Q: What would you want them\nto feel about your work?"/]
    A3_Q2_WIDE_SOFT -->|Thinking of them/Care/Forward| A3_R_ALTRO
    A3_Q2_WIDE_SOFT -->|Hadn't thought about it| A3_R_GROW

    A3_R_SELF(["REFLECT:\nSelf-transcendence —\nworth a thought for tomorrow"])
    A3_R_GROW(["REFLECT:\nYou're starting to see\npast your own frame"])
    A3_R_ALTRO(["REFLECT:\nYou operated with\na wide radius today"])

    A3_R_SELF --> SUMMARY
    A3_R_GROW --> SUMMARY
    A3_R_ALTRO --> SUMMARY

    SUMMARY[["SUMMARY\nAxis I: {dominant}\nAxis II: {dominant}\nAxis III: {dominant}"]]
    SUMMARY --> END([END\nSee you tomorrow.])

    %% Styling
    classDef question fill:#f5f0e8,stroke:#c4622d,stroke-width:1.5px,color:#1a1814
    classDef reflection fill:#e8f0ec,stroke:#3d6b4f,stroke-width:1.5px,color:#1a1814
    classDef bridge fill:#ece3f5,stroke:#4a2d7a,stroke-width:1.5px,color:#1a1814,font-style:italic
    classDef terminal fill:#1a1814,stroke:#1a1814,color:#f5f0e8
    classDef summary fill:#e3eaf5,stroke:#2d4a7a,stroke-width:2px,color:#1a1814

    class A1_OPEN,A1_Q1_HIGH,A1_Q1_LOW,A1_Q2_AGENCY,A1_Q2_STUCK,A1_Q2_LUCK question
    class A2_OPEN,A2_Q1_CONTRIB,A2_Q1_ENT,A2_Q1_NEUTRAL,A2_Q2_CONTRIB_DEEP,A2_Q2_CONTRIB_SOFT,A2_Q2_ENT question
    class A3_OPEN,A3_Q1_SELF,A3_Q1_COLLEAGUE,A3_Q1_WIDE,A3_Q2_SELF,A3_Q2_SELF_GROW,A3_Q2_ALTRO,A3_Q2_COLLEAGUE_PASSIVE,A3_Q2_WIDE_SOFT question
    class A1_R_INT,A1_R_EXT_GROW,A1_R_EXT_STUCK reflection
    class A2_R_CONTRIB,A2_R_MIXED,A2_R_ENT_GROW,A2_R_ENT reflection
    class A3_R_SELF,A3_R_GROW,A3_R_ALTRO reflection
    class BRIDGE_1_2,BRIDGE_2_3 bridge
    class START,END terminal
    class SUMMARY summary
```

## Path Count

The tree produces **24+ distinct conversation paths** depending on answers. Below are the two extreme paths:

### Path A — "Victim / Entitled / Self" (Persona 1)
`START → A1_OPEN(Stormy) → A1_Q1_LOW → A1_Q2_STUCK → A1_R_EXT_STUCK → A2_OPEN(get) → A2_Q1_ENT → A2_Q2_ENT → A2_R_ENT → A3_OPEN(about me) → A3_Q1_SELF → A3_Q2_SELF → A3_R_SELF → SUMMARY → END`

### Path B — "Victor / Contributing / Altrocentric" (Persona 2)
`START → A1_OPEN(Cloudy) → A1_Q1_HIGH → A1_Q2_AGENCY → A1_R_INT → A2_OPEN(offer) → A2_Q1_CONTRIB → A2_Q2_CONTRIB_DEEP → A2_R_CONTRIB → A3_OPEN(colleague) → A3_Q1_COLLEAGUE → A3_Q2_ALTRO → A3_R_ALTRO → SUMMARY → END`
