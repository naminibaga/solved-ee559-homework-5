Download Link: https://assignmentchef.com/product/solved-ee559-homework-5
<br>
<ol>

 <li>For 2-class perceptron <em>with margin</em> algorithm, using basic sequential GD, fixed increment, prove convergence for linearly separable training data by modifying the perceptron convergence proof covered in class. You may write out the proof, or you may take the 3-page proof from the posted handout (or from lecture), and mark up the proof to show all changes as needed.  If you mark up the existing proof, be sure to mark everything that needs changing (<em>g.</em>, if a change propagates through the proof, be sure to make all changes for a complete answer).</li>

 <li>You are given the following training data points in three pattern classes <em>S</em><sub>1</sub>, <em>S</em><sub>2</sub>, and <em>S</em><sub>3</sub>:</li>

</ol>

<h1>                   <em> </em>{(0,1,−1,2)}∈<em>S</em><sub>1</sub>; {(1,1,1,1),(2,1,1,1)}∈<em>S</em><sub>2</sub>; {(−1,1,0,−1)}∈<em>S</em><sub>3</sub></h1>

Note that in our notation (throughout this class), for convenience we can write (<em>x</em><sub>1</sub>,<em>x</em><sub>2</sub>,<em>x</em><sub>3</sub>,<em>x</em><sub>4</sub>) with commas, to denote a column vector (of dimension 4 in this case).

<ul>

 <li>Find linear discriminant functions that correctly classify the training data, using the multiclass Perceptron algorithm using maximal value method (given in Discussion 6 and in the posted handout). Use augmented space (so first augment the data).  There are few enough iterations that this can be done by hand, or you may write code to do it if you prefer.</li>

</ul>

<strong>Use the following assumptions and starting point.</strong>  Assume the data points have already been shuffled, so use the training data in the order given above.  Use η(<em>i</em>)= 1  ∀<em>i</em>,  and initial weight vectors:

<em> </em>

<em><u>w</u></em><sup>(1)</sup>(0)=−<u>1</u>,     <em><u>w</u></em><sup>(2)</sup>(0)=<u>1</u>,    <em><u>w</u></em><sup>(3)</sup>(0)= <u>0</u>.

<em> </em>

<ul>

 <li>From this 5-dimensional feature space, consider points that lie in the plane <em>P</em> defined by all <em><sub> </sub><u>x</u></em> such that  <em><u>x</u></em>=(1,<em>x</em><sub>1</sub>,<em>x</em><sub>2</sub>,0,0). Give the decision rule for points <em><sub> </sub></em>(<em>x</em><sub>1</sub>,<em>x</em><sub>2</sub>) that lie in this plane. Plot in 2-space, the decision boundaries and decision regions in plane <em> P </em>.</li>

</ul>

<ol start="3">

 <li><em>Widrow-Hoff learning</em>. Starting from the MSE criterion function, derive a learning algorithm using the basic sequential gradient descent technique, as follows:</li>

</ol>

<ul>

 <li>Find an expression for <em>J</em><em><sub>n</sub></em>(<em><u>w</u></em>) and from that derive an expression for ∇<em><u><sub>w </sub></u></em><em>J</em><em><sub>n</sub></em>(<em><u>w</u></em>) .</li>

 <li>Complete the derivation to get the sequential gradient descent algorithm based on MSE. Your algorithm should be stated as a set of statements and forumulas and should include:  any random shuffling of the data, what is allowed for initializatin of <em><u>w</u></em>(0), weight update formula, any restriction on <sup>η</sup>(<em>i</em>), and any formula relating the iteration index <em>i</em> to the data point index <em>n</em>.  You may omit a halting condition because that isn’t part of this homework problem.</li>

</ul>

<strong>Hint:</strong>  Note that if your weight update formula has a positive constant (call it <em>a</em>) that multiplies by η(<em>i</em>), you may set η′(<em>i</em>)=<em>a</em>η(<em>i</em>) and then drop the prime, to simplify your final formula.

<ol>

 <li>1 of 1</li>

</ol>