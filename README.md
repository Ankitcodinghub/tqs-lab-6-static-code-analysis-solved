# tqs-lab-6-static-code-analysis-solved
**TO GET THIS SOLUTION VISIT:** [TQS Lab 6-Static Code analysis Solved](https://www.ankitcodinghub.com/product/tqs-lab-6-static-code-analysis-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93896&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;TQS Lab 6-Static Code analysis Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 16">
<div class="layoutArea">
<div class="column">
Lab 6 Static Code analysis (with SonarQube)

Context and key points

Key Points

Static code quality can assess a code base to produce quality metrics. These metrics are based on the occurrence of known weaknesses. In this kind of analysis, the solution is not deployed, nor the code is executed (thus the name static analysis).

Static code analysis can be run locally using a “linter” and modern IDE will typically include support for code inspection. But it would be even more import to implement code analysis in the team develop infrastructure, i.e., at the continuous integration pipeline, using specialized services.

Key code quality measures include the occurrence of problems likely to produce errors, vulnerabilities (security/reliability concerns) and code smells (bad/poor practice or coding style); coverage (ratio tested/total); and code complexity assessment.

The estimated effort to correct the vulnerabilities is called the technical debt. Every software quality engineer needs tools to obtain realistic information on the technical debt.

Explore

<ul>
<li>⎯ &nbsp;Use the SonarQube to inspect a project of your own, maybe from another course. Note that free analyzers are not available for all languages.</li>
<li>⎯ &nbsp;public projects on Sonar cloud that you can browse and learn.</li>
</ul>
6.1 Local analysis

<ol>
<li>a) &nbsp;Select/copy a Maven-based, Java application project to use. You may reuse one from previous labs, for example, the Euromillions from Lab 1.2 (with tests passing).</li>
<li>b) &nbsp;Prepare a local instance of SonarQube (using the Docker image). For this lab, you do not need to configure a production database (an embedded database is used by default; for a production scenario, a more demanding configuration is required).
Note1: you may get a conflict on port 9000 in your host, as it is also commonly picked for other services (e.g.: Portainer).
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
16 | TQS LABS

</div>
</div>
</div>
<div class="page" title="Page 17">
<div class="layoutArea">
<div class="column">
45426 Teste e Qualidade de Software

Note2: there are known problems to run the provided docker image on Mac M1 (Apple Silicon).

Consider the following alternatives: use the .zip file version; use an alternative docker image.

c) Confirm that you can access the dashboard (default : http://127.0.0.1:9000) and change the default

credentials (admin / admin).

<ol start="4">
<li>d) &nbsp;Complete the “Analyzing a Project steps”: create a project “manually”; set for “local analysis”; generate a named token. Take note of the generated user token! You will need it later several times.</li>
<li>e) &nbsp;Recommended practice: lock the sonar plugin version in your POM (“Fix version of Maven Plugin”).</li>
</ol>
From the command line, run the code analysis (highlighted parts should be adapted as needed):

$ mvn verify sonar:sonar -Dsonar.host.url= -Dsonar.projectKey=lab6_1 -Dsonar.login=

Note: optionally, you can save part of the Sonar configuration as “global settings”.

</div>
</div>
<div class="layoutArea">
<div class="column">
f)

</div>
<div class="column">
Confirm that Sonar analysis ran in the build. Access the SonarQube dashboard (default : http://127.0.0.1:9000).

Has your project passed the defined quality gate? Elaborate your answer (in Readme document/markdown file, along with the code project).

</div>
</div>
<div class="layoutArea">
<div class="column">
g)

Issue

Bug

Vulnerability

Code smell (major)

</div>
</div>
<div class="layoutArea">
<div class="column">
Explore the analysis results and complete with a few sample issues, as applicable. (Place your response in a Readme file, either html/md/pdf…).

</div>
</div>
<div class="layoutArea">
<div class="column">
Problem description How to solve

… …

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>http://localhost:9009
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>053bd3d423525e6df97b6bfd06b8a7ecd5bb7e
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
TQS LABS | 17

</div>
</div>
</div>
<div class="page" title="Page 18">
<div class="layoutArea">
<div class="column">
6.2 Technicaldebt(Cars)

Make a copy of the “Cars” project from Lab #3.2.

Be sure you are using a project with JUnit tests implemented and passing.

<ol>
<li>a) &nbsp;Analyze this project with SonarQuebe. Remember to create a new project in your Sonar instance. Take note of the technical debt found. Explain what this value means.

Document the analysis findings with a print screen (of the sonar dashboard for this project).</li>
<li>b) &nbsp;Analyze the reported problems and be sure to correct the severe code smells reported (critical and major).
Note: if you used the Entity data type as parameter in the API methods, you will likely get the vulnerability “Persistent entities should not be used as arguments”.
</li>
<li>c) &nbsp;Code coverage reports require an additional plugin. Be sure to use a project with unit tests and configured code coverage (e.g.: add the jacoco plugin to maven and update the plugin version).</li>
<li>d) &nbsp;Run the static analysis and observe/explore the coverage values on the SonarQube dashboard. How many lines are “not covered”? And how many conditions?</li>
</ol>
6.3 Custom QG

For this exercise, it would appropriate to use a larger project. Consider using the group project from IES5. Alternatively, you may get an open-source project (maven-based, Java project). Otherwise, continue with the project from previous exercise.

Note: do not to submit this project to your Git! Focus on providing evidence that you complete the tasks and discuss the outcomes.

a) If possible, collaborate with other colleagues to define a custom quality gate to this project (especially if you are using the IES project, try to work with the development team from then).

Feel free to mix the metrics but explain your chosen configuration.

b) Add an increment to the source code. You may try to introduce some “bad smells”; in fact, try to break the quality gate.

Run the analysis and analyze the results.

6.4 IDE

[Optional. No submission required.]

In the previous tasks, we assume the static code analysis as a service, likely to be integrated at the Continuous Integration pipeline. You will, however, also benefit from having code inspection as you develop, automatically integrated in the IDE.

5 More specifically, the backend/API subproject, if applicable.

</div>
</div>
<div class="layoutArea">
<div class="column">
18 | TQS LABS

</div>
</div>
</div>
<div class="page" title="Page 19">
<div class="layoutArea">
<div class="column">
45426 Teste e Qualidade de Software

</div>
</div>
<div class="layoutArea">
<div class="column">
a)

b)

Lab 7

</div>
<div class="column">
IntelliJ (and most IDE) already integrates a code inspection tool. If you have not used before, try it.

The Sonar Qube analysis can be integrated in IntelliJ through the SonarLint plug-in.

Integration tests (Test Containers, REST Assured)

</div>
</div>
<div class="layoutArea">
<div class="column">
Note that:

<div class="page" title="Page 19">
<div class="layoutArea">
<div class="column">
IntelliJ (and most IDE) already integrates a code inspection tool. If you have not used before, try it.

The Sonar Qube analysis can be integrated in IntelliJ through the SonarLint plug-in.

</div>
</div>
</div>
</div>
</div>
</div>
