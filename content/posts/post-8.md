---
title: "10 Things Software Developers Should Learn about Learning"
date: 2023-12-31T02:01:58+05:30
description: "Learning is necessary for software developers. Change is perpetual"
tags: [tech,learning,research]
---

New technologies are frequently invented, and old technologies are repeatedly updated. Thus, developers do not learn to program just once—over the course of their careers they will learn many new programming languages and frameworks.


So recently I started learning regularly (Yeah finally I started) it’s been so long I didn't learn new things (I think more than 6 months, so in that period, I decided to take a little break and explore some places). But anyways, come to the topic. Recently, I joined one boot camp, and daily learning started while doing a full-time job and, of course, pursuing my hobby. Below are the 10 learnings from this recent experience and a bit of research.

Just because we learn does not mean we understand how we learn. One survey in the U.S. found that the majority of beliefs about memory were contrary to those of scientific consensus: People do not intuitively understand how memory and learning work.

As an example, consider learning styles. Advocates of learning styles claim that effective instruction matches learners' preferred styles—visual learners look, auditory learners listen, and kinesthetic learners do. People believe that learners' preferred styles should dictate instruction, though researchers have known for several decades that this is inaccurate.

While learners have preferred styles, effective instruction matches the content, not learning styles. A science class should use graphs to present data rather than verbal descriptions, regardless of visual or auditory learning styles, just like cooking classes should use hands-on practices rather than reading, whether learners prefer a kinesthetic style or not.

Decades of research into cognitive psychology, education, and programming education provide strong insights into how we learn. The next 10 sections of this article provide research-backed findings about learning that apply to software developers and discuss their practical implications. This information can help with learning for yourself, teaching junior staff, and recruiting staff.


### 1. Human Memory Is Not Made of Bits

Our brains are not hard drives that store information in neat, binary code. The human memory is a complex system influenced by emotions, context, and connections. Unlike computers, our memory is fallible, subjective, and associative.

Human memory is central to learning, Learning means that there has been a change made in one's long-term memory. Software developers are familiar with the incredible power of computer memory, where we can store a series of bits and later retrieve that exact series of bits. While human memory is similar, it is neither as precise nor as reliable.

Due to the biological complexity of human memory, reliability is a complicated matter. With computer memory, we use two fundamental operations: read and write. Reading computer memory does not modify it, and it does not matter how much time passes between writes and reads. Human long-term memory is not as sterile. Human memory seems to have a "read-and-update" operation, wherein fetching a memory can both strengthen and modify it—a process known as reconsolidation. This modification is more likely on recently formed memories. Because of this potential for modification, a fact does not exist in a binary state of either definitively known or unknown; it can exist in intermediate states. We can forget things we previously knew, and knowledge can be unreliable, especially when recently learned.

Another curious feature of human memory is "spreading activation." Our memories are stored in interconnected neural pathways. When we try to remember something, we activate a pathway of neurons to access the targeted information. However, activation is not contained within one pathway. Some of the activation energy spreads to other connected pathways, like heat radiating from a hot water pipe. This spreading activation leaves related pathways primed for activation for hours.

Spreading activation has a negative implication for memory1 and a positive implication for problem-solving. Spreading activation means that related, but imprecise, information can become conflated with the target information, meaning our recall of information can be unreliable. However, spreading activation is also associated with insight-based problem solving, or "aha moments." Because pathways stay primed for hours, sometimes stepping away from a problem to work on a different one with its own spreading activation causes two unrelated areas to connect in the middle. When two previously unrelated areas connect, creative and unique solutions to problems can arise. This is why walks, showers, or otherwise spending time away from a problem can help you get unstuck in problem solving.

Think about learning a new programming language. Instead of rote memorization, create associations. If you're learning a new function, relate it to something you already know. For instance, if you're familiar with Python, connecting a new JavaScript function to a similar one in Python can help solidify the memory.

In summary, human memory does not work by simply storing and retrieving from a specific location like computer memory. Human memory is more fragile and more unreliable, but it can also offer great benefits in problem solving and deep understanding by connecting knowledge together. We will elaborate further on this in later sections, especially on retrieving items from memory and strengthening memories.


### 2. Human Memory Is Composed of One Limited and One Unlimited System


We have a short-term memory with limited capacity and a long-term memory with seemingly infinite potential. Understanding how to transfer information from one to the other is crucial for effective learning.

Human memory comprises two main components that are relevant to learning: long-term memory and working memory. Long-term memory is where information is permanently stored and is functionally limitless; in that sense, it functions somewhat like a computer's disk storage. Working memory, however, is used to consciously reason about information to solve problems; it functions like a CPU's registers, storing a limited amount of information in real time to allow access and manipulation.

Working memory is limited, and its capacity is roughly fixed at birth. While higher working-memory capacity is related to higher general intelligence, working-memory capacity is not the be-all and end-all for performance. Higher capacity enables faster learning, but our unlimited long-term memory removes limitations on how much we could ultimately learn in total.1 Expert programmers may have low or high working memory capacity but it is the contents of their long-term memory that make them experts.

As people learn more about a topic, they relate information together into chunks.a Chunking allows the multiple pieces of information to act as one piece of information in working memory. For example, when learning an email address, a familiar domain, such as gmail.com, is treated as one piece of information instead of a random string of characters, like xvjki.wmt. Thus, the more information that is chunked, the larger working memory is functionally. Using our computer analogy, our working memory/CPU registers may only let us store five pointers to chunks in long-term memory/disk, but there is no limit on the size of the chunks, so the optimal strategy is to increase the size of the chunks by practicing using information and solving problems.

When you're learning a complex algorithm, don't cram all the details into your short-term memory. Break it down into smaller, manageable parts, and gradually transfer them to your long-term memory. Think of it like building a puzzle; each piece contributes to the overall picture.

### 3. Experts Recognize, Beginners Reason

One key difference between beginners and experts is that experts have seen it all before. Research into chess experts has shown that their primary advantage is their ability to remember and recognize the state of the board. This allows them to decide how to respond more quickly and with less effort.

Expert developers can reason at a higher level by having memorized common patterns in program code, which frees up their cognition.

Expert developers can reason at a higher level by having memorized (usually implicitly, from experience) common patterns in program code, which frees up their cognition. One such instance of this is "design patterns" in programming, similar to previously discussed chunks. An expert may immediately recognize that a particular piece of code is carrying out a sorting algorithm, while a beginner might read line by line to try to understand the workings of the code without recognizing the bigger picture.

A corollary to this is that beginners can become experts by reading and understanding a lot of code. Experts build up a mental library of patterns that let them read and write code more easily in the future. Seeing purely imperative C code may only partially apply to functional Haskell code, so seeing a variety of programming paradigms will help further. Overall, this pattern matching is the reason that reading and working with more code, and more types of code, will increase proficiency at programming.

Consider debugging. Beginners might go through their code step by step, reasoning through each line. Experts, on the other hand, might quickly identify the problem based on patterns they've seen before. However, the expert was once a beginner who meticulously reasoned through code.

### 4. Understanding a Concept Goes from Abstract to Concrete and Back

Learning is not a linear process. Concepts start abstract, become concrete as you practice, and then might return to abstraction as you gain a deeper understanding.

Research shows that experts deal with concepts in different ways than beginners. Experts use generic and abstract terms that look for underlying concepts and do not focus on details, whereas beginners focus on surface details and have trouble connecting these details to the bigger picture. These differences affect how experts reason but also how they learn.

Problem-solving is (incorrectly) conceived as a generic skill. However, this is not how problem-solving works in the brain.

Programming frequently involves learning about abstract concepts. Faced with an abstract concept to learn, such as functions, people often reach for concrete instantiations of the concept to examine, for example, the abs function that returns the absolute value of a number. One challenge is that as concepts get more abstract (from values to variables/objects to functions/classes to higher-order functions/metaclasses and eventually category theory), the distance to a concrete example increases. The saving grace is that as we learn abstract concepts, they become more concrete to us. Initially, a function is an abstract concept, but after much practice, a function becomes a concrete item (or chunk) to us and we can learn the next level of abstraction.

Take the concept of object-oriented programming. Initially, it might seem abstract, but as you implement it in a project, it becomes concrete. However, as you become more experienced, you might start seeing it abstractly again, understanding the underlying principles rather than just the syntax.


### 5. Spacing and Repetition Matter


Cramming doesn't lead to long-term retention. Spacing out your learning and repeating information at intervals significantly improves memory.

How often have you heard that you should not cram for an exam? Unless, of course, you want to forget everything by the next day. This advice is based on one of the most predictable and persistent effects in cognitive psychology: the spacing effect. According to the spacing effect, humans learn problem-solving concepts best by spacing out their practice across multiple sessions, multiple days, and ideally, multiple weeks.

The reason spacing works is due to the relationship between long-term and working memory. When learners practice solving problems, they practice two skills. First, matching the information in the problem to a concept that can solve it (such as a filtering loop), and second, applying the concept to solve the problem (such as writing the loop). The first skill requires activating the correct neural pathway to the concept in long-term memory

If learners repeatedly solve the same kind of problem, such as for-each loop problems, then that pathway to long-term memory stays active, and they miss practicing the first skill. A common result of un-spaced practice is that people can solve problems, but only when they are told which concept to use.

While interleaving different types of problems, such as loop and conditional problems, can help, pathways take time to return to baseline, making spacing necessary to get the most out of practice time. In addition, the brain needs rest to consolidate the new information that has been processed so that it can be applied to new problems.

To structure a day of learning, learners should limit learning bouts to 90 minutes or less. The neuro-chemical balance in the brain makes concentration difficult after this point. After each learning bout, take at least 20 minutes to rest. Really rest by going for a walk or sitting quietly—without working on other tasks, idly browsing the Internet, or chatting with others. Rest speeds up the consolidation process, which also happens during sleep.

Within a learning bout, there are a couple of strategies to maximize efficiency. First, randomize the order of the type of problem being solved so that different concepts are being activated in long-term memory.Be forewarned, though, that randomizing the order improves learning outcomes but requires more effort. The second strategy is to take short breaks at random intervals to enhance memory consolidation. A 10-second break every 2–5 minutes is recommended.

Imagine you're learning a new library. Instead of trying to memorize all the functions in one sitting, space it out. Regularly revisit and practice using the functions in different contexts. This not only reinforces the information but also aids in long-term retention.

### 6. The Internet Has Not Made Learning Obsolete

Despite the vast resources available online, effective learning requires more than just access to information. Curated learning paths, meaningful projects, and interactive experiences are still vital.

The availability of programming knowledge changed with the advent of the Internet. Knowledge about syntax or APIs went from being buried in reference books to being a few keystrokes away. Most recently, AI-powered tools such as ChatGPT, Codex, and GitHub Copilot will even fill in these details (mostly accurately) for you. This raises an obvious question: Why is it worth learning details—or anything at all—if the knowledge is available from the Internet within seconds?

We learn by storing pieces of knowledge in our long-term memory and forming connections between them. If the knowledge is not present in the brain, because you have not yet learned it well, the brain cannot form any connections between it, so higher levels of understanding and abstraction are not possible. If every time you need a piece of code to do a database join you search online for it, insert it, and move on, you will be unlikely to learn much about joins. The wisdom of relying on the Internet or AI differs between beginners and experts: There is a key distinction between a beginner who has never learned the details and thus lacks the memory connections, and an expert who has learned the deeper structure but searches for the forgotten fine details.

There is also the issue of cognitive load discussed earlier. An Internet search requires a form of context switching for the brain; its limited attention and working memory must be switched from the task at hand (programming) to a new cognitive task (searching the Internet and selecting a result or evaluating an AI-generated result). If the required knowledge is instead memorized, then not only is access much faster (like using a cache versus fetching from a hard disk), but it also avoids the cognitive drain of context switching and filtering out extraneous information from the search. So there are multiple reasons to memorize information, despite it being available on the Internet.

Learning a new framework by reading documentation is valuable, but it's enhanced by building a real-world project. The internet provides information, but application and context come from hands-on experience.

### 7. Problem-Solving Is Not a Generic Skill

Problem-solving is context-dependent. What works in one scenario might not in another. Understanding the problem domain is as crucial as the ability to solve problems.

Problem-solving is a large part of programming. One common (but incorrect) idea in software development is to directly teach problem-solving as a specific skill, which can then be applied to different aspects of development (design, debugging, and so on). Thus, problem-solving is (incorrectly) conceived as a generic skill. However, this is not how problem-solving works in the brain.

While humans do have some generic problem-solving skills, they are much less efficient than domain-specific problem-solving skills, such as being able to debug programs. While we can learn to reason, we do not learn how to solve problems in general. Instead, we learn how to solve programming problems, or how to plan the best chess move, or how to create a knitting pattern. Each of these skills is separate and does not influence the others. Research into chess found little or no effect of learning it on other academic and cognitive skills, and the same is true for music instruction and cognitive training.36 This inability to transfer problem-solving skills is why "brain training" is ineffective for developing general intelligence.

The one exception to this rule appears to be spatial skills. Spatial skills allow us to visualize objects in our mind, like a Tetris shape, and mentally manipulate those objects, like rotating a Tetris shape. Training these generic skills can improve learning in other disciplines. This phenomenon is so unusual that it has caused much consternation in cognitive and learning sciences. Yet, spatial training improves performance on a range of non-verbal skills regardless of initial ability, age, or type of training task.Recent work has even demonstrated that spatial training can improve efficiency for professional software developers, likely because they are still learning new concepts. Even with this strange exception, the best way to learn how to solve programming problems is still to practice solving programming problems rather than looking for performance benefits from learning chess or other cognitive training.

There is a secondary implication here for recruitment. One popular idea for screening programming candidates was to give brain-teaser puzzles, such as how to weigh a jumbo jet. As Google worked out by 2013, this is a waste of time7—there is no reliable correspondence between problem-solving in the world of brain teasers and problem-solving in the world of programming. If you want to judge programming ability, assess programming ability.

Consider two developers solving a bug in a web application. One might excel because of their deep understanding of frontend technologies, while the other, despite being a skilled backend developer, might struggle. Contextual expertise matters in problem-solving.


### 8. Expertise Can Be Problematic in Some Situations

Expertise can lead to cognitive biases. Experts might overlook fundamental steps assuming them to be too obvious. Being aware of this and revisiting basics is essential for continuous improvement.

We have discussed many ways in which expertise benefits learning and performance. However, being an expert can also lead to problems.

Programmers use tools and aids to be more effective, such as version control systems or IDEs. Such tools can have different effects on beginners and experts. Beginners may get overwhelmed by the amount of options available in professional tools (due to increased cognitive load) and may benefit from beginner-friendly hints on how to use the tool. However, experts find the same hints more distracting than useful because they already know what to do. This is known as the expertise-reversal effect: Hints and guides that help beginners can get in the way of experts and make them less productive.

Programmers usually learn multiple programming languages throughout their careers. Knowing multiple languages can be beneficial once they have been mastered, but sometimes transferring knowledge from one programming language to another can lead to faulty knowledge. For example, a programmer may learn about inheritance in Java, where one method overrides a parent method as long as the signatures match, and transfer this knowledge to C++, where overriding a parent method additionally requires that the parent method is declared virtual. These kinds of differences—where features are similar in syntax but different in semantics between languages—specifically hinder the transfer of knowledge

Experts often help to train beginners, but experts without experience in training others often do not realize that beginners think differently. Thus, they fail to tailor their explanations for someone with a different mental model. This is known as the expert blind-spot problem: difficulty in seeing things through the eyes of a beginner once you have become an expert. It can be overcome by listening carefully to beginners explain their current understanding and tailoring explanations accordingly.

Sometimes, however, knowledge becomes so automated that it is difficult for experts to verbalize it.1 This automated knowledge is why experts have intuitions about how to solve problems or explain their process as, "I just know." In these cases of tacit knowledge, beginners might better learn from instructional materials designed to support beginners, often called scaffolded instruction, or from a peer rather than an expert. A more knowledgeable (but still relatively novice) peer is a highly valuable resource to bridge the gap between beginners and experts. They can help the beginner develop new knowledge and the expert to rediscover automated knowledge.

An experienced developer might dismiss the importance of writing clean, readable code, assuming it's too basic. However, in a team setting, clear code is crucial for collaboration and maintenance.

### 9. The Predictors of Programming Ability Are Unclear


Traditional markers like academic degrees don't always correlate with programming proficiency. Skills, experience, and the ability to learn and adapt are often better indicators.

The success of learning programming, like most activities, is built on a mix of inherent aptitude and practice. Some people believe it is purely about aptitude—the "you're born with it" view—and some believe it is almost entirely about practice—the "10,000 hours" idea that only sufficient practice is required for expertise. Both extreme views are wrong, and in this section, we will explore the evidence for the differing effects of aptitude and practice.

There has been much research to try to predict programming aptitude but few reliable results. Attempts to produce a predictive test for programming ability have generally come to naught. Research has found that all of the following fail to predict programming ability: gender, age, academic major, race, prior performance in math, prior experience with another programming language, perceptions of CS, and preference for humanities or sciences.

There is mixed evidence for the importance of years of experience, which relates to practice. There is a correlation between the reputation of programmers on Stack Overflow and their age: Older people have a higher reputation

However, a recent study found only a weak link between years of experience and success on a programming task among programmers who were relatively early in their careers,suggesting that aptitude may have a stronger effect than experience, at least early in programmers' careers.

Consider two candidates – one with a computer science degree and the other with a diverse portfolio of projects. The latter might demonstrate a more practical and adaptable skill set, making them a better fit for a dynamic development environment.

In short, it is very hard to predict who will be able to program, especially in the long term. Programmers could come from any background or demographic, and links to any other factors (such as intelligence) are generally fleeting in the face of experience. Therefore, in recruiting new programmers, there are no shortcuts to identifying programming ability, nor are there any reliable "candidate profiles" to screen candidates for programming ability.

### 10. Your Mindset Matters

Believing in your ability to learn and adapt, known as a growth mindset, significantly impacts your learning journey. Embrace challenges as opportunities to grow.

There is a long-standing idea of a binary split in programming ability: You either can program or you cannot. There have been many competing theories behind this. One of the more compelling theories is the idea of learning edge momentum, that each topic is dependent on previous topics, so once you fall behind you will struggle to catch up. 

A less compelling theory is the idea of a "geek gene" (you are born with it or not), which has little empirical evidence. we have recently come to understand differences in programming ability as differences in prior experience. Learners who might seem similar (for example, in the same class, with the same degree, completing the same bootcamp) can have vastly different knowledge and skills, putting them ahead or behind in terms of learning edge momentum or, within a snapshot of time, making them seem "born with it" or not. A similar effect is found in any highly technical field that is optionally taught before university (for example, CS, physics, and engineering).

The binary split view, and its effects on teaching and learning, have been studied across academic disciplines in research about fixed versus growth mindsets. A fixed mindset aligns with an aptitude view that people's abilities are innate and unchanging. Applied to learning, this mindset says that if someone struggles with a new task, then they are not cut out for it. Alternatively, a growth mindset aligns with a practice view—that people's abilities are malleable. Applied to learning, this mindset says that if someone struggles with a new task, they can master it with enough practice.

If you encounter a difficult concept, instead of thinking, "I can't understand this," approach it with, "I can't understand this yet." The growth mindset fosters resilience and perseverance in the face of challenges.


<br>
<br>

![Image](https://i.ibb.co/nfW3nX2/Screenshot-2023-12-31-at-12-35-08-PM.png)

<br>
<br>


*Intelligent people will not always make good programmers, and good programmers need not be high in general intelligence*


In conclusion, the journey of learning as a software developer is multifaceted. Understanding the intricacies of memory, embracing a growth mindset, and appreciating the nuances of expertise can transform the learning experience. So, whether you're a seasoned developer or just starting, remember that effective learning is not just about the quantity of information but the quality of understanding.


<br>
<br>

![Image](https://i.ibb.co/wSN70Dd/IMG-3128.jpg)

<br>
<br>

Thanks for reading complete blog! See you in next blog.



