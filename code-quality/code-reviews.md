## Code Reviews


𝙂𝙤𝙖𝙡𝙨 𝙤𝙛 𝙘𝙤𝙙𝙚 𝙧𝙚𝙫𝙞𝙚𝙬𝙨:

* Sharing knowledge
* Spreading ownership
* Unifying development practices
* Quality control

𝘞𝘩𝘦𝘯𝘦𝘷𝘦𝘳 𝘪𝘮𝘱𝘭𝘦𝘮𝘦𝘯𝘵𝘪𝘯𝘨 𝘤𝘩𝘢𝘯𝘨𝘦𝘴 𝘵𝘰 𝘸𝘢𝘺𝘴 𝘰𝘧 𝘸𝘰𝘳𝘬𝘪𝘯𝘨, 𝘪𝘵'𝘴 𝘢 𝘨𝘰𝘰𝘥 𝘪𝘥𝘦𝘢 𝘵𝘰 𝘦𝘯𝘴𝘶𝘳𝘦 𝘵𝘩𝘢𝘵 𝘦𝘷𝘦𝘳𝘺𝘰𝘯𝘦 𝘢𝘨𝘳𝘦𝘦𝘴 𝘰𝘯 𝘵𝘩𝘦 𝘱𝘳𝘰𝘤𝘦𝘴𝘴 𝘢𝘯𝘥 𝘩𝘢𝘴 𝘩𝘢𝘥 𝘵𝘩𝘦 𝘤𝘩𝘢𝘯𝘤𝘦 𝘵𝘰 𝘤𝘰𝘯𝘵𝘳𝘪𝘣𝘶𝘵𝘦 𝘵𝘰 𝘵𝘩𝘦 𝘥𝘦𝘤𝘪𝘴𝘪𝘰𝘯. 𝘛𝘩𝘪𝘴 𝘸𝘪𝘭𝘭 𝘤𝘢𝘶𝘴𝘦 𝘭𝘦𝘴𝘴 𝘧𝘳𝘪𝘤𝘵𝘪𝘰𝘯.

> Agree on the philosophy and motivation behind code reviews.
> Write down an internal "what's a good code review" document together.
> Refer to existing code review guides.

### Multiple perspectives to a code review process:
* author
* reviewer
* team


𝘽𝙚𝙨𝙩 𝙥𝙧𝙖𝙘𝙩𝙞𝙘𝙚𝙨 𝙛𝙤𝙧 𝙘𝙤𝙙𝙚 𝙧𝙚𝙫𝙞𝙚𝙬𝙨

𝗙𝗼𝗿 𝘁𝗵𝗲 𝗧𝗲𝗮𝗺:
1. Create pull request guidelines everyone can follow easily. Discuss whether the author or reviewer is responsible for which activity, as well as what to do during each step of the review process.
2. Create a checklist for the standards that you'd like to focus on during the review.
* *Functionality*: Does it behave as expected?
* *Software Design*: Does the code fit the rest of the code base?
* *Complexity*: Is the code easy to understand for other devs?
* *Tests*: Does the code include the proper tests?
* *Naming*: Are names for variables, functions, etc. descriptive?
* *Comments*: Are the comments clear and useful?
* *Documentation*: Did the author also update the  relevant docs?
3. Get the team to agree on the items in 1. and 2. above.
4. Decide on the team’s preferred channels to communicate certain information, whether it's email, chat, the PR thread, etc.
5. Use the shared repository model. Collaborators are granted push access to a single shared repository and topic branches are created when changes need to be made.
6. Invest in setting up a continuous integration  solution to automate as many quality checks as possible.They can provide additional data for the review process.
7. Convert linting, spacing and other rules about details into automated checks. Consider using the Prettier defaults for Javascript, for example.
8. Consider creating a PR templates for authors to standardize parts of the descriptions.

𝗙𝗼𝗿 𝗔𝘂𝘁𝗵𝗼𝗿𝘀: 
1. Make sure that complex and/or important stories and features are discussed beforehand to avoid rewrites after the PR. Consider creating a PoC or drawing a diagram as your first draft PR.
2. Before submitting a PR for a review, go through the changes yourself. This helps to catch accidentally included changes, typos, and other simple mistakes that potentially waste the reviewer's time.
3. Keep pull requests small. If your stories usually take a day's work, pull requests can be based on them to keep them small. Or slice it into tasks if it still feels large. 
4. Utilize feature flags to gain the ability to ship half-ready product features along with the existing ones.
5. Write clear PR descriptions. Additional details often include information such as what setup is needed to test the PR, surprising implementation details, and anything that makes the reviewer's job smoother.
6. A demo in any visual form is a nice touch. The format can be a screenshot, a screen capture, terminal output pasted in a code block, or anything that captures the change well. 
7. Document the PR discussion in code. Feel free to write comments. Add a summary of any face-to-face discussion as a PR comment (can be done by either author or reviewer). 

𝗙𝗼𝗿 𝗥𝗲𝘃𝗶𝗲𝘄𝗲𝗿𝘀:
1. Reviewers should minimize the response lag to the author. Tell the author when they can expect their code to be reviewed, whether that's the next hour or the next day.
2. Dev shouldn't interrupt their focus to do reviews.
3. Have a bias for action. If a tech decision lingers and work becomes blocked, deciding something relatively quickly is better than slowly concluding to an "ideal" decision. Be inclined to merge code instead of nitpicking.
4. Foster a positive feedback culture. Some ways to do this:
  * Give feedback about the code, not about the author. 
  * Accept that there are multiple correct solutions to a problem.
  * Provide reasons, not feelings, to support your position.
  * Use the "Yes, and..." technique to keep an innovative atmosphere.
  * Don't dismiss fresh and fragile ideas in a draft PR stage.
  * Keep the feedback balanced with positive comments. It's always delightful to receive praise from the reviewer.
5. When reviewing a piece of code, be explicit about the action you request from the author.
6. Make sure reviews are done evenly by all developers instead of siloing reviews to a single person.
7. If possible, pull the code change into your local dev environment and test it manually. 


**References**:  
- https://www.swarmia.com/blog/a-complete-guide-to-code-reviews/



