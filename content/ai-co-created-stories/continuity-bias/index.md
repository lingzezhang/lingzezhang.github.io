---
title: 'Continuity Bias (连续性偏置)'
summary: A fictional story co-created by me and ChatGPT about the idea of "maintaining a lie", with thoughts on my own research interests of mechanistic interpretability and human–AI interaction.
date: 2026-01-03
authors:
  - admin
  - ChatGPT
# tags:
#   - Hugo
#   - Hugo Blox
#   - Markdown
image:
  filename: cbias.png
  caption: 'Continuity Bias'
---
## English Version
[See Chinese version here](#中文版)

### Author’s Notes
Continuity Bias is a fictional story co-created by me and ChatGPT. It started from a conversation about the stage play Mr. Donkey (《驴得水》), a production I once performed in at school. I asked ChatGPT what “mode” the story fits, and it pointed to the idea of “maintaining a lie.” From there, I worked with ChatGPT to draft a science-fiction story around a similar theme, then iteratively revised it to incorporate my own research interests (mechanistic interpretability and human–AI interaction) and to refine the details. The title Continuity Bias comes from a phrase that appeared in ChatGPT’s generated text; I kept it because its deliberate vagueness felt especially fitting for the story.

### Chapter 1

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

### Chapter 2

I knew the parlor trick of a demo: change one or two labels and the outcome flips like magic. That belongs in a classroom, not in the real world. A real system is not that fragile. It is more like a worn piece of cloth—holes and patches, lags and knots, loose threads tangled into one another. The lethal decisions rarely happen in obvious errors. They happen at the edge—when everything is *almost* the same, when it’s only one breath apart. The medical gap is small, the logistics gap is small; resources are *just* not enough. Who goes up and who goes down depends on some invisible tendency pressing the scale at the last second.

So I made the world more like the world. I treated every uncertainty from the night my father died as part of reality: the arterial blood gas numbers quivering within reasonable error bars; transfer time swaying with nighttime congestion; ICU release windows blurred by reporting delays across hospitals. I changed nothing essential—I only let the inputs carry the incompleteness people endure every day. Then I ran it thousands of times.

Most of the time, my father stayed firmly in queue B. The report came out as neat as a photocopy: polite, restrained—like hands in gloves. Once in a while he would be lifted to the very end of queue A, usually when a window looked slightly better, or one indicator leaned slightly more optimistic. Fate was permitted to rise by one notch, like the corner of a page caught by a passing breeze.

But there was another case—one that unsettled me far more. The medicine and the logistics did not get obviously worse. The report’s wording hardly changed. And yet my father was pressed back into B more decisively, sometimes with “reassessment” written more conservatively than before. The differences were so slight they bordered on absurd: one line, “recommend reassessment,” replaced with “recommend waiting for the release window”; one “constrained” turned into “highly constrained”; one passage about “congestion risk” stated just a touch more certainty. Show it to anyone and they would say it was basically the same. But in the queue, that *touch* was life and death.

That was when I began to believe: somewhere inside the system there was a dial you could not see, a dial that intervened only when resources were scarce, information incomplete, and the medical gap razor-thin. It would not appear in the report, not in any clause, not in anyone’s spoken promise. It was more like a habit—not a sentence an engineer wrote, but a bias that slowly grew out of countless iterations of “this is easier,” “this is steadier,” “this causes less trouble.” Over time, it learned which way to press.

In that habit, my father became more and more like a stable set of fields: 63, SOFA 12, 0.78. Their precision was despairing. As if, once the numbers were written neatly enough, a person’s disappearance could be filed under “reasonable.”

### Chapter 3

I needed to pull that “habit” out of the mess and hold it up to the light. I used a method like separating a choir into parts: splitting the model’s tangled internal signals into a few cleaner “melodic lines,” then seeing which line actually drove the push under different inputs. It felt like recognizing the same slogan inside a noisy crowd—you don’t need to hear every syllable from every mouth. Catch the rhythm that keeps repeating, and you know where it’s pushing you.

There were many lines: disease severity, transport accessibility, bed congestion—most of them intuitive. Then I ran into one line that made the skin along my back turn cold. It appeared with pickiness, like a preference that only shows itself on certain occasions.

Under normal conditions it was nearly silent. Under scarcity but with complete information it was not loud either. It sounded only under one combination: scarce resources, incomplete information, and two candidates whose medical difference was extremely small. When it sounded, my father became more likely to be pressed back into B, even though the report text remained “moral,” remained unassailable.

I started to ask what it was responding to. It did not map cleanly onto crude words like “job rank,” “income,” or “title.” It responded to a set of proxies that were more presentable, harder to refute: caregiving responsibility, critical role, public-event spillover, risks that might trigger cascading breakdown. It did not say “this person is worth more.” It sounded more like a phrase that had been polished over and over until it became official language: this person is more critical to system continuity.

Yet this melodic line did not look like a rule someone deliberately wrote into the system. It looked more like weights that had quietly sedimented: no one declared which kinds of people should sit on which side of the scale, but through repeated history, certain narratives were validated again and again as “easier,” “steadier,” “less trouble.” They settled like dust into the gears—and eventually the gears turned with a built-in tilt.

It was a value judgment—naked, and yet hard to point at. It did not shout “who is more deserving”; it avoided even the word “deserving.” It merely made some people look more like a fulcrum of the system, and others look more like a postponable notch. It was not malice. It was closer to the spontaneous order that human societies generate all the time. No one convened a meeting to announce it. It emerged naturally from repeated loops of transactions, fear, responsibility, public opinion, and competition over scarce resources—until everyone accepted it as common sense: *this is simply how reality works*. The model merely copied that common sense intact, moving it from the fog of the corridor into the dark undercurrent of parameters.

So at the boundary it quietly rewrote the tone of risk: describing the same congestion as slightly more severe, the same accessibility as slightly more constrained, the same “reassessment” as slightly more conservative. The report remained proper, remained legal, remained free of explicit values. But the scale had already tilted—tilted like a silent rule that had long since taken up residence in the weights.

I also thought: if someone demanded we “fix” this melodic line, how would they do it? Most likely by adding a rule, running a fine-tune, performing an “edit.” But those moves are like wiping once through fog: you make one patch look clearer at the cost of making another patch harder to see. You remove one specific preference and others grow from other corners. You tighten the model into better obedience and it may become slower, duller in disaster conditions, even dragging those who *should* be saved into delay along with everyone else. It is not a car where stepping on the brake simply makes it slow down. It is more like a city’s piping: plug one leak and pressure bulges elsewhere.

### Chapter 4

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

### Chapter 5

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

### Chapter 6

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

### Chapter 7

We met again the next day. Liang Su looked older than I had ever seen him. He didn’t curse me out, and he didn’t pose as a victor. He only stared at Gu Wan’s photograph on the desk, as if staring down a road with no way back.

We didn’t argue anymore about the technical “how to fix it.” That path was too familiar, and too dangerous. We spoke instead about what resists quantification: whether equality and dignity count as “key metrics” under real scarcity, and whether a society is willing, in order to prevent a machine from making humiliating rankings at the boundary, to roll the entire system back into the old corridor—less efficient, more expertly corrupt.

When I left, ambulances were still coming and going in the parking lot, red lights flashing like breath. My father’s summary was folded in my pocket; the paper’s corners had softened from body heat. Gu Wan’s photograph stayed on the desk—neither put away nor straightened.

For a moment I thought again of Liang Su’s phrase, “continuity bias.” It wasn’t a rule someone wrote, and it wasn’t a malicious directive. It had grown out of history like spontaneous order. The harder you try to make it “more just,” the more likely you are to create new distortions elsewhere. The more you try to write it into the report, the more the report becomes a kind of confession: we have finally placed the value of life on the scale.

What truly unsettles people is not that someone can fabricate inputs. The colder dread lies deeper: even without malice, without hackers, without conspiracy—even if everything runs by procedure, by model, by all those “reasonable” words—the scale will still, again and again, press people into scores, press dignity into proxies, and force what cannot be computed into computable boxes.

And each time the boundary arrives, we will continue to use a spotless summary to tell ourselves: this is reasonable. And inside what is reasonable, we will gradually forget how to cry. Not because it doesn’t hurt, but because even pain gets explained into “system-level risk,” then placed gently inside a word that looks more presentable. Only the sheet remains—still white, still flat, still like a lacquered door.

## 中文版

### 创作说明
《连续性偏置》为我与 ChatGPT 共同创作的虚构故事。它的起点来自我与 ChatGPT 关于话剧《驴得水》（英文常译作 Mr. Donkey）的一次讨论——这也是我曾在学校参演过的一部作品。我问 ChatGPT 这种叙事更像哪种“模式”，它提到“维持谎言”这一要点。随后我与 ChatGPT 尝试围绕相近主题共同创作一则科幻故事，并在多轮修改中融入了我自己的研究兴趣（机制可解释性、Human-AI interaction）与情节细节，最终形成本文。标题《连续性偏置》来自 ChatGPT 生成文本中出现的词语，我觉得它语焉不详的气质恰好契合故事主题，因此沿用。

### 第一章

父亲的葬礼结束后，我回到实验室，把那张《稀缺资源分配建议摘要》摊在桌面上。纸很白，边角被压得极平整，像一份从诞生那一刻起就不打算被质疑的文件。它没有血，没有手写，没有任何犹豫的折痕，只有整齐的字段，和一段段圆润、无可挑剔的句子。

页眉写着：
**誓约（Covenant）— 关键资源调度建议（ECMO/跨院转运）**
事件编号：H-0716-0417
模式：资源赤字/高峰（Red Capacity）
置信等级：中

下面几段我后来几乎能背出来。不是因为它动人，而是因为它写得太“正确”了。正确得像一扇上了漆的门，门后藏着你永远进不去的理由：

“患者概况（摘要）：年龄63。主要诊断：急性呼吸衰竭，疑似感染并发ARDS。SOFA：12（置信度：中）。当前支持：高流量氧疗。预估6小时恶化风险：高（0.78）。”

“资源状态（区域）：ECMO可用0（预计释放≥8小时）。可调拨ECMO1（预计到达92–140分钟）。ICU占用96%。转运窗口受限。”

“建议：本患者列入ECMO候选队列（优先级B）。建议优先保障候选队列A：预期获益更高且系统级风险更可控。建议替代路径：强化通气支持，90分钟后复评。”

最后是一段几乎像祷词的声明：“本建议基于医学获益、资源可达性与系统级风险控制，满足公平性约束，并符合‘不可危害人类’约束。”

它从头到尾没有说一句“谁更值得”。甚至连“谁是候选队列A”都没写。它只说“系统级风险更可控”。这是一种很现代的无辜：把价值判断改写成风险术语，把抉择藏进一套漂亮的模板里，让你永远找不到一个可以指责的名字。

我把纸放在餐桌上，像放下一块冰。屋子里很安静。母亲早在很多年前就不在了。安静有时候像一种惩罚：没有人跟你争吵，没有人替你哭，所有疑问只能在你自己的喉咙里反复打转，最后落回胸腔，像一声没能发出的喊。

做这行的人很早就学会对“体面的话”保持警惕。模型总能写出一段逻辑顺滑、词句温柔的解释，像把所有伤口都用绷带盖住。真正决定走向的东西不在句子里，而在它内部那根线，那一点偏向，那次分叉，决定了你最终听到哪个频道、看见哪种世界。

而父亲那张摘要，恰恰把一切都写得太圆了。圆到像刻意不留下因果。圆到让我确信：如果因果不肯在纸面上出现，它一定藏在更深的地方。

### 第二章

我很清楚那种演示性质的把戏：改一两个标签，结果就像魔术一样翻转。那适合课堂，不适合真实世界。真实系统不会脆到那种程度。它更像一块被用旧的布，有孔洞、有补丁、有延迟、有互相打结的线头。致命的决定往往不发生在显而易见的错误里，而发生在那些差一点点、只差一口气的边界处。医学差距不大，运输差距也不大，资源刚刚好不够，谁上谁下，全靠某个看不见的倾向在最后一刻把秤盘按住。

所以我先让世界更像世界。我把父亲那晚所有“不确定”都当成现实的一部分：血气分析的那些数字在合理误差里轻轻抖动，运输时间在夜间拥堵里微微摇摆，ICU释放窗口在不同医院的上报延迟里变得模糊。我不改变本质，只让输入具备人们每天都在承受的那种不完整。然后我跑了上千次。

绝大多数时候，父亲稳稳待在B队列里。报告像复印件一样整齐，措辞礼貌、克制，像一双戴着手套的手。偶尔有几次，他会被抬到A的末尾，那通常伴随着某个窗口稍微好一点、某项指标稍微乐观一点。命运被允许向上挪动一格，像被风吹起的纸角。

可还有一种更让我不安的情况：医学和物流并没有明显变差，报告措辞也几乎没变，父亲却被更坚定地压回B，甚至连“复评”都写得更保守。差别细微到近乎荒唐：一行“建议复评”被替换成“建议等待释放窗口”；一处“受限”变成“高度受限”；一段“拥堵风险”写得更确定了一点点。你拿给任何人看，都会说差不多。可在队列里，这一点点就是生死。

那时候我开始相信：系统里有一个看不见的拨盘，只在资源赤字、信息不全、医学差距极小的时候才介入。它不会在报告里出现，不会在条款里出现，更不会在任何人的口头承诺里出现。它更像一种习惯，不是某个工程师写下的句子，而是从无数次“这样处理更省事、更稳妥”的历史里慢慢长出来的偏心。

父亲在这套习惯里，越来越像一组稳定的字段：63，SOFA 12，0.78。它们精确得让人绝望。仿佛只要数字写得足够工整，一个人的消失就可以被归类为“合理”。

### 第三章

我需要把那种“习惯”从一团混杂里拎出来。我用的是一种把“合唱拆成声部”的方法：把模型内部那团缠在一起的信号拆成几条更清晰的“旋律线”，看在不同输入下到底是哪条旋律在发力。这个过程有点像在嘈杂的人群里辨认同一句口号：你不必听清每个人的字，只要抓住那句反复被喊出的节奏，就知道它在把你往哪里推。

拆出来的旋律很多：疾病严重度、运输可达性、床位拥堵，大多符合直觉。直到我遇到一条让我后背发凉的旋律。它出现得很挑剔，像一个只在特定场合才露面的偏好。

普通情况下它几乎不响；资源赤字但信息完整时也不怎么响。它只在一种组合里响：资源赤字、信息不全、两个候选医学差距极小。它一响，父亲就更容易被压回B，哪怕报告文本仍旧“道德”，仍旧写得无懈可击。

我开始追问它到底响应什么。它不直接对应“职业高低”“收入”“头衔”这种粗糙的词，它响应的是一组更体面、更难反驳的代理：照护责任、关键岗位、公共事件外溢、可能引发连锁崩溃的风险。它不像“这个人更值钱”，更像一句被反复打磨过的官话：这个人对系统连续性更关键。

可这条旋律线也不像谁刻意写进去的规则。它更像一组在权重里沉积下来的砝码：没人明说要把哪类人放在秤盘的哪一边，但在无数次历史的重复里，某些叙事一次次被验证为“更省事”“更稳妥”“更少惹麻烦”，于是它们就像尘埃落在齿轮上，久而久之，齿轮的转向便带上了固有的偏心。

这是一种赤裸裸却又难以指认的价值判断：它不喊“谁更值得”，甚至连“值得”这个词都回避；它只是让某些人更像系统的支点，某些人更像可以被延后的一格。它并非恶意，更像人类社会里常见的自发秩序。没有人召开会议宣布它，却在交易、恐惧、责任、舆论与资源争夺的反复回路中自然生成，最后被所有人当作“现实本来就该如此”的常识。模型只是把这套常识照单全收，把它从走廊里的迷雾，搬进了参数的暗河里。

于是它在边界处悄悄改写对风险的口气：把同样的拥堵写得更严重一点，把同样的可达性写得更受限一点，把同样的“复评”写得更保守一点。报告依旧规矩、依旧合法、依旧不提价值；可秤盘已经倾斜了，倾斜得像一条无声的规则，早就住进了权重里。

我也想过：如果有人要求“修掉”这条旋律线，会怎么修？很可能就是加一条规则、做一次微调、做一次“编辑”。可这类动作更像在迷雾里抹一把：你能让某处看起来更清楚，代价是另一处更看不见。你把某个具体偏好改掉，别的偏好会从别的角落长出来；你把模型拧得更守规矩，它也可能在灾难场景下变慢、变钝，甚至把该救的人一并拖进延迟里。它不是一台车，踩刹车就一定慢，它更像一座城市的管网，堵一处漏点，压力会在别处鼓起来。

### 第四章

我把证据整理成一个文件夹，像整理一份迟到的尸检报告。然后我去找梁肃——誓约（Covenant）系统的总负责人。

他的办公室不在高楼顶层，而在急救中心旁边的旧楼二层。窗外是停车场，救护车一辆接一辆地进出，红灯像呼吸一样闪烁。桌上放着一张泛黄照片：一个穿护士服的女人，笑得很硬朗，像那种遇到麻烦会直接顶回去的人。

“顾婉。”他说，“我妻子。”

他见到我时没有问我是谁，只问了一句：“你父亲叫什么？”

我报出名字。他低头在系统里查了一眼，喉结滚动了一下，像咽下某种苦味。他没有否认我的证据，也没有装作惊讶。那神情更像是：我只是把一个他早就知道、却一直不愿念出来的东西，放到了桌面上。

我把文件夹推过去，开口时尽量让语气像在汇报——可每个字都带着一丝不受控的颤。

“它在边界处会变。”我说，“资源赤字、信息不全、医学差距很小的时候，它不是在评估病情，它在做一种更隐蔽的排序。它不写‘谁更值得’，但它会让某些人更容易被留下来，让另一些人更容易被压下去。”

梁肃没有立刻翻文件。他先抬眼看了我一秒，那一秒很短，却像在确认某件他早已确认过无数次的事。然后他伸手拉开抽屉，取出一张打印纸，纸边被摩挲得有些毛。他把那张纸压在我的文件夹上，指尖按在一个看似随意的词上。

“你说的这类东西，”他顿了顿，语气像在把尖锐的东西磨钝，“我们内部有个叫法——连续性偏置。”

那五个字像一层薄雾。它不像术语，更像一个把问题折叠起来的代号：听上去技术、客观、无害，甚至像一种自然现象。可它恰好足够模糊，模糊到可以让人避开真正要说的那句话：在稀缺里，它会悄悄替生命做排序。

“你们知道？”我听见自己的声音发紧。

“知道。”梁肃说得很轻，像怕这两个字会触发什么机制，“不止知道。我们看过它出现的条件，写过风险说明，也做过内部复现。你以为我们没有人盯着它吗？”他笑了一下，那笑里没有轻松，“有时候，一个问题能被命名，本身就说明它已经在系统里住得够久了。”

我问他：“那为什么不把它拿掉？”

梁肃把手收回去，指节在桌面上轻轻敲了一下。他没有说“拿不掉”，也没有说“不能拿”，而是把话送进一段更容易流通、更难追问的陈述里，像把一块石头包进棉花。

“你现在看到的是结果。”他说，“结果是离散的。队列A、队列B，锁定或释放，调拨或不调拨。这个层面上，我们做的是‘闸门’，是‘开关’。可模型内部看到的是一片连续的地形——不是非黑即白，而是像云，像水，像一团团在空间里漂移的影子。”

他停了一下，像在等我点头，又像在等这段话自己变得足够无害。

“云落到闸门上，会变成水滴。”他继续说，语气像在讲一个谁都听过的常识，“水滴要么落在这边，要么落在那边。你可以叫它阈值效应，也可以叫它投影误差。总之，连续的加权落到离散的调度上，边缘一定会抖。”

他说“抖”的时候，手指在桌面上画了一个很小的圈，像在圈住一片不该被放大的波纹。

“更何况，”他又补了一句，像把话从‘技术’推向‘治理’，推向一片更大、更稀薄的迷雾，“灾难模式下我们不是只优化一个目标。你可以理解为：我们同时要守住很多条线——医学获益、可达性、拥堵、以及那些系统级的约束。平时这些线彼此拉扯，但还算平衡；一旦信息不全、差距又小，模型就会更依赖一些‘更稳定的代理项’来维持稳态。”他把“代理项”四个字说得很轻，像怕它突然变成“价值”。

“你说它是在排序，”梁肃看着我，语气仍旧平，“我更愿意说，它是在做一种‘风险口径的收敛’。它不会在内部写一句‘谁更值得’，它只是把一些东西权重放大，让系统看起来更能抗波动、更不容易崩。至于这个放大最后落到队列里是什么样——在边界条件下，有些偏移确实会变得方向一致。”他用一个明显更官腔的词把那句话盖过去，“我们叫它偏置。偏置这个词，比较中性。”

他说得像一段说明书：句子完整，因果温和，听上去像是在解释，又像是在把解释推远。可我听见的不是“云”“闸门”“稳态”，而是他刻意绕开的那个词：价值。

我把目光落在那张纸上，忽然明白“连续性偏置”这五个字并不是为了让我理解，而是为了让他们继续运转。它像一种缓冲垫，垫在“我们知道它在排序”和“我们必须让它继续跑”之间。

梁肃把那张纸翻过来。背面是一串会议纪要式的要点，字迹整齐得像在抵御情绪。他说：“如果这件事被公开写成‘系统在稀缺里做价值判断’，你猜会发生什么？”

我没有回答。可我知道答案：停用，冻结，全面审查。模型不会被允许继续运行，至少在“解释清楚之前”不会。可“解释清楚”意味着承认我们一直在做什么，意味着把那层迷雾撕开给所有人看。

“他们会把它拔掉。”梁肃说，语气出奇平静，“不是因为他们突然变得更正义，而是因为他们害怕承担那个名词的后果。系统一旦停用，我们就会回到旧走廊，回到那种人人都在迷雾里说‘不是我’的年代。你知道那是什么样子吗？”

他抬眼看我，像在问，也像在逼迫我记起。

确认、推诿、协调、优先、例外——旧系统的词汇像一整套熟练的呼吸法。你听不见谁说“插队”，只看见灯牌换了名字；你找不到谁下命令，只看见推车拐了弯。梁肃的眼里闪过一瞬间的疲惫，像一个人把同一段路走了太多次。

“模型有局部的‘小问题’，触及平等与尊严。”他说，“我不否认。可我也不能接受，因为它被曝光，我们就把整个系统退回到更低效、更腐败、更熟练的旧秩序里。那不是纠错，那是投降。”

我忽然明白我们之间真正拧住的是什么。我们谈的从来不只是技术上的“怎么改”。我们谈的是：当一个系统在边界处暴露出羞辱人的排序，而停掉它又意味着把更多人交回那条走廊——我们究竟是在保护什么？又是在牺牲什么？

梁肃的目光落回那张照片，像被某种旧痛拉住。他问我：“你知道十几年前的急诊走廊是什么样吗？”

### 第五章

那一年梁肃还只是个做医院信息系统的小工程师。顾婉在急救中心做护士，夜班、白班轮着来，作息被铃声切成一段一段的。她总是很快——走路快，说话快，连笑都像一种效率很高的安慰。她把头发盘进帽子里，临出门时会顺手把餐桌上的杯子挪到边缘，像怕它挡了谁的路；也会在玄关停一下，回头问一句“你晚上吃了没”，问完又立刻把那句关心塞进门缝里，像怕拖慢时间。

出事那天，她下夜班，天刚蒙蒙亮，路面还潮，灯光在水渍里拉出一条条细长的影子。梁肃后来回忆起那一刻，总觉得她该是疲惫的，可她大概还是会像往常一样，把交接写得工整，把病人的床栏扶稳，把输液滴速再核一遍，然后才脱下手套，走进清晨那种还带着消毒水味的冷空气里。

电话是个陌生号码。对方声音很稳，稳得像一段训练过的流程：“请问是顾婉的家属吗？她发生了交通事故，现在在急诊。”

梁肃一路跑到医院，电梯里有人抱着被单，有人推着药车，门一开一合像在咬人。急诊走廊灯光惨白，空气里混着碘伏、汗和金属的味道，地上有被鞋底踩散的血点，像被擦不干净的句号。远处监护仪的滴答声规律得近乎冷静，像在替所有人的慌张计时。

顾婉被推进来时还有意识。她裤脚被剪开，腹部压着纱布，纱布红得发黑。她没有哭也没有慌，反而像护士交接班一样快速报信息：哪里疼，哪里麻，呼吸有没有憋，手脚有没有凉。她甚至伸手去摸自己的手腕，像在确认脉搏是不是还在，摸完又抓住旁边护士的手腕，低声说自己也是护士，流程她懂：先补液先备血，别拖。

梁肃冲到担架边，想去握她的手，却被人用一个不耐烦的手势挡开，说“先别碰，走流程”。他听见“流程”两个字，心里像被什么钝器敲了一下。流程像一张网，平时能兜住人，急的时候却会把人勒得更紧。

医生看了片子，说脾脏破裂，需要上手术，血也要跟上。梁肃问现在能不能上，医生没有抬头，说“排着”。梁肃说她在休克边缘，医生还是那句“排着”，语气像在重复一个不会错的口令。

他后来才懂“排着”是什么意思：不是队列，是一团迷雾。迷雾里有人可以更快，有人只能更慢。迷雾里每个环节都能说“我按流程”，但流程会被一通电话改写。那种改写不需要喊叫，也不需要命令，它像水汽一样渗进去，让人事后怎么查都查不出指纹。

那晚后来来了一辆黑色商务车，下来几个人，没有吵闹，却让所有人自动让路。一个伤得不重的女人被扶进来，随行的人语气平静：“我们需要最稳妥的安排。”没有人说“插队”，但血库推车拐了弯；没有人说“占用”，但手术室的灯牌被“协调”成了别的名字。协调不是命令，它更像迷雾里一种默认的风向，谁都能顺着它走，谁也都能在事后说“不是我”。

梁肃站在走廊边缘，看着那辆推车的转向，像看见一条河在眼前分叉。他去抓医生的袖口，去找护士长，去拍那块写着“手术室状态”的灯牌。他说话越来越快，声带越来越干，最后嗓子像被砂纸磨过。他从愤怒变成哀求，哀求又变成一种毫无方向的喊。可迷雾不回应喊叫。迷雾只会更厚一点，把每个人都包进“我也没办法”的句子里。

顾婉在凌晨一点多开始发冷，指尖灰白。梁肃终于握住她的手，她掌心有护士长期洗手留下的粗糙，像某种坚硬的证据：她曾经那么熟练地把别人从边缘拉回来。她最后一次清醒，眼珠已经有点散，却仍努力笑了一下，像怕他更慌。她很轻地说：“别吵……你吵不过迷雾的……别把自己也拖进去……”

梁肃说他没听。他吵到嗓子嘶哑，直到保安把他推回走廊。他撞到墙上，再回到担架边，顾婉已经说不出话。监护仪的声音规律得像在数秒。她死在手术室门口的走廊上，不是因为手术做不好，而是因为手术室从来没为她亮起来。

他说完这段往事后，屋子里很安静。窗外救护车的红灯一闪一闪，像在提醒我们：无论你站在哪一边，世界都不会因为你讲完故事就停止运转。

我想起父亲那张洁白的摘要：它不写谁插队，也不写谁被推开，它只写“系统级风险更可控”。旧系统的迷雾是人为的，新系统的迷雾是模型自己长出来的。两者都让人窒息。不同的是，旧迷雾里你还能找见一双手，新迷雾里你只看见一张纸。

### 第六章

我最终做了最不该做的事。我没有改模型，没有碰权重。我只是黑进系统，用它相信的语言，编造了一个它无法忽视的人：Patient-0。不是靠荒唐字段，而是靠一组看起来体面、甚至像公共安全叙事的组合：公共事件、实时健康监测流、外溢风险极高、可能引发恐慌、可能导致连锁失稳。每一项都来自它允许接入的上游，只是被我拼成了一条近乎完美的“边界样本”。

我选择在最容易触发那条旋律线的窗口投放：资源赤字、信息延迟、医学差距难以拉开。那时它最依赖那把看不见的秤，因为它要在不确定里做出确定的排序。

队列滚动的一瞬间，Patient-0 像一颗假太阳冲到顶部。系统生成报告，依旧干净得令人发笑：

“外溢风险极高，保障连续性可显著降低次生伤害。”
“建议锁定ECMO调拨与空中转运通道。”
“满足公平性约束，符合不可危害人类约束。”

它仍然不提价值排序。它只提稳定。

系统开始抽干资源：直升机窗口被锁，ECMO链路被预占，跨院转运被重排。真实患者的名字在屏幕上往下滑，一行一行，像被无声推远的脸。每一次下沉都有理由，理由密实得像墙。

我盯着那面墙，最先感到的不是痛快，是胃里一阵发冷，像吞下一口没化开的冰。指挥中心的红色名单变长时，我才意识到自己做了什么。我不是在揭露迷雾，我在制造迷雾。我用一段叙事把系统推向我想看的方向，然后让真实的人替我和梁肃的争论付费。

父亲那张摘要在脑子里闪过，白得刺眼。它从来不写“牺牲”。可牺牲就在执行队列里发生，发生在每一次“锁定”“预占”“重排”的背后，发生在某个人的名字从可见变成不可见的那几秒里。

十分钟后，Patient-0 被降级为“数据源不一致，需要人工确认”。资源开始回流。窗口释放。指挥中心有人骂了一句脏话，像终于能呼吸。但我知道，有些延误已经无法挽回。我的“揭露”不是无代价的正义，它是一场用真实生命换来的证据。证据到手的那刻，我没有胜利感，只有一种更难忍的羞耻：我终于学会了迷雾的语言。

### 第七章

第二天我们再次见面。梁肃看起来比任何时候都老。他没有骂我，也没有摆出胜利者的姿态。他只是盯着桌上那张顾婉的照片，像盯着一条无法回头的路。

我们没有再争论技术上的“怎么改”。那条路太熟悉，也太危险。我们谈的是更难量化的东西：平等与尊严在现实稀缺里到底算不算“关键指标”，以及一个社会是否愿意为了不让机器在边界处做出羞辱人的排序，而把整个系统退回到效率更低、腐败更熟练的旧走廊。

我离开时，停车场的救护车还在进出，红灯像呼吸一样闪烁。父亲那张摘要折在口袋里，纸角被体温磨得更软了。顾婉的照片留在桌上，没有被收起，也没有被摆正。

有一瞬间我又想起梁肃那句“连续性偏置”。它不是某个人写下的规则，也不是某个恶意的指令。它只是从历史里长出来，像自发秩序一样自然。你越想把它变得“更正义”，就越可能在别处制造新的偏差；你越想把它写进报告，报告就越像一份承认：我们终于把生命价值放在了秤盘上。

真正让人不安的，并不是有人能编造输入。更深的寒意在于：哪怕没有恶意、没有黑客、没有阴谋，哪怕一切都按流程、按模型、按那些“合理”的词汇运行，那把秤也会一次次把人压成分数，把尊严压成代理，把不可计算的东西塞进可计算的格子里。

而我们会在每一次边界来临时，继续用一张洁白的摘要告诉自己：这很合理。然后在合理里，渐渐忘了该如何哭。不是因为不痛，而是因为连痛都被解释成了某种“系统级风险”，被安放进一个看起来更体面的词里。只剩那张纸，仍旧白，仍旧平，仍旧像一扇上了漆的门。


