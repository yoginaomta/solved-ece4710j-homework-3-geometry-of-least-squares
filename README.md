Download Link: https://assignmentchef.com/product/solved-ece4710j-homework-3-geometry-of-least-squares
<br>
<h1>Geometry of Least Squares</h1>

<ol>

 <li>Suppose we have a dataset represented with the design matrix span(X) and response vector Y. We use linear regression to solve for this and obtain optimal weights as <em>✓</em>ˆ. Draw the geometric interpretation of the column space of the design matrix span(X), the response vector Y, the residuals Y X<em>✓</em>ˆ, and the predictions X<em>✓</em>ˆ(using optimal parameters) and X<em>↵ </em>(using an arbitrary vector <em>↵</em>).</li>

</ol>

<ul>

 <li>What is always true about the residuals in least squares regression? Select all that apply.</li>

</ul>

⇤ A. They are orthogonal to the column space of the design matrix.

⇤ B. They represent the errors of the predictions.

⇤ C. Their sum is equal to the mean squared error.

⇤ D. Their sum is equal to zero. ⇤ E. None of the above.

1

<ul>

 <li>Which are true about the predictions made by OLS? Select all that apply.</li>

</ul>

⇤ A. They are projections of the observations onto the column space of the design matrix.

⇤ B. They are linear combinations of the features.

⇤ C. They are orthogonal to the residuals.

⇤ D. They are orthogonal to the column space of the features.

⇤ E. None of the above.

<ul>

 <li>We fit a simple linear regression to our data (<em>x<sub>i</sub>,y<sub>i</sub></em>)<em>,i </em>= 1<em>,</em>2<em>,</em>3, where <em>x<sub>i </sub></em>is the independent variable and <em>y<sub>i </sub></em>is the dependent variable. Our regression line is of the form <em>y</em>ˆ = <em>✓</em>ˆ<sub>0 </sub>+<em>✓</em>ˆ<sub>1</sub><em>x</em>. Suppose we plot the relationship between the residuals of the model and the <em>ys</em>ˆ , and find that there is a curve. What does this tell us about our model?</li>

</ul>

⇤ A. The relationship between our dependent and independent variables is well represented by a line.

⇤ B. The accuracy of the regression line varies with the size of the dependent variable.

⇤ C. The variables need to be transformed, or additional independent variables are needed.

3

<h1>Understanding Dimensions</h1>

<ol start="2">

 <li>In this exercise, we will examine many of the terms that we have been working with in regression (e.g. <em>✓</em>ˆ) and connect them to their dimensions and to concepts that they represent.</li>

</ol>

First, we define some notation. The <em>n</em>⇥<em>p </em>design matrixX hasX corresponds to<em>p</em>+1 features, where the addition<em>n </em>observations on <em>p </em>features. (In lecture, we stated that we sometimes say

feature is a column of all 1s for the intercept term, but strictly speaking that column doesn’t need to exist. In this problem, one of the <em>p </em>columns <em>may </em>be a column of all 1s.) Y is the response variable. It is a vector, containing the true response for all observations. We assume in this problem that we use X and Y to compute optimal parameters <em>✓</em>ˆfor a linear model, and that this linear model generates predictions using Yˆ = X<em>✓</em>ˆ as we saw in lecture and in Question 1 of this discussion. Each of the <em>n </em>rows in our design matrix X contains all features for a single observation. Each of the <em>p </em>columns in our design matrix X contains a single feature, for all observations. We denote the rows and columns of X as follows:

X:<em><sub>,j   </sub></em><em>j<sup>th </sup></em>column vector in X<em>,j </em>= 1<em>,…,p </em>X<em>i,</em><sub>:                       </sub><em>i<sup>th </sup></em>row vector in X<em>,i </em>= 1<em>,…,n</em>

Below, on the left, we have several expressions, labelled a through h, and on the right we have several terms, labelled 1 through 10. For each expression, determine its shape (e.g., <em>n</em>at all. If a specific expression is nonsensical because the dimensions don’t line up for a matrix⇥ <em>p</em>), and match it to one of the given terms. Terms may be used more than once or not multiplication, write “N/A” for both.

<table width="460">

 <tbody>

  <tr>

   <td width="266">(a)    X(b)    <em>✓</em>ˆ(c)     X:<em><sub>,j</sub></em>(d)    X1<em><sub>,</sub></em><sub>: </sub>· <em>✓</em>ˆ(e)    X:<em><sub>,</sub></em><sub>1 </sub>· <em>✓</em>ˆ(f)      X<em>✓</em>ˆ(g)    (X<em><sup>T </sup></em>X) <sup>1</sup>X<em><sup>T </sup></em>Y</td>

   <td rowspan="2" width="194">1.    the residuals2.    03.    1st response, <em>y</em><sub>1</sub>4.    1st predicted value, <em>y</em>ˆ<sub>1</sub>5.    1st residual, <em>e</em><sub>1</sub>6.    the estimated coefficients7.    the predicted values</td>

  </tr>

  <tr>

   <td width="266">(h) (<em>I </em>X(X<em><sup>T </sup></em>X) <sup>1</sup>X<em><sup>T </sup></em>)Y</td>

  </tr>

 </tbody>

</table>

<ol start="8">

 <li>the features for a single observation</li>

 <li>the value of a specific feature for all observations</li>

 <li>the design matrix</li>

</ol>

As an example, for 2a, you would write: “2a. Dimension: <em>n </em>⇥ <em>p</em>, Term: 10”.