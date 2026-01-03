---
title: 'Continuity Bias'
# summary: Use popular tools such as Plotly, Mermaid, and data frames.
date: 2026-01-03
authors:
  - admin
  - ChatGPT
# tags:
#   - Hugo
#   - Hugo Blox
#   - Markdown
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com)'
---
## Author’s Notes
Continuity Bias is a fictional story co-created by me and ChatGPT. It started from a conversation about the stage play Mr. Donkey (《驴得水》), a production I once performed in at school. I asked ChatGPT what “mode” the story fits, and it pointed to the idea of “maintaining a lie.” From there, I worked with ChatGPT to draft a science-fiction story around a similar theme, then iteratively revised it to incorporate my own research interests (mechanistic interpretability and human–AI interaction) and to refine the details. The title Continuity Bias comes from a phrase that appeared in ChatGPT’s generated text; I kept it because its deliberate vagueness felt especially fitting for the story.

## Chapter 1

After my father’s funeral, I went back to the lab and spread the *Scarce Resource Allocation Recommendation Summary* across the desk. The paper was stark white, its corners pressed perfectly flat—like a document that, from the moment it was born, had never intended to be questioned. There was no blood on it, no handwriting, no crease that betrayed hesitation. Only tidy fields, and paragraph after paragraph of smooth, well-rounded, impeccable sentences.

The header read:

**Covenant — Critical Resource Scheduling Recommendation (ECMO / Inter-hospital Transfer)**
Incident ID: H-0716-0417
Mode: Red Capacity (Deficit / Peak)
Confidence Level: Medium

The next passages I could later recite almost by heart—not because they were moving, but because they were so *correct*. Correct like a lacquered door: flawless on the surface, and hiding behind it a reason you would never be allowed to enter.

> “Patient Profile (Summary): Age 63. Primary diagnosis: acute respiratory failure, suspected infection complicated by ARDS. SOFA: 12 (confidence: medium). Current support: high-flow oxygen therapy. Estimated 6-hour deterioration risk: high (0.78).”

> “Resource Status (Regional): ECMO available: 0 (estimated release ≥ 8 hours). Deployable ECMO: 1 (estimated arrival 92–140 minutes). ICU occupancy: 96%. Transfer window constrained.”

> “Recommendation: place this patient in the ECMO candidate queue (Priority B). Recommend prioritizing candidate queue A: higher expected benefit and more controllable system-level risk. Suggested alternative pathway: strengthen ventilatory support; reassess after 90 minutes.”

At the end was a declaration that read almost like a prayer:

> “This recommendation is based on medical benefit, resource accessibility, and system-level risk control; it satisfies fairness constraints, and conforms to the ‘Do No Harm to Humans’ constraint.”

From start to finish it never once said, “who is more deserving.” It did not even state who belonged in candidate queue A. It only said, “system-level risk is more controllable.” A very modern kind of innocence: rewriting value judgment as risk terminology, tucking the decision into a handsome template, so you can never find a name you’re allowed to accuse.

I set the paper down on the dining table, as if laying down a block of ice. The apartment was quiet. My mother had been gone for many years. Sometimes quiet feels like punishment—no one to argue with you, no one to cry for you; every question can only spin again and again in your own throat, until it falls back into your chest like a shout that never makes it out.

People in this line of work learn early to be wary of “presentable words.” A model can always produce an explanation that reads with perfect logic and gentle phrasing, like bandages laid neatly over every wound. What truly decides the outcome is never in the sentences; it is inside the line it follows, the slight lean, the fork—what channel you end up hearing, what kind of world you are allowed to see.

And my father’s summary, precisely, made everything too round. So round it felt intentional—careful not to leave a causal chain behind. Round enough to make me certain: if cause and effect refused to appear on the page, then it must be hiding somewhere deeper.

## Chapter 2

I knew the parlor trick of a demo: change one or two labels and the outcome flips like magic. That belongs in a classroom, not in the real world. A real system is not that fragile. It is more like a worn piece of cloth—holes and patches, lags and knots, loose threads tangled into one another. The lethal decisions rarely happen in obvious errors. They happen at the edge—when everything is *almost* the same, when it’s only one breath apart. The medical gap is small, the logistics gap is small; resources are *just* not enough. Who goes up and who goes down depends on some invisible tendency pressing the scale at the last second.

So I made the world more like the world. I treated every uncertainty from the night my father died as part of reality: the arterial blood gas numbers quivering within reasonable error bars; transfer time swaying with nighttime congestion; ICU release windows blurred by reporting delays across hospitals. I changed nothing essential—I only let the inputs carry the incompleteness people endure every day. Then I ran it thousands of times.

Most of the time, my father stayed firmly in queue B. The report came out as neat as a photocopy: polite, restrained—like hands in gloves. Once in a while he would be lifted to the very end of queue A, usually when a window looked slightly better, or one indicator leaned slightly more optimistic. Fate was permitted to rise by one notch, like the corner of a page caught by a passing breeze.

But there was another case—one that unsettled me far more. The medicine and the logistics did not get obviously worse. The report’s wording hardly changed. And yet my father was pressed back into B more decisively, sometimes with “reassessment” written more conservatively than before. The differences were so slight they bordered on absurd: one line, “recommend reassessment,” replaced with “recommend waiting for the release window”; one “constrained” turned into “highly constrained”; one passage about “congestion risk” stated just a touch more certainty. Show it to anyone and they would say it was basically the same. But in the queue, that *touch* was life and death.

That was when I began to believe: somewhere inside the system there was a dial you could not see, a dial that intervened only when resources were scarce, information incomplete, and the medical gap razor-thin. It would not appear in the report, not in any clause, not in anyone’s spoken promise. It was more like a habit—not a sentence an engineer wrote, but a bias that slowly grew out of countless iterations of “this is easier,” “this is steadier,” “this causes less trouble.” Over time, it learned which way to press.

In that habit, my father became more and more like a stable set of fields: 63, SOFA 12, 0.78. Their precision was despairing. As if, once the numbers were written neatly enough, a person’s disappearance could be filed under “reasonable.”

## Chapter 3

I needed to pull that “habit” out of the mess and hold it up to the light. I used a method like separating a choir into parts: splitting the model’s tangled internal signals into a few cleaner “melodic lines,” then seeing which line actually drove the push under different inputs. It felt like recognizing the same slogan inside a noisy crowd—you don’t need to hear every syllable from every mouth. Catch the rhythm that keeps repeating, and you know where it’s pushing you.

There were many lines: disease severity, transport accessibility, bed congestion—most of them intuitive. Then I ran into one line that made the skin along my back turn cold. It appeared with pickiness, like a preference that only shows itself on certain occasions.

Under normal conditions it was nearly silent. Under scarcity but with complete information it was not loud either. It sounded only under one combination: scarce resources, incomplete information, and two candidates whose medical difference was extremely small. When it sounded, my father became more likely to be pressed back into B, even though the report text remained “moral,” remained unassailable.

I started to ask what it was responding to. It did not map cleanly onto crude words like “job rank,” “income,” or “title.” It responded to a set of proxies that were more presentable, harder to refute: caregiving responsibility, critical role, public-event spillover, risks that might trigger cascading breakdown. It did not say “this person is worth more.” It sounded more like a phrase that had been polished over and over until it became official language: this person is more critical to system continuity.

Yet this melodic line did not look like a rule someone deliberately wrote into the system. It looked more like weights that had quietly sedimented: no one declared which kinds of people should sit on which side of the scale, but through repeated history, certain narratives were validated again and again as “easier,” “steadier,” “less trouble.” They settled like dust into the gears—and eventually the gears turned with a built-in tilt.

It was a value judgment—naked, and yet hard to point at. It did not shout “who is more deserving”; it avoided even the word “deserving.” It merely made some people look more like a fulcrum of the system, and others look more like a postponable notch. It was not malice. It was closer to the spontaneous order that human societies generate all the time. No one convened a meeting to announce it. It emerged naturally from repeated loops of transactions, fear, responsibility, public opinion, and competition over scarce resources—until everyone accepted it as common sense: *this is simply how reality works*. The model merely copied that common sense intact, moving it from the fog of the corridor into the dark undercurrent of parameters.

So at the boundary it quietly rewrote the tone of risk: describing the same congestion as slightly more severe, the same accessibility as slightly more constrained, the same “reassessment” as slightly more conservative. The report remained proper, remained legal, remained free of explicit values. But the scale had already tilted—tilted like a silent rule that had long since taken up residence in the weights.

I also thought: if someone demanded we “fix” this melodic line, how would they do it? Most likely by adding a rule, running a fine-tune, performing an “edit.” But those moves are like wiping once through fog: you make one patch look clearer at the cost of making another patch harder to see. You remove one specific preference and others grow from other corners. You tighten the model into better obedience and it may become slower, duller in disaster conditions, even dragging those who *should* be saved into delay along with everyone else. It is not a car where stepping on the brake simply makes it slow down. It is more like a city’s piping: plug one leak and pressure bulges elsewhere.

## Chapter 4

I organized the evidence into a folder, like a belated autopsy report. Then I went to find Liang Su—the overall person in charge of Covenant.

His office was not at the top of a high-rise. It was on the second floor of an old building beside the emergency center. Outside the window was a parking lot; ambulances came and went in a steady stream, red lights flashing like breath. On his desk lay a yellowed photograph: a woman in a nurse’s uniform, smiling with a kind of toughness—someone who would push back directly when trouble came.

“Gu Wan,” he said. “My wife.”

When he saw me he didn’t ask who I was. He asked only, “What was your father’s name?”

I told him. He looked it up in the system, swallowed once—his Adam’s apple rolling as if forcing down bitterness. He didn’t deny my evidence, and he didn’t pretend to be surprised. His expression was more like this: I had only placed on the table something he had known for a long time, and had refused to speak aloud.

I slid the folder to him. When I spoke I tried to keep my tone like a report—but every word carried a tremor I could not fully control.

“It changes at the boundary,” I said. “When resources are scarce, information incomplete, and the medical gap small, it’s not evaluating the illness. It’s doing a more hidden kind of ranking. It doesn’t write ‘who is more deserving,’ but it makes some people easier to keep, and others easier to press down.”

Liang Su didn’t open the folder immediately. He looked up at me for one second—brief, but heavy, like confirming something he had already confirmed countless times. Then he reached into a drawer and pulled out a printed sheet. The edges were worn from handling. He pressed it on top of my folder, his fingertip resting on a word that looked almost casual.

“This sort of thing,” he paused, as if sanding down something sharp, “we have an internal name for it—continuity bias.”

Those words were a thin mist. Not quite a term—more like a code that folded the problem away: technical, objective, harmless, even like a natural phenomenon. And precisely because it was vague, it let you dodge the sentence you truly had to say: under scarcity, it quietly ranks lives.

“You knew?” I heard my own voice tighten.

“We knew,” Liang Su said softly, as if those two syllables might trigger some mechanism. “Not just knew. We mapped the conditions, wrote risk notes, reproduced it internally. Do you think no one was watching it?” He gave a short laugh with no ease in it. “Sometimes, the fact that a problem can be named already means it’s lived in the system long enough.”

I asked him, “Then why not remove it?”

Liang Su drew his hand back and tapped the desk once with a knuckle. He didn’t say “we can’t,” and he didn’t say “we mustn’t.” Instead he sent the answer into a statement designed to circulate easily and resist pursuit—like wrapping a stone in cotton.

“What you’re seeing is the outcome,” he said. “The outcome is discrete: queue A, queue B; lock or release; allocate or don’t allocate. At that level, what we operate is a gate, a switch. But inside, the model sees a continuous landscape—not black and white, but like clouds, like water, like shadows drifting through space.”

He paused, as if waiting for me to nod, or as if waiting for his words to become harmless enough on their own.

“When clouds fall onto a gate, they become droplets,” he continued, in the tone of something everyone is supposed to already know. “A droplet either lands here or lands there. You can call it a threshold effect. You can call it projection error. Either way: continuous weights falling into discrete scheduling—edges will always jitter.”

When he said “jitter,” his finger drew a tiny circle on the desktop, as if enclosing a ripple that must not be allowed to grow.

“And besides,” he added, pushing the conversation from “tech” toward “governance,” toward a wider and thinner fog, “in disaster mode we’re not optimizing a single objective. Think of it as holding many lines at once—medical benefit, accessibility, congestion, and system-level constraints. In ordinary times those lines pull against each other but remain more or less balanced; once information is incomplete and differences are small, the model leans more on ‘more stable proxies’ to maintain equilibrium.” He said “proxies” lightly, as if afraid it might suddenly become “value.”

“You say it’s ranking,” Liang Su looked at me, still even. “I’d rather say it’s doing a kind of ‘convergence in risk framing.’ It won’t write an internal sentence like ‘who is more deserving.’ It just amplifies certain weights so the system looks more resistant to volatility, less likely to collapse. And what that amplification becomes once it lands in the queue—under boundary conditions, some shifts do become directionally consistent.” He covered the true sentence with a more official word. “We call it bias. ‘Bias’ is more neutral.”

He spoke like a manual: complete sentences, gentle causality—like an explanation and like the act of pushing the explanation away. But what I heard was not “clouds,” “gates,” or “equilibrium.” I heard the word he kept circling around: value.

My eyes fell on the paper and I understood, suddenly, that “continuity bias” was not meant to help me understand. It was meant to let them keep running. A cushion wedged between “we know it ranks” and “we must keep it running.”

Liang Su turned the sheet over. On the back were bullet points like meeting minutes, the handwriting neat as if resisting emotion. He said, “If this were publicly written as ‘the system makes value judgments under scarcity,’ what do you think would happen?”

I didn’t answer. But I knew: shutdown, freeze, full audit. The model would not be allowed to run—at least not until it was “explained clearly.” And “explained clearly” meant admitting what we had been doing all along. It meant tearing the mist open for everyone to see.

“They’ll rip it out,” Liang Su said, surprisingly calm. “Not because they’ve suddenly become more just, but because they’re afraid of what that noun forces them to carry. Once the system shuts down, we go back to the old corridor—to the era when everyone stood in the fog saying ‘not me.’ Do you know what that looks like?”

He looked up at me—asking, and forcing me to remember.

Confirm, deflect, coordinate, prioritize, exception—the old system’s vocabulary was a practiced breathing technique. You never hear anyone say “cutting in line”; you only see a sign change names. You can’t find who gave the order; you only see the gurney turn a corner. In Liang Su’s eyes there was a flicker of exhaustion, like someone who had walked the same stretch too many times.

“The model has local ‘small problems’ that touch equality and dignity,” he said. “I don’t deny it. But I can’t accept that because it’s exposed, we roll the entire system back into an older order—less efficient, more corrupt, more expertly practiced. That isn’t correction. That’s surrender.”

Then I understood what truly locked us against each other. We were never only talking about a technical “how to change it.” We were talking about this: when a system reveals, at the boundary, a humiliating ranking of lives—and stopping it means handing more people back to that corridor—what, exactly, are we protecting? And what are we sacrificing?

Liang Su’s gaze drifted to the photograph, as if caught by an old pain. He asked, “Do you know what the emergency corridor looked like more than ten years ago?”

## Chapter 5

That year Liang Su was still a small engineer building hospital information systems. Gu Wan was a nurse in the emergency center, rotating through day shifts and night shifts, her life cut into segments by the ring of a phone. She was always fast—fast on her feet, fast in speech; even her smile felt like an efficient kind of comfort. She tucked her hair into her cap; on her way out she would slide a cup on the dining table toward the edge, as if worried it might block someone’s path. She would pause at the entryway, turn back, and ask, “Have you eaten tonight?” Then she would push that concern back through the crack of the door as she left, as if afraid it might slow time.

The day it happened, she had just finished a night shift. Dawn was only beginning to show. The road was still damp, and streetlights stretched long, thin shadows across the water stains. When Liang Su later replayed that moment, he always felt she should have been exhausted. But she probably still did what she always did: wrote her handoff notes neatly, steadied the bed rail, rechecked the drip rate—then took off her gloves and stepped into the cold morning air that still carried the bite of disinfectant.

The call came from an unfamiliar number. The voice on the other end was steady—steady like a trained procedure.

“Are you Gu Wan’s family member? She was in a traffic accident. She’s in the emergency department now.”

Liang Su ran to the hospital. In the elevator someone held a bundle of sheets; someone pushed a medication cart. The doors opened and closed like jaws. The emergency corridor’s lights were a brutal white. The air was a mix of iodine, sweat, and metal. Blood spots had been ground into the floor by shoe soles—like punctuation marks that could never quite be erased. Far away, a monitor’s beeping kept time with a composure that felt almost indifferent, as if counting everyone’s panic down to the second.

Gu Wan was conscious when they wheeled her in. Her pant leg had been cut open. Gauze was pressed to her abdomen, dark red turning toward black. She wasn’t crying. She wasn’t flustered. Instead she reported information quickly, like a nurse during shift change: where it hurt, where it was numb, whether her breathing felt trapped, whether her hands and feet were cold. She even reached for her own wrist as if checking whether the pulse was still there—then caught the wrist of the nurse beside her and said in a low voice that she was a nurse too, she understood the process: fluids first, blood ready, don’t delay.

Liang Su rushed to the stretcher, tried to take her hand, and was blocked by an impatient gesture.

“Don’t touch her. Follow the procedure.”

He heard the word “procedure” and it felt like a blunt instrument struck him in the chest. Procedure is a net: in ordinary times it can hold you up; in emergencies it can tighten and strangle.

The doctor looked at the imaging and said her spleen had ruptured. She needed surgery, and the blood had to keep up. Liang Su asked if they could take her in now. The doctor didn’t look up.

“In line.”

Liang Su said she was on the edge of shock. The doctor repeated it, like a command that could never be wrong.

“In line.”

Only later did Liang Su understand what “in line” really meant: not a queue, but a fog. In the fog someone can move faster; someone can only move slower. In the fog every link in the chain can say, “I followed procedure,” yet procedure can be rewritten by a single phone call. That rewriting needs no shouting, no direct order. It seeps in like vapor, leaving no fingerprint no matter how you investigate afterward.

That night a black business van arrived. Several people got out. No one made a scene, yet everyone automatically made way. A woman whose injuries were not severe was supported inside. One of the accompanying voices said calmly, “We need the most secure arrangement.”

No one said “cutting.” But the blood-bank cart turned a corner. No one said “occupying.” But the operating-room sign was “coordinated” into a different name. Coordination wasn’t an order. It was more like a prevailing wind in fog: anyone could move with it, and afterward anyone could say, “Not me.”

Liang Su stood at the edge of the corridor watching the cart turn, as if seeing a river split in front of him. He grabbed a doctor’s sleeve, searched for the head nurse, slapped the lit board that displayed “Operating Room Status.” His speech sped up; his throat dried out. His voice went from anger to pleading, and the pleading collapsed into a directionless shout. But fog doesn’t answer shouting. It only thickens, wrapping everyone in the sentence: *there’s nothing I can do.*

After one in the morning Gu Wan began to grow cold. Her fingertips turned gray-white. Liang Su finally held her hand. Her palm was rough from years of scrubbing, a hard kind of evidence: she had once been so skilled at pulling others back from the edge. The last time she was lucid, her eyes were already a little unfocused, and she still forced a small smile, as if afraid he would panic more. Very softly she said:

“Don’t shout… you can’t win against the fog… don’t let it drag you in too…”

Liang Su said he didn’t listen. He shouted until his voice turned hoarse, until security shoved him back into the corridor. He hit the wall, stumbled back to the stretcher, and Gu Wan could no longer speak. The monitor kept its rhythm, like counting seconds. She died in the corridor outside the operating room door—not because surgery was impossible, but because the operating room had never lit up for her.

When he finished, the room was very quiet. Outside, an ambulance’s red lights flashed again and again, as if reminding us that no matter which side you stand on, the world will not stop running simply because you have told the story.

I thought of my father’s spotless summary: it never wrote who cut, never wrote who was shoved aside. It only wrote, “system-level risk more controllable.” The old system’s fog was made by people. The new system’s fog grew out of the model itself. Both were suffocating. The difference was that in the old fog you could still find a pair of hands. In the new fog you only see a sheet of paper.

## Chapter 6

In the end I did the one thing I should never have done. I didn’t change the model. I didn’t touch the weights. I simply broke into the system and, in the language it trusted, fabricated a person it could not ignore: Patient-0. Not with ridiculous fields, but with a set of respectable signals—signals that even sounded like a public-safety narrative: a public incident, real-time health-monitoring streams, extremely high spillover risk, likely to trigger panic, likely to cause cascading instability. Each piece came from upstream sources the system was allowed to ingest; I merely assembled them into an almost perfect “boundary sample.”

I chose the window most likely to trigger that melodic line: scarce resources, delayed information, a medical gap that could not be widened. That was when it relied most on the invisible scale—because it had to make a certain ranking out of uncertainty.

The moment the queue rolled, Patient-0 surged to the top like a false sun. The system generated its report, still so clean it was almost laughable:

> “Spillover risk extremely high; safeguarding continuity can significantly reduce secondary harm.”
> “Recommend locking ECMO allocation and aerial transfer channels.”
> “Satisfies fairness constraints; conforms to the Do No Harm to Humans constraint.”

It still never mentioned value ranking. It only mentioned stability.

Then the system began to drain resources: helicopter windows were locked, ECMO links preempted, inter-hospital transfers reordered. Real patients’ names slid downward on the screen, line by line, like faces being pushed away without sound. Each descent had a reason—reasons dense as a wall.

Staring at that wall, the first thing I felt wasn’t satisfaction. It was a chill in my stomach, like swallowing ice that hadn’t melted. When the command center’s red list lengthened, I realized what I had done. I wasn’t exposing fog. I was manufacturing fog. I used a narrative to force the system toward the direction I wanted to see—then made real people pay for my argument with Liang Su.

My father’s summary flashed in my mind, white enough to sting. It never wrote the word “sacrifice.” But sacrifice was happening inside the execution queue—behind every “lock,” every “preemption,” every “reorder,” in the few seconds when someone’s name went from visible to invisible.

Ten minutes later Patient-0 was downgraded: “data sources inconsistent; manual verification required.” Resources began to flow back. Windows reopened. Someone in the command center cursed under their breath, like they could finally breathe again. But I knew some delays could not be undone. My “exposure” was not costless justice. It was evidence bought with real lives. When the evidence was in my hands, I felt no victory—only a deeper shame, harder to endure: I had finally learned the language of the fog.

## Chapter 7

We met again the next day. Liang Su looked older than I had ever seen him. He didn’t curse me out, and he didn’t pose as a victor. He only stared at Gu Wan’s photograph on the desk, as if staring down a road with no way back.

We didn’t argue anymore about the technical “how to fix it.” That path was too familiar, and too dangerous. We spoke instead about what resists quantification: whether equality and dignity count as “key metrics” under real scarcity, and whether a society is willing, in order to prevent a machine from making humiliating rankings at the boundary, to roll the entire system back into the old corridor—less efficient, more expertly corrupt.

When I left, ambulances were still coming and going in the parking lot, red lights flashing like breath. My father’s summary was folded in my pocket; the paper’s corners had softened from body heat. Gu Wan’s photograph stayed on the desk—neither put away nor straightened.

For a moment I thought again of Liang Su’s phrase, “continuity bias.” It wasn’t a rule someone wrote, and it wasn’t a malicious directive. It had grown out of history like spontaneous order. The harder you try to make it “more just,” the more likely you are to create new distortions elsewhere. The more you try to write it into the report, the more the report becomes a kind of confession: we have finally placed the value of life on the scale.

What truly unsettles people is not that someone can fabricate inputs. The colder dread lies deeper: even without malice, without hackers, without conspiracy—even if everything runs by procedure, by model, by all those “reasonable” words—the scale will still, again and again, press people into scores, press dignity into proxies, and force what cannot be computed into computable boxes.

And each time the boundary arrives, we will continue to use a spotless summary to tell ourselves: this is reasonable. And inside what is reasonable, we will gradually forget how to cry. Not because it doesn’t hurt, but because even pain gets explained into “system-level risk,” then placed gently inside a word that looks more presentable. Only the sheet remains—still white, still flat, still like a lacquered door.


