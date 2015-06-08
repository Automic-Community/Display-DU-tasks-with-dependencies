*Display DU tasks with dependencies*
=============


This script output list of task and the dependant objects.
http://github.com/Automic-Community/Display-DU-tasks-with-dependencies

<!-- List of attached files -->
Contents of Solution Package:

						
								*Dollar_Universe-Task_Dependencies.zip
								
						


Documenation and Instructions
---

<div class="ipsType_textblock ipsPad_half description_content"><strong class="bbc"><span>Description</span></strong><br /><br />This script output list of task and the dependant objects<br /><br /><strong class="bbc"><span>Argument list</span></strong>
<ul class="bbc">
<li>Area: APP, SIM, INT, EXP</li>
<li>Nodes (optional, can contain wildcards *)</li>
</ul>
<span><strong class="bbc">Example</strong></span><br /><br />
<pre class="prettyprint lang-auto linenums:0 prettyprinted"><span class="pln">C</span><span class="pun">:</span><span class="pln">\Users\Administrator\Documents</span><span class="pun">&gt;</span><span class="pln">perl du_task_dependencies</span><span class="pun">.</span><span class="pln">pl EXP hklpmsup01

HKLPMSUP01 </span><span class="pun">|</span><span class="pln"> </span><span class="pun">((</span><span class="pln">ENDMONTH</span><span class="pun">,</span><span class="lit">09</span><span class="pun">/</span><span class="lit">16</span><span class="pun">/</span><span class="lit">2013</span><span class="pun">))</span><span class="pln"> </span><span class="pun">|</span><span class="pln">  </span><span class="pun">|</span><span class="pln"> RESTARTWEB </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CMD</span><span class="pun">)</span><span class="pln"> servicetomcat5restart

HKLPMSUP01 </span><span class="pun">|</span><span class="pln"> </span><span class="pun">((</span><span class="pln">SUNDAY</span><span class="pun">,</span><span class="lit">09</span><span class="pun">/</span><span class="lit">16</span><span class="pun">/</span><span class="lit">2013</span><span class="pun">))</span><span class="pln"> </span><span class="pun">|</span><span class="pln"> DB_BACKUP </span><span class="pun">|</span><span class="pln"> BCK_HEADER </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_INT</span><span class="pun">)</span><span class="pln">
                                                 BCK_STOPDB </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_EXT</span><span class="pun">)</span><span class="pln"> </span><span class="pun">/</span><span class="pln">opt</span><span class="pun">/</span><span class="pln">tools</span><span class="pun">/</span><span class="pln">DB</span><span class="pun">/</span><span class="pln">stop</span><span class="pun">.</span><span class="pln">ksh
                                                 BCK_SQLEXP </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_EXT</span><span class="pun">)</span><span class="pln"> </span><span class="pun">/</span><span class="pln">opt</span><span class="pun">/</span><span class="pln">tools</span><span class="pun">/</span><span class="pln">DB</span><span class="pun">/</span><span class="pln">backupsql</span><span class="pun">.</span><span class="pln">ksh
                                                 BCK_STRTDB </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_EXT</span><span class="pun">)</span><span class="pln"> </span><span class="pun">/</span><span class="pln">opt</span><span class="pun">/</span><span class="pln">tools</span><span class="pun">/</span><span class="pln">DB</span><span class="pun">/</span><span class="pln">start</span><span class="pun">.</span><span class="pln">ksh
                                                 BCK_UPLOAD </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_EXT</span><span class="pun">)</span><span class="pln"> </span><span class="pun">/</span><span class="pln">opt</span><span class="pun">/</span><span class="pln">tools</span><span class="pun">/</span><span class="pln">DB</span><span class="pun">/</span><span class="pln">server_publish</span><span class="pun">.</span><span class="pln">ksh
                                                 BCK_NOTIFY </span><span class="pun">|</span><span class="pln"> </span><span class="pun">(</span><span class="pln">type</span><span class="pun">:</span><span class="pln"> CL_INT</span><span class="pun">)<br /><br /></span></pre>
<p>&nbsp;</p>
<p><strong class="title">Target environments:</strong> Unix</p>
<p><strong class="title">Prerequisites:</strong> Perl, $U</p>
</div>

Copyright and License
---

Solutions, Templates, Actions and other content available on the Automic Marketplace subject to the Automic [Developers Distribution License] (http://automic.com/developers-distribution-license) as well as the Automic Community [Terms of Service] (http://automic.com/community-terms-of-service).
Automic does not support, maintain or warrant any content submitted by the Automic Community.



Questions or Need Help? 
---
Any questions or comments? Converse with your fellow Users in the [Automic Community] (https://community.automic.com).