
<figure>
 <img src="./assets/images/OWASP_Project_Header.png" title="SCAT" alt="SCAT" width="800" />
  <figcaption>Process integrity tool</figcaption>
</figure>

<table>
<tbody>
<tr class="odd">

<p>
  <a href="https://www.linkedin.com/pulse/secure-code-assurance-tool-scat-version-20-michael-bergman/">For more information on the <b>why</b> behind the SCAT, read my linkedIn Article here.</a>
</p>
<h2>What is the SCAT</h2>
* SCAT is a process integrity tool, its objective is to implementing a Software development process that is consistent, authorized and auditable
<li>SCAT is used by development teams to build, verify and assure secure software
<li><strong>Build</strong>: uses a combination of code level guidance and on demand training to clearly define the security requirments before development begins and guide software developers towards its correct implementation</li>
<li><strong>Verify</strong>: uses a combination of manual test plans and SATS tools to guide and verify correct implementation</li>
<li><strong>Assure</strong>: centrally stores and publishes evidence of secure development and testing as an audit trail. Providing traceability through requirements and proving that security controls operate efficiently over a period of time.</li>
</li>
<li>SCAT is <strong>not a point in time security verification tool </strong>for detecting vulnerabilities after development</li>

<h2>Process integrity and point in time tools: How they work in the SDLC</h2>
<figure>
<img src="/assets/images/Process_integrity_VS_point_in_time_without_check.png" title="Process_integrity_VS_point_in_time_without_check.png" alt="Process_integrity_VS_point_in_time_without_check.png" width="800" /><figcaption>Process integrity tool VS point in time verification tool</figcaption>
</figure>

<h1><p><b>Technical Description</b></p></h1>
<h2>Without further complicating development environment</h2>
<li>SCAT is a simple 5 screen MVC, C# web application with a small footprint that can be deployed without further complicating development environment</li>
<li>Integrates with Jira and runs ZAP and SonarQube in docker containers</li>
<li>SCAT is part of three domains to consider when securing software development. <em>I've detailed the other domains in an article that will be published in the Nov/Dec issue of the ISC2 magazine, I will add a link here after publication.</em>

<h1><p><b>See how developers use SCAT</b></p></h1>
<p>See below how the Secure code assurance tool integrates security into software development phases</p>

<h2>Sprint planning phase</h2>
<p><b>Objective</b>: Ensures security requirements are understood<br /></p>
<li><b>Developers</b> use the <b>Identify risks</b> screen to<br />
<ol>
<li>Select the critical function to developing/changing</li>
<li>Identify the technologies used</li>
<li>Automatically generate the security requirements and tests</li>
</ol>
<p><a href="https://youtu.be/Gpk4K5keLyw">See how to use the tools and its internal mapping to generate security requirements</a></p></li>
</li>
</ol>
<li>
<p><b>Product owners</b> use the <b>Secure code requirements</b> screen to<br />
</p>
<ol>
<li>Create an audit trail to store evidence of secure development</li>
<li>Create Jira tickets for requirements and tests to manage work</li>
</ol>
</li>
<h2>Development phase</h2>
<p><b>Objective</b>: Ensure correct implementation of security requirements<br />
</p>
<li><b>Developers</b> use the <b>Secure development</b> screen to<br />

<ol>
<li>View and understand how to attack and prevent the risk</li>
<li>View the secure code requirements</li>
<li>View the secure code block to implement the security requirement</li>
<li>Manage development effort in Jira</li>
<li>After development run a ZAP basic scan to verify security requirements have been correctly implemented</li>
</ol>
<p><a href="https://youtu.be/1pSatE_7mEs">See how the tool helps developers understand security requirements and write secure code</a></p></li>
</ol>
</li>
<h2>Secure code review phase</h2>
<p><b>Objective</b>: Ensure correct implementation of security requirements<br />
</p>
<li><b>Code reviewers</b> use the <b>Secure code review </b> screen to<br />

<ol>
<li>Guide manually secure code review</li>
<li>After manual secure code review run a Sonarqube scan to verify security requirements have been correctly implemented</li>
</ol>
<p><a href="https://youtu.be/ygre0SrWxD4">See how the tool verifies correct security requirements implementation</a></p></li>
</ol>
</li>
<h2>Testing phase</h2>
<p><b>Objective</b>: Ensure valid security testing<br />
</p>
<li><b>Testers</b> use the <b>Secure testing</b> screen to<br />

<ol>
<li>View the test plans required to test the risk</li>
<li>Manage testing effort in Jira</li>
</ol>
<p><a href="https://youtu.be/QdbCzheceUw">See how the tool helps testers test risk mitigation efforts</a></p></li>
</ol>
</li>
<h2>Approval phase</h2>
<p><b>Objective</b>: Streamline the approval and audit process<br />
</p>
<li><b>Approvers</b> use the <b>Assurance evidence </b> screen to<br />

<ol>
<li>View relevant testing evidence alongside the risk, reducing the time assurance teams need to examine and approve releases</li>
<li>View verified development effort and whether it falls within risk tolerance levels</li>
</ol>
<p><a href="https://youtu.be/oyKK3Mq13B4">See how the tool streamlines the approval process with centrally stored testing evidence</a></p></li>
</ol>
</li>
<h2>Risk management</h2>
<p><b>Objective</b>: Enable risk managers to prioritise, plan and monitor mitigation efforts<br />
</p>
<li><b>Risk managers</b> use the <b>Application risk exposure</b> screen to<br />

<ol>
<li>View each application critical function and the associated risks</li>
<li>Identify where mitigation effort is required by viewing which risks require security requirements</li>
<li>Identify where development effort is required by viewing which security requirements need secure code blocks</li>
<li>Identify where extra testing effort is required by viewing which risks require security test plans</li>
</ol>
<p><a href="https://youtu.be/8pKxorPSq_M">See how the Application landscape overview screen informs risk based decision making</a></p></li>
</ol>
</li>
<p><br />
<br />
</p>
<h1>
<p><b>Preparation phase</b></p>
</h1>
<p>When developing secure software we need to consider both standard secure code and client specific architectural requirements</p>
<h2>Standard secure code requirements</h2>
<li>SCAT comes out the box with a standard OWASP secure code requirements map. This mapping need to be modified to the specific organisation requirements</li>
<p><br />
</p>
<li>
<p><b>Information security and development team</b> use the <b>Internal mapping </b> screen to</p>
<ol>
<li>Map the security requirements to OWASP risks</li>
<li>Map organisation approved secure code blocks to security requirements</li>
<li>Map security test plans to OWASP risks</li>
</ol>
<p><a href="https://youtu.be/EkWdAC1sbkE">See how to setup the SCAT's internal mapping</a></p>
</ol>
</li>
<h2>Client specific architectural requirements</h2>
<li>To generate these requirements we perform a risk assessment on client application landscape and identify</li>
<ol>
<li>Critical applications and functions</li>
<li>Risk associated with each critical application function</li>
<li>Architectural security requirements to secure each critical application functions</li>
<li>Client specific secure code blocks to implement security requirements</li>
<li>Secure test plans to verify risk has been mitigated</li>
</ol>
<p><br />
</p>
<li>
<p><b>Tool administrators</b> use the <b>Internal mapping </b> screen to</p>
<ol>
<li>Create json files of the organisation specific risks, security requirements, secure code blocks and tests</li>
<li>Import these into the SCAT</li>
</ol>
<p><a href="https://youtu.be/FD3O2ObYBQs">See how to import organisations specific risks, security requirements, secure code blocks and tests</a></p>
</ol>
<p><br />
<br />
</p>
<h1>
<p>Project information</p>
</h1>
<h2>Licensing</h2>
<p>This program is free software: you can redistribute it and/or modify it under the terms of the <a href="http://www.gnu.org/licenses/agpl-3.0.html">link GNU Affero General Public License 3.0</a> as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.</p>
<h2>Interested in contributing</h2>
<p><a href="https://www.linkedin.com/in/michael-bergman-99826212a/">Please send a connect request with subject SCAT</a></p>
<h2>Project Resources</h2>
<p>[Installation Package]</p>
<p>[Source Code]</p>
<h2>Project Leader</h2>
<p><a href="https://www.linkedin.com/in/michael-bergman-99826212a/">Michael Bergman LinkedIn</a></p></td>
</tr>
</tbody>
</table>
