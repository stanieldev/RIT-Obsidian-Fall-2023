
https://mycourses.rit.edu/d2l/le/content/1044537/viewContent/9378289/View
[https://mail.google.com/mail/u/0/#inbox/KtbxLvHPwVmTSkWPRbRsghhcRDWMBkWJhg](https://mail.google.com/mail/u/0/#inbox/KtbxLvHPwVmTSkWPRbRsghhcRDWMBkWJhg)



### The Conflict Between Physics and Computer Science
- Explore the specific challenges arising from the clash between physics and computer science notation.
- Provide examples illustrating the differences and potential sources of confusion.
- We’re exploring notations that could actually be in the same problem. Not like Big O notation.

Typical notation for wavefunctions of state are represented as binary indices.
$$\ket{\psi} = \psi^{ijk\dots}\ket{i}\ket{j}\ket{k}\dots = \psi^{ijk\dots}\ket{ijk\dots}$$
Computer science has a representation for binary strings like the following
$$i,j,k = b \implies \ket{\psi} = \psi^b \ket{b}$$
Problem arises when you take the product of 2 binary states.
For physics, the result is pretty simple, but CS has a few problems.


#### Binary Notation
For a set of objects that have binary states in quantum mechanics, the typical notation is:
$$\ket{\psi} = \psi^{ijk\dots}\ket{i}\ket{j}\ket{k}\dots = \psi^{ijk\dots}\ket{ijk\dots}$$
The concatenation of ijk is a shorthand for a state with each index.

Using a concept from Computer Science called a "Binary String", we can rewrite the wavefunction as:
$$\ket{\psi} = \psi^b \ket{b}$$
This is only possible due to group homeomorphisms outside the scope of this paper.

**Where the conflict arises:**

The dual vector of $\psi$ has a reverse order of bits relative to is vector.
This is because of the order of decomposition of covectors under a tensor product.
CS removes this problem, but a new one comes after.

When you want to concatenate 2 binary strings in CS, you have to extend the originals bits.
$$\ket{\phi} = \phi^b \ket{b}, \ket{\psi} = \psi^b \ket{b} \implies \ket{\phi}\ket{\psi} = \phi^{b_1}\psi^{b_2} \ket{b_1}\ket{b_2}$$
For CS students, the concatenation makes sense since binary strings are a very common occurrence.
This isn't the case for physics, as there's no reason to break it down.


#### Oplus and Otimes
















### The Messy Landscape of Quantum Computing Notation
- Discuss the inherent messiness of quantum notation due to the novelty of the field.
- Highlight instances where notation has evolved or is still evolving, contributing to confusion.
### Strategies for Teaching Quantum Computing
- Outline effective teaching strategies to address the challenges posed by ambiguous notation.
- Emphasize the importance of a holistic approach that integrates both physics and computer science perspectives.
### Curriculum Design for Quantum Computing Education
- Present a detailed curriculum for teaching quantum computing.
- Include specific topics, milestones, and suggested learning outcomes.
### Implementation Examples
- Provide real-world examples of how the proposed curriculum can be implemented in educational settings.
- Discuss case studies or success stories from institutions that have navigated the quantum computing education landscape effectively.
### Conclusion
- Summarize key findings from the paper.
- Emphasize the importance of addressing notation ambiguity in quantum computing education.
- Provide recommendations for future research and educational practices.
### References














### Notes
Representation of Quantum States is taken directly from physics.
$$\ket{\psi} = \psi^{ijk\dots}\ket{i}\ket{j}\ket{k}\dots = \psi^{ijk\dots}\ket{ijk\dots}$$
Writing the shorthand for vector tensor products looks like binary representation in classical computing, and so it's common to rewrite the above as:
$$\ket{\psi} = \psi^{b}\ket{b}$$
Where the $b$ here stands for the bit representation of the state.

During this exchange, the tensor goes from a (n, 0) tensor with 2 states each to a (1, 0) tensor with 2^n states.










### Timeline
1.  **Short Concept** (Due Friday 11/17). A 4-6 sentence summary of your idea. 
2. **Written rough draft** (Due Thursday 12/7). A 4-6 page _rough_ draft of your report.
3. **Oral presentation** (Due Thursday 12/14, 8 AM). You will present this during our final exam slot on Thursday 12/14 from 8-10:30 am  (Note we can shift the exam time later in the day if everyone agrees on a new time).
4. **Written report** (Due Thursday 12/14). Final version due at the end of the day.


### Paper Details
**Big idea: Select one or more readings and apply them to some innovation or reform. I want you to have fun applying concepts or ideas you found interesting to some physics education context you are excited about.**

**You will develop a written and oral version of your proposal.** 
- **Written** form: A 4-6 page paper 
- **Oral** presentation: A 10 minute presentation (with slides) + 5 minutes for discussion. 
- It is expected the content will be similar between oral and written. 

#### Criteria:
1. **Identify key ideas from the literature that you want to apply  (1+ page)**
	1. Provide clear definitions.
	2. Provide appropriate references. 
	3. The description should be thorough enough that someone not in this class could understand the basic ideas of what you are thinking about.
2. **Describe the educational situation where you want to apply this idea. (0.5+ page)**
	1. What “scale” is your concept? A single assignment/activity? A lesson within a course? A unit? A whole course? A program? An outreach event? Or something else?
	2. What student population would participate or benefit from this development? 
	3. What particular physics topic(s) or course would this impact? 
	4. Why would this situation benefit from the application of this idea?
3. **Propose innovation or reform in physics education (1.5+ pages)**
	1. In light of the ideas from the literature, what innovation or reform are you proposing? 
	2. Provide a rich description of your idea
		1. What are the goals? What outcomes? (Measurable/observable results)
			1. [Bloom’s Taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/) Verbs are helpful ([example list of verbs](https://www.utica.edu/academic/Assessment/new/Blooms%20Taxonomy%20-%20Best.pdf))
		2. How does it employ the idea from the literature? 
		3. If appropriate, provide a schedule, lesson plan, or outline? 
		4. Provide examples. 
	3. After the reader finishes this section, they should have a good picture in your head of what you are planning and why it is innovative. 
4. **Propose assessment and research (1.5+ page)**
	1. What research question(s) could you ask related to your innovation or reform? These questions may relate to the goals for your project. 
	2. What data would you collect? (student work, interviews, observations, surveys, etc).  
	3. Within your chosen data collection method, describe what evidence you would be looking for. For example, if collecting student work, what  would the task be and how would you analyze it? If doing interviews, what task or questions would the participant be asked to do? 
	4. Who would your participants be? How many participants? (keep in mind not everyone who takes part as a student needs to be part of the research study)
	5. How would this research be useful in improving your educational plans or your understanding of how learning works?