# HTB CPTS: A Journey Through Pain, Enumeration, and Existential Crises

A personal experience, preparation guide, and lessons learned.


1. Introduction
    
    - A Little About Me (whoami)
        Hi, I'm Nightcrypt! As of writing this article, I'm a Junior Offensive Security Consultant primarily involved in web application and web services penetration testing engagements. Before landing this role, I was just an office worker at an international school who spent almost every day for two years upskilling in cybersecurity.
        ![Two years of studying cybersecurity after work. Everything is fine.](https://github.com/user-attachments/assets/27365cd7-3da1-4115-afd5-094b26e62402) _Two years of studying cybersecurity after work. Everything is fine._

        I have completed several Tryhackme paths as a beginner and eventually crushed INE's eJPT exam on my first take. You might ask why am I sharing about myself. Well, I wanted my readers to understand that I have a solid cybersecurity foundation and penetration testing background before taking this exam. I wouldn't recommend jumping straight into this certification as an absolute beginner. However, if you have the resources and simply want to challenge yourself or assess your current capabilities, that's entirely up to you. Some takers are just trying this Certification exam to test their skills to understand their baseline then proceed in filling the gaps before getting serious in crushing it.
        
    - Why CPTS?
        If I'm gonna be honest, it's about the cost. I think **$1,749** (or more depending on the bundle you wanted to avail) is a little too much for an intermediate-level certification. You may argue that it's about the prestige and HR recognition because it's the "gold standard", but yeah. I agree because it is. However, as a broke guy with a "Junior" or skill level, I wanted to test my capabilities in delivering Intermediate-level engagements without breaking my bank.
        CPTS and OSCP are always getting compared within the professionals in the industry. OSCP has established industry recognition and is frequently used as a hiring requirement or screening criterion. CPTS, on the other hand, appealed to me because of its technically demanding training material, practical approach, and emphasis on developing a structured penetration testing methodology.
        I'm still in my early career so I'm more focused on building my skills before gaining recognitions within the industry. HTB Academy can be overwhelming, but everything in the modules are helpful and necessary in filling out my skill gaps and building or strengthening my methodology. In my opinion, HTB offers a bang for a buck in terms of building skills than OffSec.
    
2. The Preparation
    
    - My Starting Point
        As mentioned, I did not start grinding the Academy as an absolute beginner. I've been grinding Tryhackme Paths including solving practical rooms, and solving active HTB boxes in the HTB Labs. When I was employed in my current job, we were trained for six months. Our training mostly involves solving boxes and creating reports about our findings. We also simulate readouts which forced me to develop my soft skills along with my technical skills. We also shadow other consultants before we got deployed to deliver billable projects. Those accumulated experience made grow exponentially and become stronger compared to my self years ago. With this, I got the confidence to tackle the exam so I started grinding the CPTS path whenever I'm on a "white-day" (days when I don't have billable projects or shadowing opportunities). 
    - How I Approached HTB Academy
        I approached HTB Academy in a rather conventional way: I simply followed the entire learning path from beginning to end, which I think is a little inefficient since I already have the background. My colleagues said that I should've just skipped some parts that I'm already knowledgeable about. 

        So if you're already skilled and had some hands-on background, it's alright to skip some parts and just went straight in answering the tasks to complete the modules.
        But yeah. I still insisted to follow the path and read everything because I might still get some tips and tricks which I might miss if I skipped them. I made sure to take notes throughout every module, which I highly recommend. It's impossible to remember everything, and having structured notes can save you countless hours when revisiting concepts or troubleshooting unfamiliar situations.
    - My Study Habits and Resources
        I made sure to allocate at least 2 hours of my time everyday to study. Sometimes I made sure to complete one section per day. Of course, there are days that I missed because I was busy like some emergencies, hectic projects, or some events or responsibilities that I'm supposed to attend to.
    - Things I Wish I Knew Beforehand
        There's so little things that I regretted not doing but if there's anything that comes to my mind on what things I wish I knew beforehand, is that I should've mastered using `Sysreptor`. I mean it's easy and it's just using a markdown format to render the report contents but understanding the HTB template structure and on how to write the details in each section, would be so beneficial and would made my reporting a little faster and better. 
        I was used to do the reporting based on how our company do it but in HTB, it's a little different especially in the walkthrough part. This, I think is an additional Section which are not always present in any professional reports because there's the "Details" part of each Findings where a tester should put the PoC. I also wish I knew that the walkthrough requires every details of the steps I've done. Some also mentioned that it's normal to reach 100 to 200+ pages in the report and here I thought, I should've redacted or cut every unnecessary details. It is the part that I should've provided a lot more details and supporting screenshots and evidences. I'm still not sure if it's alright to show sensitive information such as usernames and passwords but I redacted them just to be safe. 
    
3. The Exam
    The exam is brutal and fun at the same time. It puts me in a roller coaster of emotions. Without further shitty introduction, the following describes everything I've experienced.
    - Going In: Expectations vs. Reality
        Even if I knew the exam is far from a typical HTB Lab, I got used to it and I still expected the exam to mirror the standalone **HTB Academy machines**. However, the reality is a little far from what I expected. The environment is **black-box and ambiguous**, lacking obvious entry points or known CVEs. It requires deep **enumeration** and the ability to handle novel, non-linear scenarios where a single compromised host may yield no immediate progress. This is what made me spend and lose lots of time figuring out things, overthinking, and getting frustrated most of the time.
        ![Expectations vs. Reality](https://github.com/user-attachments/assets/73686cb8-6641-4d69-894f-e0726c951e79)
      _Panel 1: Your expectation: A straightforward machine with an obvious foothold._ | 
      _Panel 2: Reality: A complicated network diagram with question marks everywhere._

    - My Approach and Methodology
        I approached the exam using a methodology I had developed through practice: enumerate first, leave no stone unturned, formulate a hypothesis, and then test it. Rather than blindly attempting exploits, I wanted to understand why a particular attack path might work before pursuing it.
        ![Me connecting three seemingly unrelated findings at 3 AM.](https://github.com/user-attachments/assets/ab1ab6a1-b24d-4c93-ae3e-9c160043fa2b) _Me connecting three seemingly unrelated findings at 3 AM._

        Of course my methodology is not perfect. I still stumbled upon rabbit holes but with a solid methodology, you'll notice that you're in a rabbit hole in no time. Also, make sure to think outside the box. Not every path is obvious. Sometimes, you need to approach the same problem from a different perspective. A hypothesis is only useful when you can validate it through evidence and consistent results. Searching is a skill and with the help of AI, I was able to progress my research faster and learn new things while doing the exam. It is important to mention that I do not rely on it like fully automating the engagement. I treat it like an assistant or a companion when doing the testing. AI is just a tool and not my replacement. The exam still needs me as the pilot because as my mentors say, "as a consultant, you are the supposed to be the expert" so it is necessary fully understand the problem, where it is located, what's the impact of a successful exploitation, and how would another technical person be able to replicate your proof-of-concept (PoC).
        I also made sure to keep taking notes. Practice having structured note taking while solving boxes to make it feel natural like a muscle memory. I'll explain why later.
        
    - The Struggles, Breakthroughs, and Everything In Between
        Ugh... this is giving me nightmares. I had a fair share of struggles in this exam. this is not a smooth ride. I literally jumped into the exam while still recovering from an illness I got after working night shifts on my previous engagement. Also, I admit that sometimes, my methodology is all over the place. 
        There were instances when I missed potential targets during enumeration because I relied on an inadequate wordlist. This taught me an important lesson: don't immediately assume that an unsuccessful enumeration attempt means there is nothing to discover. Sometimes, changing your wordlist, parameters, or approach can reveal what you initially missed. It does not only apply to fuzzing but in any other situations. Sometimes it is necessary to look on things differently to test if your hypothesis is right and consistent in different scenarios.
      
      	<p align="center"> <img src="https://github.com/user-attachments/assets/35710b5c-d40d-4d5d-92c5-aaf56e391b64" alt="Me running the same enumeration command for the third time with a different wordlist."width="450"> </p>
		<p align="center"><i>Me running the same enumeration command for the third time with a different wordlist.</i> </p>

		During the exam, I remembered that I got some credentials but I didn't know where I could use them. In CTFs or HTB Labs, getting credentials is straightforward. You'll usually locate another service or endpoint where you can use them. However, the exam isn't always that straightforward. There are additional steps, and you need to enumerate further to understand where those credentials fit into the bigger picture.

		<p align="center">
  		<img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExNGx6cXR4cmMxZHliMnh4cGd3MGJ4bGdhaHZ1djEwaWJmYXhkaDl4ciZlcD12MV9naWZzX3NlYXJjaCZjdD1n/5zoxhCaYbdVHoJkmpf/giphy.webp" alt="Confused reaction GIF" width="450">
		</p>

		<p align="center">
  			<i>When you finally recover credentials but have absolutely no idea what they're for.</i>
		</p>


        Next thing that I remembered is I struggled in some situations that requires me to know the basics. I can't emphasize this enough and I hope no one falls for this trap. I got stuck because I fail to understand deeply a certain concept that was required for me to find a solution. I'm just glad I got some mentors and colleagues who already experienced that kind of misconfiguration so I was able to ask for some guidance. LLMs also helped me understand those concepts and helped me on how to approach them. There may be times that the technology featured in the exam is unfamiliar but the basics are just the same. And this I can say, having a solid methodology is really essential in this exam. In a real-world engagement, there are times that you won't be familiar with the technology your clients are using. On the spot research and asking the right questions or searching for the right thing is necessary to come up with a hypothesis and exploits that would likely work.
        Lastly, this is the one that still haunts me. Expect for the worst case scenarios. Create snapshots of your VM if your disk space allows you to. I recommend taking notes on your host machine instead of the VM to avoid losing your progress. If also possible for your case, host your `Sysreptor` in a different VM. This would prevent you from losing your time caused by troubleshooting if your VM breaks. I broke my VM in the middle of the exam that forced me to use the dedicated Pwnbox.
      
       	<p align="center">
  			<img src="https://github.com/user-attachments/assets/f7790fb1-a927-45f6-a61c-98b2d6c85190" alt="The real adversary was the VM we broke along the way." width="450">
		</p>

		<p align="center">
  			<i>The real adversary was the VM we broke along the way.</i>
		</p>

        
    - Documentation and Reporting: The Second Exam
        This is the boring part, but it's the most important thing because this will probably be the thing that would determine if you'll pass or fail. 
        Documentation is not just about writing the report and just taking down notes. It also includes preserving your command logs, using terminal multiplexer to organize your commands, and others depending on how you approach your testing. 
        As mentioned earlier, I'm glad that I was able to take notes and preserve my logs because if not, I might've to redo everything that I already did just to continue the exam on the dedicated Pwnbox.
        I also recommend that when you are halfway in the exam or when you got the sixth flag, you also make sure that your report is halfway done to prevent cramming on the report like I did. I think it also affected my report greatly because I think, If I had started the report earlier, it will have a better quality.
        One of the most valuable lessons from my experience is that technical exploitation is only part of the assessment. You also need to demonstrate your findings through reproducible evidence and a properly structured report. And a `Sysreptor` solves most of them. You should not just focus on the findings. Make sure to supply the necessary information in the other sections like the Executive Summary and the Appendices. Proofread everything and make sure it makes sense that even a third grader can understand.
        Here's a simple recommended workflow:
        - Enumerate and document observations.
        - Preserve commands and their outputs.
        - Record credentials and their associated context securely.
        - Capture screenshots at important milestones.
        - Document exploitation steps while they're still fresh.
        - Transfer validated findings into Sysreptor.
        - Review the report for completeness and reproducibility.
     
          ![Documentation hell.](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExZHh5eW10aXd3MWp4ZTE3a3l0eDlwYnZrazJ4bzlvbm0yeDg2bjl4cCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/3orifaQEOagjYJ1EXe/200.webp)

    
1. The Aftermath: Waiting, Wondering, and Losing My Sanity.
    
    - The Waiting Game
        This is the part that tortures me. Waiting for the results feels like being in a Limbo (well figuratively. I haven't been there obviously. I'm still alive FFS lol). After the grueling 10 days, I was forced to wait for no one knows how long. The platform says results will be given within 20 days. However, it forums and people from the discord servers mentioned that HackTheBox usually releases results earlier. I knew someone who also took the exam the same day as I am. He submitted his report earlier than I do since he got the 12 flags on the 7th day. Three days later, he got his results. It is also the time when I just submitted mine. I got the 12th flag on the 9th day and pulled an all nighter to finish the report. I honestly don't think I did a great job in writing my report. Since I lost some time getting constantly stuck and troubleshooting my machine, I cram in writing it and needed some help from some AI models on how am I going to phrase my findings and the walkthrough from my notes as the source of truth. I pulled out my notes and narrate to AI in each phase to show my workflow. Of course, I treated it like a real engagement so it is important to note that sensitive information should be redacted. Also, you don't want my client or a reader to think that AI made it so I still spent time proofreading it and correcting things to maintain the accuracy of the final report. It is important to note that getting the minimum requirements of 12 flags don't guarantee a pass. It still depends on the quality of the report. I gotta be honest, the feeling of not knowing whether I pass or fail is not good. I get paranoid, anxious, and that feeling of uncertainties made me feel sick. I literally got some nightmares that woke me up in my sleep and made me check my emails constantly to see if the results are out. 
    ![Mr. Bean](https://github.com/user-attachments/assets/75e37e4a-00f7-4161-91ea-d35a96f1f17b) _Me refreshing my inbox for the 47th time._

    - The Results
        One ordinary Thursday, I am sitting on a solo pentest engagement. While testing and getting stressed and scratching my head on the current project that I'm delivering, I got an email from HackTheBox. It says I'm certified! LEZZGOO!!! Well, that's what I wanted to express. but I'm too occupied with this current engagement that I don't even know what to feel. It sinks in during the weekend lol. I felt relieved and tired at the same time. I felt the burn out and I have a feeling like I don't want to touch a computer for a while. I don't even want to take another certification exam on this level yet. I realized that these types of exams really require lots of preparation like mental, physical, and emotional conditioning. It's hard taking this exam while being sick while also dealing with your personal and professional issues.
    ![Cheers!](https://github.com/user-attachments/assets/ad0a47d3-188f-4c92-880c-160d2d35c2e5) _12 flags. 10 days. One report. One very tired pentester._

    
2. Lessons Learned
    
    - What Worked
        I guess getting lots of hands-on experience worked for me. I have been participating in HTB Seasons twice while grinding the CPTS path. I make sure to solve machines every weekend whenever there are seasonal machines are released. The six months training in my current company also helped a lot because I get to experience the realities of the industry. Of course, there is a big chance that you, reading this, is not yet employed as a consultant or a penetration tester that's why you are reading this personal blog. So I guess, solving labs, or getting some hands-on experience in any shape or form is the best way to supplement your learning in the HTB Academy. Doing so, will help in strengthening your foundation and your methodology. 
    - What Didn't
        In the actual exam engagement, I guess it's safe to say that I should've not expected it to be a CTF. I haven't been able to take on real External and Internal infrastructure projects yet and I only have HTB labs experience. There are similarities, but there are also a big difference between the exam and the labs. Not everything is straightforward. The exploits, yeah they're pretty straightforward but the path, you'll really have to think outside the box to find it.
    - What I'd Do Differently
        For this one, I guess I should've taken more AD and Windows experience. I am comfortable doing it but there are things that I should've improved my muscle memory like in privilege escalation and chaining AD permissions and misconfigurations. And if I had more time and money, I might have solved all the CPTS track to really build a muscle memory and get comfortable and confident while taking the exam. I should have also treated my body with the same training as my brain. Taking rests and working out might have increased my efficiency and my quality of life.
    - Advice for Future Candidates
        My advice? Well, don't take advice from a guy who willingly spent 10 days questioning his existence in front of a computer. JK lol hahaha. I guess I'll start with the basics. Here are the following:
        - Know your learning style (visual, auditory, or if you're a weird one that needs to move around just to remember things or experience it. what's that again? oh right bodily-kinesthetic learning? I'm not even sure if that's correct). This will help you pick up concepts easily.
        - Know the time where your brain picks up concepts easily. I'm a night owl so studying at night really made me more efficient. Well now I work in a UK shift and it's around 3 pm to 12 am in the Philippines so my work takes all my efficiency period and I got to study less on my learning window.
        - Complete the CPTS Job role path in the HTB Academy then supplement it with hands-on experience by solving some labs. Whether active or retired, it doesn't matter. I prefer active machines because I won't be tempted in looking for writeups. I only need to trust myself and my methodology plus it forced me to research on things that I'm not familiar with.
        - Take some rest and make it a part of your training. Goku is the best example for this. Sometimes, grinding burns you out more and produces a negative impact than positive ones. You'll get stronger by taking a break and touching some grass. I just noticed it after the exam. This exam traumatized me a little that I felt like not touching a computer for a while and just be a farmer in the province lol. At least the crops wouldn't give me authentication errors. LOL.
        ![Goku Sleeping](https://github.com/user-attachments/assets/cdb873e7-d490-45df-8ec8-db10c235fedd) _Even Goku needs a recovery arc._

        - Take your time. Don't race with everyone else. Focus on your own timeline. It's one of the mistakes that I made. I compared my current level to other people's level 100. As mentioned in my background, I don't have any technical experience prior to this job. My colleagues are different. They have more experience and are skilled than I am. They can solve boxes in 2 hours that took me 4 to 8 hours to solve. They recognize patterns better than I do. They have better OpSec because some of them have red teaming experience. While yes, there might be a skill gap between you and other people and it's hard not to ignore it, it should fuel your burning passion and drive to reach their level but not to the point that you're burning yourself out. You won't reach their level overnight. But it's important to see your improvement compared to your day one. Yes it's cringy but it's real.
    
3. What's Next?
    I honestly don't know. I'm still figuring it out. But I guess, I'll get more real-world experience by delivering projects and shadow other consultants who possess expertise in other specializations like cloud and mobile. Since AI has been a buzz term for a while now, I guess I'll be doing the HTB COAE path. I'm really bad at Math and there are some computations in the COAE path, so I think it'll be funny to mock my previous Math teachers by passing this Certification. It'll be funny as someone without calculus background just casually passing an AI hacking certification but I guess it'll be challenging. and I'm up for that challenge. I'll do it for the plot lol.
4. Final Thoughts
	I honestly don't know what to say anymore. I guess if you're planning to take the CPTS, I guess go for it. Sometimes, you don't need to feel ready to take the exam, you'll have to experience it to know whether or not your skills are enough. Failing is scary but it's what makes it fun and leaves you with more lessons. I don't feel ready when I took it but I passed it on the first try. I'm still afraid to fail but in life, there's no real failed attempts. It's either you win or you earn lessons. IDK who said that I just said whatever comes to my mind. I sound like a martial arts master NGL hahaha. Anyway, good luck future candidates and I hope you get something from my nonsense.
![Bocchi Celebrating](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExdng1c2hpN3ZmYzFtbnFjajNpMzRrbzV1MG92dW5oczk0emQ1bnpraiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/pwWaY9rHspjc9lKzYI/giphy.webp)
![Certified Hacker](https://ci3.googleusercontent.com/meips/ADKq_NZjG70RwiEBSapwKZUBAvVMiZv4wMO_qfGfANXfV9082chPXRPf7iEe6vprqaRzBsI_pDFI46Aaxa2cYyJaZpsdix0dqWwcDIciAoqkuSMg6auwjYatVLIH435d8tmplyTClYeLPTXyZrKW9AwlN6EA04h8UA=s0-d-e1-ft#https://img.mailinblue.com/3579920/images/content_library/original/6230a30b3aacdf79ab772a1c.gif)

