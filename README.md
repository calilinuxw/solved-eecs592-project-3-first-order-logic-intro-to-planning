Download Link: https://assignmentchef.com/product/solved-eecs592-project-3-first-order-logic-intro-to-planning
<br>
Please take care to complete all parts of this project independently.  Do not use any solutions found online or written by other students.  If you are struggling please go to office hours, post to Piazza, and/or send us email.  Please submit a single PDF file project3.pdf to Canvas.  The PDF file can contain a scan of handwritten or typewritten/typeset solutions, and any supporting graphics.

<ol>

 <li><strong>R&amp;N Problem 8.10: </strong></li>

</ol>

Consider a vocabulary with the following symbols:

<em>Occupation(p, o): </em>Predicate. Person <em>p</em> has occupation <em>o</em>.

<em>Customer (p1,p2)</em>: Predicate. Person <em>p1</em> is a customer of person <em>p2</em>.

<em>Boss(p1,p2): </em>Predicate. Person <em>p1</em> is a boss of person <em>p2</em>.

<em>Doctor , Surgeon, Lawyer , Actor: </em>Constants denoting occupations.  <em>Emily, Joe:</em> Constants denoting people.

Use these symbols to write the following assertions in first-order logic:

<ol>

 <li>Emily is either a surgeon or a lawyer.</li>

 <li>Joe is an actor, but he also holds another job.</li>

 <li>All surgeons are doctors.</li>

 <li>Joe does not have a lawyer (i.e., is not a customer of any lawyer).</li>

 <li>Emily has a boss who is a lawyer.</li>

 <li>There exists a lawyer all of whose customers are doctors.</li>

 <li>Every surgeon has a lawyer.</li>

</ol>




<ol start="2">

 <li><strong>R&amp;N Problem 8.20:</strong></li>

</ol>

Arithmetic assertions can be written in first-order logic with the predicate symbol &lt;, the function symbols + and *, and the constant symbols 0 and 1.  Additional predicates can also be defined with biconditionals.

<ol>

 <li>Represent the property “x is an even number.”</li>

 <li>Represent the property “x is prime.”</li>

 <li>Golbach’s conjecture is the conjecture (unproven as yet) that every even number is equal to the sum of two primes. Represent this conjecture as a logical sentence.</li>

</ol>

<em> </em>

<ol start="3">

 <li><strong>R&amp;N Problem 9.6: </strong></li>

</ol>

Write logical representations for the following sentences, suitable for use with Generalized Modus Ponens:

<ol>

 <li>Horses, cows, and pigs are mammals.</li>

 <li>An offspring of a horse is a horse.</li>

 <li>Bluebeard is a horse.</li>

 <li>Bluebeard is Charlie’s parent.</li>

 <li>Offspring and parent are inverse relations.</li>

 <li>Every mammal has a parent.</li>

</ol>




<ol start="4">

 <li><strong>R&amp;N Problem 9.13: </strong>  In this exercise, use the sentences you wrote in Exercise 9.6 (Problem 4 of this assignment) to answer a question by using a backward-chaining algorithm.

  <ol>

   <li>Draw the proof tree generated by an exhaustive backward-chaining algorithm for the query ∃<em> h Horse(h)</em>, where clauses are matched in the order given.</li>

   <li>What do you notice about this domain?</li>

   <li>How many solutions for <em>h</em> actually follow from your sentences?</li>

   <li>Can you think of a way to find all of them? (Hint: See Smith et al. (1986) – R&amp;N bibliography.)</li>

  </ol></li>

</ol>




<ol start="5">

 <li><strong>R&amp;N Problem 9.23:</strong>  From “Horses are animals,” it follows that “The head of a horse is the head of an animal.”  Demonstrate that this inference is valid by carrying out the following steps:</li>

 <li>Translate the premise and the conclusion into the language of first-order logic. Use three predicates: <em>HeadOf(h,x)</em> (meaning “<em>h</em> is the head of <em>x</em>”), <em>Horse(x)</em>, and <em>Animal(x).</em></li>

</ol>




<ol start="6">

 <li><strong>Write the following statements in first-order logic. Complete all steps of FOL resolution to prove the conclusion: </strong>

  <ol>

   <li>All hounds howl at night.</li>

   <li>Anyone who has any cats will not have any mice.</li>

   <li>Light sleepers do not have anything that howls at night.</li>

   <li>Sam has either a cat or a hound.</li>

   <li>(Conclusion) If Sam is a light sleeper, then Sam does not have any mice.</li>

  </ol></li>

 <li><strong>Write the following statements in first-order logic. Complete all steps of FOL resolution to prove the conclusion: </strong>

  <ol>

   <li>Everyone who feels warm either is drunk, or every costume they have is warm.</li>

   <li>Every costume that is warm is furry.</li>

   <li>Every AI student is a CS student.</li>

   <li>Every AI student has some robot costume.</li>

   <li>No robot costume is furry.</li>

   <li>(Conclusion) If every CS student feels warm, then every AI student is drunk.</li>

  </ol></li>

 <li><strong>Write the following statements in first-order logic. Complete all steps of FOL resolution to prove the conclusion: </strong>

  <ol>

   <li>Every child loves every candy.</li>

   <li>Anyone who loves some candy is not a nutrition fanatic.</li>

   <li>Anyone who eats any pumpkin is a nutrition fanatic.</li>

   <li>Anyone who buys any pumpkin either carves it or eats it.</li>

   <li>Stuart buys a pumpkin.</li>

   <li>Lifesavers is a candy.</li>

   <li>(Conclusion) If Stuart is a child, then Stuart carves some pumpkin.</li>

  </ol></li>

 <li><strong>R&amp;N 10.2 (Flying) </strong>(5 points)</li>

</ol>

Given the action schemas and initial state from R&amp;N Figure 10.1 (reproduced below), what are all the applicable concrete instances of <em>Fly(p, from, to)</em> in the state described by:




<em>At(P1, JFK ) </em>∧<em> At(P2, SFO) </em>∧<em> Plane(P1) </em>∧<em> Plane(P2) </em>∧<em> Airport(JFK ) </em>∧<em> Airport(SFO) </em>

<ol start="10">

 <li><strong>R&amp;N 10.4 (Shakey the Robot)  </strong></li>

</ol>

The original STRIPS planner was designed to control Shakey the robot.  Figure 10.14 (from R&amp;N, reproduced below) shows a version of Shakey’s world consisting of four rooms lined up along a corridor, where each room has a door and a light switch.  The actions in Shakey’s world include moving from place to place, pushing movable objects (such as boxes), climbing onto and down from rigid objects (such as boxes), and turning light switches on and off.  The robot itself could not climb on a box or toggle a switch, but the planner was capable of finding and printing out plans that were beyond the robot’s abilities.  Shakey’s six actions are the following:

<ul>

 <li><em>Go(x,y,r),</em> which requires that Shakey be <em>At</em> <em>x</em> and that <em>x</em> and <em>y</em> are locations <em>In</em> the same room <em>r</em>. By convention a door between two rooms is in both of the rooms.</li>

 <li><em>Push(b,x,y,r):</em> Push a box <em>b</em> from location <em>x</em> to location <em>y</em> within the same room You need the predicate <em>Box</em> and constants for the boxes.</li>

 <li><em>ClimbUp(x,b):</em> Climb onto a box <em>b</em> from position <em>x</em>; requires predicate <em>On(x,y)</em> (<em>x</em> is on <em>y</em>) and constant <em>Floor</em>.</li>

 <li><em>ClimbDown(b,x):</em> Climb down from a box <em>b</em> to position <em>x</em>.</li>

 <li><em>TurnOn(s,b), TurnOff(s,b):</em> Turn a light switch <em>s</em> on (or off).  To successfully achieve a light switch action, Shakey must be on top of a box <em>b</em> at the light switch’s location (room).</li>

</ul>

Write PDDL sentences for Shakey’s six actions and the initial state from Figure 10.14.  Manually construct a plan for Shakey to get <em>Box2</em> into <em>Room2</em>.





