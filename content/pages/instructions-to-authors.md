Title: Instructions to Authors
Slug: instructions-to-authors

<h3 id="instructions"> </h3>

Instructions for Authors
-----------------------
<!-- ### Directory-->
1. [Types of submission](#types)
2. [Preparing your submission](#preparing)
    - [The manuscript](#manuscript)
    - [The source code](#source_code)
3. [Submission](#submission)
    - [Pre-submission checklist](#submission_checklist)
4. [Curation](#curation)
5. [Publishing](#publishing)
6. [Copyright of submission](#copyright)

<!-- <details> -->
<!-- <summary>Click</summary> -->
The model files submitted to <i>Physiome</i> must be <a href="about.html">reusable</a>, and associated with at least one article accepted by a peer-reviewed journal in the field of physiological modelling (a Primary Publication). Authors are encouraged to prepare their <i>Physiome</i> submission(s) in parallel to the Primary Publication. Submissions will be curated and evaluated, but not published until the Primary Publication is accepted. 
<!-- </details> -->

For queries, see the <a href="faqs.html">Frequently Asked Questions</a>. Otherwise, <a href = "mailto:physiome@physiomeproject.org">email the curators</a>. Include the submission identification number if querying a specific submission.

***
<h3 id="types">1. Types of submissions</h3>

The following will be considered for publication in <i>Physiome</i>: 

**2.1 Original submission**

Original submissions are author-initiated submissions directly associated with a primary experimental or modelling paper. While matching authorship between the <i>Physiome</i> submission and the primary publication is not a requirement, it is expected that there is some overlap. The <i>Physiome</i> team can help with reaching out to additional authors if needed.

**2.2 Retrospectives**

Similar to an original submission, but is associated with a historical Primary Publication which has been judged to be of substantial value to the physiological modelling community, such that a reusable, reproducible, and discoverable version of the study should be made available. Where possible, the authors of retrospective should include authors from the primary publication. Retrospectives may be invited by the <i>Physiome</i> editors or can be author-initiated. 

When submitting a retrospective, it is best to first submit an expression of interest to the editors outlining why the original primary publication should be considered a suitable contribution to <i>Physiome</i>.

**2.3 Reviews**

The <i>Physiome</i> editorial board may solicit review submissions that document a range of published models in a given area. Such reviews will make use of previously accepted <i>Physiome</i> submissions, often applying new data or simulation experiments to explore the capabilities of the various models. They may also point to areas of the research field lacking reproducible and reusable models. 

Reviews do not require a Primary Publication.

**2.4 Letters**

This is an original submission that provides new insights about, or refinement of, a model that is already published in <i>Physiome</i>. This format allows publication of material that in itself may not justify a separate submission to a primary journal, but which may still be highly instrumental for improving an existing model, expand its empirical scope or invoke experimental and theoretical research that may drive new model development. 

Examples of such material include, but are not restricted to:
<ul>
<li>experimental measurements of important parameter values that have been only indirectly estimated in the original paper</li>
<li>empirically or theoretically justified questioning or refutation of critical model premises</li>
<li>experimental data confirming or refuting model predictions</li>
<li>theoretical analyses of the model that provide novel insights that may spur further model development or experimental work</li>
</ul>

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="preparing">2. Preparing your submission</h3>

The <i>Physiome</i> submission must include all the resources required to evaluate the reproducibility, reusability, and discoverability of the model. 

Every Original or Retrospective submission in <i>Physiome</i> must be associated with at least one Primary Publication. It is encouraged that the authors of the Primary Publication are included as authors in the <i>Physiome</i> paper. 

A <i>Physiome</i> article consists of a description and the code of a reproducible implementation of the model. Such resources can be directly included in the ZIP archive submitted to <i>Physiome</i>, or linked to via appropriate online repositories or databases. A list of the databases used by <i>Physiome</i> can be found <a href="instructions-to-authors.html#submission">here</a>. 

While there are many different types of models, file types and structures used by modelers, there are some items which are common to all <i>Physiome</i> submissions. These are:

<ul>
<li>A manuscript, which should be prepared using the <i>Physiome</i> Overleaf template.</li> 
<li>Source code for the model. Instructions on how to run them in order to reproduce the results must be presented in the manuscript. </li>

<!-- The manuscript must include: 
<ol>
<li> a summary of the background, purpose and modifications of the model </li>
<li> all instructions needed to run the implemented files</li>
<li> clearly-stated reproducibility goals that overlap with the results shown in the Primary Publication.</li>
</ol> -->

</ul>

 <div style = "text-align: center;">

<a type="button" style="vertical-align: middle; text-align: center; background-color: #580078; color:white; border: 1px solid #580078;" href="https://www.overleaf.com/latex/templates/physiome-journal-article-template/kfbqwxxmtsfv" class="button"><i>Physiome</i> Overleaf template</a>

  </div>

##### __The manuscript__ <a name="manuscript"></a>
Below is listed the minimal information required in an original submission to <i>Physiome</i>. Any sections necessary to give a clear description of the model can be added or removed at the author's discretion. Note that information such as parameter values and units may already be present in the model files, and thus do not need to be repeated in the submission.

*Introduction:* 
A brief explanation of the biological system modelled. Make sure to define the biological entities and species used in the primary papers. Clearly reference previously published iterations of the model to establish provenance, and any data that has been used for validation.

*Model Description:*
An overview of the type of model and its structure. As the model code submitted should be complete, all parameter values, units, etc. will be included in your files and are not required to be printed in the article. 

*Model Modifications:*
Any modifications made to the model as presented in the primary publication, while providing motivations for doing so. Include corrections, missing parameter values taken from other sources, reformulation of equations, etc. Provide references to the origins of the parameter values, if not defined in the primary publication.

*Computational Simulation:*
All relevant information on how to run the model. This includes, but is not limited to, definitions of libraries, versions of simulation packages, computational solvers and time steps used, type of machine the code was originally executed on,  etc. 

*Reproducibility goals:*
Figures showing that the code simulates the same graphs as shown in the primary paper. Any differences are explained.

*Discussion:*
Discuss the results and the model reliability.
 
 *Figures:*
<ul>
<li> Ensure the graphs presented in the manuscript are the same as the ones produced by your submitted code. </li>
<li>Use high quality images. Recommended image formats are .pdf for plots, graphs, and diagrams, and .jpg for photographic images. <a href="https://www.overleaf.com/learn/latex/Inserting_Images">Advice on image handling in Overleaf can be found here.</a> Maximum image size is 1MB. 
<a href="https://www.overleaf.com/help/336-my-image-files-are-very-large">See here for treatment of large images.</a> </li>
<li>Use a sans serif font for text in the figures, of at least 10pt font size in the final image in the manuscript. </li>
<!-- <li>Label subplots in the upper left corner using capital letters. Label all axes and include units. </li> -->
<!-- <li>Include a legend if the graph has multiple curves in the same plot. If you want to point out specific features of a graph, use inserts or arrows rather than incomplete representations of the graph. </li> 
 --></ul>

##### __The source code__ <a name="source_code"></a>
Source codes for the model implementation can be in procedural (e.g. Matlab, C, Python) or declarative (e.g. CellML, SBML, SED-ML) languages. 
The source material must include:
<ul>
<li>All units</li>
<li>All parameter values</li>
<li>Initial conditions</li>
<li>All equations</li>
<li>Annotation (if possible)</li>
</ul>

If possible, show that the model obeys physical laws such as conservation of energy, mass and/or charge. 
This could be done, for example, by implementing it in bond graph form, or formulating it as a port-Hamiltonian system and implementing it numerically in a mass-energy conserving form.

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="submission">3. Submission</h3>

 <div style = "text-align: center;">
 
<a type="button" style="vertical-align: middle; text-align: center; background-color: #580078; color:white; border: 1px solid #580078;" href="testing.html" class="button"><i>Physiome</i> submission system</a>

  </div>

An <a href="https://orcid.org/">ORCiD</a> is required to log in. If the submitter and the corresponding author are different, make sure that the verified email is tied to the submitter.  

All accepted submissions will be published as open access on <a href="https://physiome.figshare.com/">figshare.</a> 

Submissions can be made by sending the files directly through the submission system, or by linking to an open access, permanent, and version-controlled repository. For the latter, which we encourage authors to use the <a href="https://models.physiomeproject.org">Physiome Model Repository (PMR)</a>, which is version-controlled. Upon receipt of a submission which is not already linked to the PMR, curators will create a private PMR workspace for the submission. When a <i>Physiome</i> submission consists of models or data already in PMR, then curators will internally link the workspaces.

Alternatively, you may submit to these popular repositories. Make sure to give our curator access to your workspace.

<ul>
<li><a href="https://models.physiomeproject.org">Physiome Model Repository (PMR)</a> Username: PhysiomeCurators</li>
<li><a href="https://github.com/">GitHub</a> Username: PhysiomeCurators</li>
<li><a href="https://bitbucket.org/">Bitbucket</a> Username: PhysiomeCurators</li>
<li><a href="https://www.ebi.ac.uk/biomodels/">BioModels</a> Username: PhysiomeCurators</li>
<li><a href="https://figshare.com/">figshare</a> Username: Curators Physiome</li>
<li><a href="https://drive.google.com/">Google Drive</a> Username: PhysiomeCurators@gmail.com (Note: this email is not monitored, use only for sharing Google Drive.)</li> 
</ul>


#### Pre-submission checklist <a name="submission_checklist"></a>

<!-- ####Before submitting your model to <i>Physiome</i> for curation, please check: -->

<ul>
<li>Are the reproducibility goals clearly stated in your manuscript, and do they overlap with results from the primary paper?</li>
<li>Does the implemented model in your submission reproduce the results presented in the manuscript?</li>
<!-- , both reproduced results and additional predictions? -->
<li>Are all instructions needed to run the model files outlined in your manuscript?</li>
<li>Are all files needed to run the implemented model included?</li>
<li>Are .SEDML files, or a plotting script, included?</li>
<li>Is your model presented in a standardised format (if possible)? </li>
<li>Have you specified the provenance of your model and parameter values?</li>
<li>Does the model have appropriate modularity and annotation (if possible)?</li>
<li>Is your manuscript written in the <a href="https://www.overleaf.com/latex/templates/physiome-journal-article-template/kfbqwxxmtsfv"><i>Physiome</i> Overleaf template</a>?</li>
<li>Are all graphs and axes labeled in your figures, and is the text in your figures in a large enough font size to be easily read?</li>
<li>Have you shown that the model obeys physical laws such as conservation of energy, mass and/or charge?</li>
</ul>

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="curation">4. Curation</h3>
The <i>Physiome</i> curators will check the reproducibility of your model by running the model implementation provided in the submission and comparing the results to the primary paper as stated in the reproducibility goals of the manuscript. If the model can not reproduce the results, or if there are any problems with running the files, the submitting author will be contacted. 

If the model or simulation implementation can be encoded in one of the <a href="faqs.html#standard_formats"><i>Physiome</i> standards</a>, the curators will assist the author to do this, resource permitting.

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="publishing">5. Publishing</h3>
Two outputs are made in the final published <i>Physiome</i> articles:
<ul>
<li> as a PDF manuscript hosted on <a href="http://physiome.figshare.com/">figshare</a> containing all details on model implementation</li>
<li> an <a href="faqs.html#omex">OMEX archive</a> containing the model files</li>
</ul>

<i>Physiome</i> will collaborate with the <a href="http://reproduciblebiomodels.org">Center for Reproducible Biomedical Modeling</a> to produce a reproducibility report for every <i>Physiome</i> article. This report will detail the different aspects of the model’s reproducibility and repeatability and will be appended to the finalised manuscript.

<i>Physiome</i> articles are curated and published as open access with a DOI citable as a journal article. 

We store only the information you submit to us, which includes your <a href="https://orcid.org/">ORCID</a>, your name and email address. Submission data are stored locally on the submission system while we rely on a private <a href="https://docs.aws.amazon.com/AmazonS3/latest/gsg/GetStartedWithS3.html">Amazon S3 bucket</a> to store files you submit to us. No payment information will be stored by us, as this is managed through <a href="https://stripe.com/">Stripe</a>, our payment provider. Personal information will only be used for attribution of the research work being published.

There is an author processing charge of US$300. This is to be paid after acceptance of the submission, but before publication.

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>
***
<h3 id="copyright">6. Copyright of submission</h3>
<i>Physiome</i> supports open science and believes that authors should retain the rights to their works. Our copyright policy is the following:
<ol>
<li>The authors grant to the <i>Physiome</i> the right to publish and communicate Works to the public in electronic form under one <a href="https://creativecommons.org/licenses/by/4.0/legalcode">Creative Commons license.</a></li>
<li>The authors retain copyright in the Works and the right to re-use the Works after publication.</li>
<li>The authors must obtain permission from any rights owner to include any third party content.</li>
</ol>
For additional questions on <i>Physiome</i>’s copyright and licensing policies, please contact our editors at <a href = "mailto:physiome@physiomeproject.org">physiome@physiomeproject.org</a>.

<div align="right"><h4><a href="#instructions"><i class="fa fa-angle-double-up"></i></a></h4></div>