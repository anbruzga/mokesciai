<h1>Mokesciai Application</h1>

<p>
  <strong>Mokesciai</strong> is a basic Java Swing application designed for utility cost calculation across multiple units. 
  The application is quite hardcoded, with predefined unit areas and a focus on shared cost distribution.
</p>

<h2>Features</h2>
<ul>
  <li>Calculates gas, electricity, and water costs for up to four units.</li>
  <li>Displays per-unit cost breakdown and total cost.</li>
  <li>Validates inputs and highlights errors.</li>
</ul>

<h2>Notes</h2>
<ul>
  <li>The user interface was built using <strong>NetBeans IDE</strong>. Any changes to the layout should be done via the NetBeans Form Editor.</li>
  <li>Many elements, such as unit sizes and default values, are hardcoded for simplicity.</li>
</ul>

<h2>Calculation Formula</h2>
<p>The application uses the following formula to calculate gas costs for each unit:</p>
<pre>
Gas Cost for Unit = (Total Gas Cost for All Units × Unit Area / Total Area)
                  + (Gas for Cooking / Number of Units)
                  + (Service Fee / Number of Units)
</pre>
<p>Where:</p>
<ul>
  <li><strong>Total Gas Cost for All Units</strong>: (Gas Used × Gas Price) - Gas for Cooking</li>
  <li><strong>Gas for Cooking</strong>: Fixed value of 20, shared equally among all units.</li>
  <li><strong>Unit Area</strong>: The area of the specific unit (e.g., 9.93, 15.69, etc.).</li>
  <li><strong>Total Area</strong>: Sum of all unit areas.</li>
</ul>

<h3>Electricity and Water Costs</h3>
<p>The costs for electricity and water are shared equally among all units:</p>
<pre>
Electricity or Water Cost per Unit = Total Electricity or Water Cost / Number of Units
</pre>

<h3>Total Cost</h3>
<p>The total cost for each unit includes gas, electricity, and water:</p>
<pre>
Total Cost for Unit = Gas Cost for Unit + Electricity Cost per Unit + Water Cost per Unit
</pre>
<h2>Usage</h2>
<ol>
  <li>Run the application via NetBeans or the command line:</li>
  <pre><code>
    javac com/bruzga/antanas/mokesciai/Mokesciai.java
    java com.bruzga.antanas.mokesciai.Mokesciai
  </code></pre>
  <li>Input utility details (e.g., gas consumption and price, service fees).</li>
  <li>Click <strong>Skaiciuoti</strong> to calculate and view results.</li>
</ol>

<h2>Development</h2>
<p>
  This project is hardcoded and designed for personal use. Contributions or extensions may require significant customization.
</p>

<h3>Example1:</h3>
<img src="https://github.com/user-attachments/assets/2839ed99-3277-4c5f-974c-57c6a559938f" alt="Application Screenshot" width="600">
<br>

<h3>Example2:</h3>
<img src="https://github.com/user-attachments/assets/320eea81-c513-4d1e-a0be-1ed079e8a24c" alt="Application Screenshot" width="600">
