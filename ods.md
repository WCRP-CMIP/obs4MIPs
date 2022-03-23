<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 9; WARNINGs: 1; ALERTS: 39.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>
<a href="#gdcalert13">alert13</a>
<a href="#gdcalert14">alert14</a>
<a href="#gdcalert15">alert15</a>
<a href="#gdcalert16">alert16</a>
<a href="#gdcalert17">alert17</a>
<a href="#gdcalert18">alert18</a>
<a href="#gdcalert19">alert19</a>
<a href="#gdcalert20">alert20</a>
<a href="#gdcalert21">alert21</a>
<a href="#gdcalert22">alert22</a>
<a href="#gdcalert23">alert23</a>
<a href="#gdcalert24">alert24</a>
<a href="#gdcalert25">alert25</a>
<a href="#gdcalert26">alert26</a>
<a href="#gdcalert27">alert27</a>
<a href="#gdcalert28">alert28</a>
<a href="#gdcalert29">alert29</a>
<a href="#gdcalert30">alert30</a>
<a href="#gdcalert31">alert31</a>
<a href="#gdcalert32">alert32</a>
<a href="#gdcalert33">alert33</a>
<a href="#gdcalert34">alert34</a>
<a href="#gdcalert35">alert35</a>
<a href="#gdcalert36">alert36</a>
<a href="#gdcalert37">alert37</a>
<a href="#gdcalert38">alert38</a>
<a href="#gdcalert39">alert39</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



# obs4MIPs data specifications (ODS) v2.1 

** **Peter J. Gleckler, Karl E. Taylor, Paul J. Durack, Denis Nadeau, Jim Biard, Robert Ferraro, Stephan Finkensieper, Scott Stevens, Matthias Tuma and

contributing members from the WDAC, WDAC task team, and others…

**

<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Latest version finalized : September 22, 2017 (v2.1.0)"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Latest version finalized : September 22, 2017 (v2.1.0)](#heading=h.mnn77v48k374)**

**Short URL: [https://goo.gl/jVZsQl](https://goo.gl/jVZsQl)**

**[Link to obs4MIPs tables and controlled vocabulary 2.0.0](https://github.com/PCMDI/obs4MIPs-cmor-tables/tree/2.0.0) **

**ODS v2.1 strives to improve upon the original obs4MIPs data specifications (ODS v1.0) by capturing additional useful information while at the same time retaining consistency with both ODS v1.0 (for backwards compatibility) and the CMIP6 data specifications. We believe most, if not all of the required global attributes that will be relied on through CMIP6 are described below. However, minor updates to this document can be expected throughout 2017 as some of the underlying metadata tables are revised and ESGF search facets are upgraded. Any changes will be noted with an increment to the ODS version number (

<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Appendix 3"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Appendix 3](#heading=h.mnn77v48k374)), which is currently “2.1.0”.**

**We strongly encourage obs4MIPs data providers to communicate with us ([obs4MIPs-admin@llnl.gov](mailto:obs4MIPs-admin@llnl.gov)) as they prepare their data contributions with CMOR3 ([https://goo.gl/LePm8H](https://goo.gl/LePm8H)) following the metadata specifications below. **


# 


# CONTENTS


[TOC]



# 


# Introduction {#introduction}

The purpose of [obs4MIPs](https://www.earthsystemcog.org/projects/obs4mips/) is to facilitate comparison of observational data to model output from WCRP intercomparison projects (notably the [Coupled Model Intercomparison Project, CMIP](https://www.wcrp-climate.org/wgcm-cmip)). To accomplish this, the organization of CMIP and obs4MIPs data are closely aligned, including the data structure and metadata requirements, and the infrastructure relied on for archival, searching and accessibility via the [Earth System Grid Federation (ESGF)](http://esgf.llnl.gov/) using the [CoG](https://www.earthsystemcog.org/projects/cog/).

[The original set of obs4MIPs contributions adhered to guidelines](https://docs.google.com/document/d/1kgtS3vHfA_v3xje-HsNG2NT6d7Gc7NcBO35O7oSrrHw/edit#heading=h.qozxbcgu2wiv) (ODS V1.0, circa 2012) that were based on the [CMIP5 data specifications](http://cmip-pcmdi.llnl.gov/cmip5/output_req.html#req_list). Now, as described below, the obs4MIPs data specifications have been refined to be closely aligned with the [CMIP6 data specifications](https://docs.google.com/document/d/1h0r8RZr_f3-8egBMMh7aqLwy3snpD6_MrDz1q8n5XUk/edit), which are overseen by the [Working Group on Coupled Models (WGCM) Infrastructure Panel (WIP](https://www.earthsystemcog.org/projects/wip/)). Obs4MIPs governance is provided by [WCRP’s Data Advisory Council's “Observations for Model Evaluation Task Team” (or simply “obs4MIPs TT”)](https://www.wcrp-climate.org/wdac-overview).  

To avoid naming conflicts in the identification of data sources and institutions, it is necessary for  data providers to register the name of their institution and information about their data sets _prior to generating_ obs4MIPs data sets. This is done by submitting an “issue” on the [obs4MIPs-cmor-tables Github repository](https://github.com/PCMDI/obs4MIPs-cmor-tables). (See [Appendix 2](#bookmark=id.r55y5lgk9uho) for the information requested.)

obs4MIPs metadata specifications for the following categories are described in this document: 

 



1. 

<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Global attributes"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Global attributes](#heading=h.2et92p0): Explicitly defined metadata included in netCDF files that describe the contents of the dataset and provenance (e.g., “variable_id”). 
2. 

<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Data Reference Syntax (DRS)"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Data Reference Syntax (DRS)](#heading=h.3dy6vkm): Some attributes (e.g.,“institution_id’, “source_id”, “variable_id”) comprise the data reference syntax (DRS) for obs4MIPs, which closely parallels the DRS of CMIP6. The DRS is used, for example, in file names, directory structures, the further_info_url, and in facets of some search tools such as ESGF.
3. 

<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Directory structure"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Directory structure](#heading=h.4d34og8): This can be thought of in the traditional sense, and includes selected DRS information used as subdirectories. It is explicitly defined in obs4MIPs to facilitate searching for data with the ESGF.    
4. 

<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Filenames"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Filenames](#heading=h.1t3h5sf): Like the directory structure, filenames are constructed based on a template that relies mainly on a subset of the CV entries.   

The global attributes are constructed to facilitate organization of the obs4MIPs datasets, and in particular for providing a useful set of options (or facets) for data exploration via CoG/ESG. The purpose of the DRS is more behind the scenes than the search functions - but it is critical in defining how data from the complex CMIP6 and obs4MIPs databases is organized (notably the directory structure). These obs4MIPs data structures are curated by the authors of this document in consultation with the obs4MIPs TT and the WIP.

Satisfying these (or the CMIP6) data requirements can be facilitated by using the [Climate Model Output Rewriter](http://cmor.llnl.gov/) (CMOR3), as described in a [separate document](https://docs.google.com/document/d/1F25iGZ4C56byK38ObAXeukCAkKm_TwGX8dN41Bj2VaI/edit). Use of CMOR3 is not required for producing obs4MIPs data, but it is strongly recommended because CMOR3 ensures that the necessary metadata for distributed data searching is included. A user populates an input table with the entries of the required global attributes, and from this, CMOR3 automatically produces the DRS and filenames.  

Beyond metadata, this document includes a discussion of the inclusion (or not) of grid cell bounds. This information makes it possible for users of the data to weight the influence of each cell based on its surface area (or volume), e.g., for calculating a global mean. A user can estimate the grid cell bounds, but in general those closest to the original data are better positioned to estimate them. We recommend that data providers include grid bounds (

<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Appendix 1"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

[Appendix 1](#heading=h.gwx8b34tp8q)).


# Global attributes {#global-attributes}

Table 1 contains the list of obs4MIPs global attributes, indicating which are required and which are optional. The values for many of the global attributes must be drawn from special obs4MIPs “controlled vocabularies” (CVs). A CV, in simplest form, is a list of the permitted values that can be assigned to a given global attribute. The lists of permitted values can be found in the [reference CVs for obs4MIPs](https://github.com/PCMDI/obs4MIPs-cmor-tables) maintained on a github repository.



**Table 1: obs4MIPs global attribute description** 

and comparison with the original obs4MIPs conventions (ODS V1.0, circa 2012)

**Table color key: **

Name or form has been changed relative to CMIP5 and/or ODS V1.0

New attribute for obs4MIPs

Controlled Vocabulary (CV)

Registered Content (RC)


<table>
  <tr>
   <td><strong>obs4MIPs required global attributes</strong>
<p>
<strong>see note 1</strong>
   </td>
   <td><strong>description</strong>
   </td>
   <td><strong>examples</strong>
   </td>
   <td><strong>related attribute in original  obs4MIPs </strong>
<p>
<strong>circa 2012</strong>
   </td>
   <td><strong>form</strong>
<p>
<strong>see note 2</strong>
   </td>
   <td><strong>when required?</strong>
   </td>
   <td><strong>further information and rationale</strong>
   </td>
  </tr>
  <tr>
   <td><strong>activity_id</strong>
<p>
<strong>(see note 3) </strong>
<p>
<strong>  </strong>
   </td>
   <td>activity  identifier
   </td>
   <td>only value permitted is <strong>“</strong>obs4MIPs<strong>”</strong>
   </td>
   <td>project_id
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>Renamed more generically, since not all activities are projects; also multiple activities may now be listed separated by single spaces
   </td>
  </tr>
  <tr>
   <td><strong>comment</strong>
   </td>
   <td>see note 9
   </td>
   <td>see note 9
   </td>
   <td>comment
   </td>
   <td>free form
   </td>
   <td>never
   </td>
   <td>No change from original obs4MIPs or CMIP5; CF-convention standard
   </td>
  </tr>
  <tr>
   <td><strong>contact</strong>
   </td>
   <td>see note 9
   </td>
   <td>see note 9
   </td>
   <td>contact
   </td>
   <td>free form
   </td>
   <td>always
   </td>
   <td>Still required with ODS-2.0, but anticipated to be superseded by “further_info_url” (below) maintained by ESDOCs
   </td>
  </tr>
  <tr>
   <td><strong>Conventions </strong>
   </td>
   <td>convention version
   </td>
   <td>"CF-1.7 ODS-2.1” or higher
   </td>
   <td>Conventions
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>Updated version from ODS-1.0  with a list of conventions separated by single spaces now allowed
   </td>
  </tr>
  <tr>
   <td><strong>creation_date </strong>
   </td>
   <td>date file was created
   </td>
   <td>see note 5
   </td>
   <td>creation_date
   </td>
   <td>structured form
   </td>
   <td>always
   </td>
   <td>No change from original obs4MIPs specs (automatic with CMOR3)
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>data_specs_version</strong>
   </td>
   <td>version  identifier of obs4MIPs CV’s and CMOR tables
   </td>
   <td>2.1.0
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>This version number is associated with the version or github “tag” for the obs4MIPs CMOR tables and the CV’s. See 

<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "CV discussion"). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.tyjcwt">CV discussion</a> and <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables">PCMDI/obs4MIPs-cmor-tables</a> which originate from the CMIP6 tables
   </td>
  </tr>
  <tr>
   <td><strong>external_variables</strong>
   </td>
   <td>external cell measures
   </td>
   <td>“areacella”, “areacello”, “volcella”, “volcello”,  
<p>
as defined in CMIP6
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV
   </td>
   <td>rarely needed, but include when appropriate
   </td>
   <td> List of cell measure variables (separated by single spaces) that are referenced but not included in the file. These variables will be stored independently in the obs4MIPs  data archive. Use of this attribute is expected to be infrequent in contrast to the recommended inclusion of grid bounds (

<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: undefined internal link (link text: "Appendix "). Did you generate a TOC? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<a href="#heading=h.gwx8b34tp8q">Appendix </a>1)
   </td>
  </tr>
  <tr>
   <td><strong>frequency</strong>
   </td>
   <td>sampling frequency
   </td>
   <td>“day”
   </td>
   <td>frequency
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>No change from original obs4MIPs. The current options are given in <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_frequency.json">obs4MIPs_frequency.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>further_info_url</strong>
   </td>
   <td>location of documentation
   </td>
   <td>see note 6
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV based
   </td>
   <td>always 
   </td>
   <td>Efforts are underway to coordinate with ES-DOCs to create urls for each dataset. It is expected that this will point to documentation that can be updated by the data provider
   </td>
  </tr>
  <tr>
   <td><strong>grid</strong>
   </td>
   <td>grid
   </td>
   <td>see note 7
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>free form
   </td>
   <td>always
   </td>
   <td>Briefly describes output grid characteristics
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>grid_label</strong>
   </td>
   <td>grid identifier
   </td>
   <td>“gn”, “gr1”
<p>
 see note 8
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV
<p>
(note 11)
   </td>
   <td>always
   </td>
   <td>Used in file name to distinguish among files when the variable is reported on more than one grid.  See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_grid_label.json">obs4MIPs_grid_label.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>history</strong>
   </td>
   <td>see note 9
   </td>
   <td>see note 9
   </td>
   <td>history
   </td>
   <td>free form
   </td>
   <td>never
   </td>
   <td>No change; CF-convention standard
   </td>
  </tr>
  <tr>
   <td><strong>institution</strong>
   </td>
   <td>institution name
   </td>
   <td>“NOAA's National Centers for Environmental Information, Asheville, NC 28801, USA”
   </td>
   <td>institution
   </td>
   <td>CV with registered content
   </td>
   <td>always
   </td>
   <td>Can be used to identify institute responsible for dataset including a curator role if data is no longer managed by original individual or entity. These entries must be registered in: <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_institution_id.json">obs4MIPs_institution_id.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>institution_id</strong>
<p>
Will have ESGF alias with institution_id to be backwards compatible with ODS v1.0
   </td>
   <td>institution identifier
   </td>
   <td>“NCEI”
   </td>
   <td>institute_id
   </td>
   <td>CV with registered content
   </td>
   <td>always
   </td>
   <td>Was “institute_id”; name changed to parallel other global attributes; this string is constructed only using the character set: a-z, A-Z, 0-9, and “-’. These entries must be registered in: <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_institution_id.json">PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_institution_id.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>license</strong>
   </td>
   <td>license restrictions
   </td>
   <td>see note 13
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>some required text
   </td>
   <td>always
   </td>
   <td>Ensures that anyone using the files has access to the terms of use
   </td>
  </tr>
  <tr>
   <td><strong>nominal_resolution</strong>
   </td>
   <td>approximate horizontal resolution
   </td>
   <td>“50 km”, “100 km”, “250 km”,  “1x1 degree”. (See <a href="https://docs.google.com/document/d/1h0r8RZr_f3-8egBMMh7aqLwy3snpD6_MrDz1q8n5XUk/edit#bookmark=id.ibeh7ad2gpdi">Appendix 2</a> of CMIP6 specifications)
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>Added in CMIP6 to provide an indication of approximate output  grid resolution. See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_nominal_resolution.json">obs4MIPs_nominal_resolution.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>product</strong>
   </td>
   <td>product type
   </td>
   <td>“observations”, “reanalysis”
   </td>
   <td>product
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>As in original obs4MIPs and CMIP5
   </td>
  </tr>
  <tr>
   <td><strong>realm</strong>
   </td>
   <td>realm(s) where variable is defined
   </td>
   <td>“atmos”, “ocean”, 
<p>
“land”,
<p>
“seaIce”
<p>
“atmosChem”
   </td>
   <td>realm
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>As in original obs4MIPs. See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_realm.json">obs4MIPs_realm.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>references</strong>
   </td>
   <td>see note 9
   </td>
   <td>see note 9
   </td>
   <td>references
   </td>
   <td>free form
   </td>
   <td>never
   </td>
   <td>No change; CF-convention standard
   </td>
  </tr>
  <tr>
   <td><strong>region</strong>
   </td>
   <td>Pre-defined (CF conventions) approximate regions 
   </td>
   <td>“north_america”, “global”, “global_land”
<p>
(multiple entries ok)
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV (list object)
   </td>
   <td>always
   </td>
   <td>See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_region.json">obs4MIPs_region.json</a>
   </td>
  </tr>
  <tr>
   <td><strong>source</strong>
<p>
<strong>(modified form)</strong>
   </td>
   <td>full observational dataset  name/version
   </td>
   <td>see <a href="#bookmark=id.r55y5lgk9uho">Appendix 2</a>
   </td>
   <td>source  
   </td>
   <td>CV (Generated from registered content)
   </td>
   <td>always
   </td>
   <td>More comprehensive than original obs4MIPs and CMIP5. See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/Tables/obs4MIPs_CV.json">Tables/obs4MIPs_CV.json</a> and search for source_id
   </td>
  </tr>
  <tr>
   <td><strong>source_id</strong>
<p>
<strong>(modified form)</strong>
   </td>
   <td>Observations identifier
   </td>
   <td>“GPCP-2-4-1”
<p>
See <a href="#bookmark=id.r55y5lgk9uho">Appendix 2</a>
   </td>
   <td>source_id
   </td>
   <td>CV (Generated from 
<p>
registered content)
   </td>
   <td>always
   </td>
   <td>Edited version of first part of “source” (with forbidden characters like spaces and periods replaced with hyphens); used in constructing the file name. See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_source_id.json">obs4MIPs_source_id.json</a> for examples
   </td>
  </tr>
  <tr>
   <td><strong>source_label</strong>
   </td>
   <td>label used to identify source (independent of source version)
   </td>
   <td>“GPCP”
<p>
See <a href="#bookmark=id.r55y5lgk9uho">Appendix 2</a>
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV with registered content
   </td>
   <td>always
   </td>
   <td>This should be the same as source_id, but without a version number. It will likely be used in faceted searches to get a truncated list of sources (without all the different versions listed)
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>source_type</strong>
   </td>
   <td>Observational class
   </td>
   <td> ‘satellite_retrieval’, ‘satellite_blended’,
<p>
“gridded_insitu”,
<p>
“reanalysis”
   </td>
   <td>Mixture of source_type and product
   </td>
   <td>CV
<p>
see Appendix 2
   </td>
   <td>always
   </td>
   <td>See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_source_type.json">obs4MIPs_source_type.json</a>.
<p>
Additional entries may be added over time
   </td>
  </tr>
  <tr>
   <td><strong>source_version_number</strong>
   </td>
   <td>Numeric version identifier 
   </td>
   <td>v1.0, 1.2
<p>
ver2.3.1
<p>
See <a href="#bookmark=id.r55y5lgk9uho">Appendix 2</a>
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>CV with registered content
   </td>
   <td>always
   </td>
   <td>See <a href="https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_source_id.json">obs4MIPs_source_id.json</a> and search for source_version_number
   </td>
  </tr>
  <tr>
   <td><strong>title</strong>
   </td>
   <td>see note 4
   </td>
   <td>see note 4
   </td>
   <td>title
   </td>
   <td>free form
   </td>
   <td>never
   </td>
   <td>no change; CF-convention standard
   </td>
  </tr>
  <tr>
   <td><strong>tracking_id </strong>
   </td>
   <td>unique file identifier
<p>
(automatically generated by CMOR)
   </td>
   <td>see note 14
   </td>
   <td>tracking_id
   </td>
   <td>structured form with some CV
   </td>
   <td>always
   </td>
   <td>Form modified to facilitate use by ESGF
   </td>
  </tr>
  <tr>
   <td><strong>variable_id</strong>
   </td>
   <td>variable identifier
   </td>
   <td>“tas”, “pr”, “ua”
   </td>
   <td>variable_id
   </td>
   <td>CV
   </td>
   <td>always
   </td>
   <td>Added to direct users and software to the primary variable of interest in the file. The complete list of CMIP6 variable_ids is <a href="http://clipc-services.ceda.ac.uk/dreq/index/CMORvar.html">here</a>
   </td>
  </tr>
  <tr>
   <td><strong>variant_info</strong>
   </td>
   <td>description of run variant
   </td>
   <td>“Best Estimate”,
<p>
“Sphere of influence = 20km”  See note 15
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>free form
   </td>
   <td>as appropriate
   </td>
   <td>Provides brief description of variant differences. Not needed in most cases, when there is only a “Best Estimate” (BE)
   </td>
  </tr>
  <tr>
   <td><strong>variant_label</strong>
   </td>
   <td>“variant” label
   </td>
   <td>Usually “BE” 
<p>
(for “Best Estimate”); rarely “r1”, “r2”, r123”
<p>
 See note 16
   </td>
   <td><strong><em>NEW</em></strong>
   </td>
   <td>structured form
   </td>
   <td>always
   </td>
   <td>In most cases the value is “BE”.  Only when there are multiple estimates of the same source_id (e.g., constructed with alternate processing choices) is the value different in which case it should follow CMIP6, e.g., with “BE”, “r1”, “r2”, “r3”, ...
   </td>
  </tr>
</table>


<span style="text-decoration:underline;">Table Notes:</span>

1. If CMOR is used to write output files (strongly recommended), an additional global attribute will automatically be included: cmor_version, but this is not an obs4MIPs required global attribute

2. “CV” means content must be taken from a “controlled vocabulary” defined by the WDAC’s task team in coordination with the WIP. “registered content” (RC) is special controlled vocabulary defined by data contributor and monitored by the obs4MIPs TT. Data contributors can submit RC at ([https://github.com/PCMDI/obs4MIPs-cmor-tables)](https://github.com/PCMDI/obs4MIPs-cmor-tables)) and contact obs4MIPs-admin@llnl.gov

3. For backwards compatibility with ODS V1, project_id will be an alias of activity_id on ESGF.

4. Since some software uses the ‘title’ for default plotting or describing the contents of a file, it can be used to provide a description that is similar or equivalent to the source. A common entry may be the same as the source but without the release_year. 

       

5. creation_date form: YYYY-MM-DDTHH:MM:SSZ  (e.g., “2010-03-23T05:56:23Z”)

6. further_info_url has the form 

https://furtherinfo.es-doc.org/&lt;activity_id>.&lt;institution_id>.&lt;source_label>.&lt;source_id>.&lt;variable_id>

(e.g., “https://furtherinfo.es-doc.org/obs4MIPs.RSS.REMSS-PRW[.](http://furtherinfo.es-doc.org/cmip6.MOHC.HadCM3.historical.none.r3i1p1f1)REMSS-PRW-6-6-0.prw”). The further_info_url page will be maintained by the ES-DOCs project and will simply be a rendering by the Viewer tool of information provided by modeling groups and recorded in so-called CIM documents.

7. The “grid” global attribute can be used to describe the horizontal grid and regridding procedure. There is no standard form used to record this information, but it is suggested that when appropriate the following be indicated: brief description of native grid and resolution, and if data have been regridded, regridding procedure and description of target grid.  Here are some examples:


        grid = “data regridded to a CMIP6 standard 1x1 degree latxlon grid from the native T63 grid using an area-average preserving method”


        grid = “data regridded via bilinear interpolation to a 3x3 deg latxlon grid from the native atmosphere T63 gaussian grid (64x128 latxlon)”


        grid = “data regridded to a CMIP6 standard 1x1 degree latxlon grid from the native T63 grid using an area-average preserving method”


        grid = “data regridded via bilinear interpolation to a 3x3 deg latxlon grid from the native atmosphere T63 gaussian grid (64x128 latxlon)”

8. Data providers may choose to report their output on one or more grids, or with special care provide an alternate projection. To distinguish between output reported on different grids, a “grid_label” attribute is defined. The original grid should be labeled with “gn”. Additional grids should be labeled using the form “gr[i]” where i is a positive integer. If the data is subsequently regridded to a second and third grid, “gr2” and “gr3” could be used to distinguish these grids from “gr1”.

9. A description and examples of the contact, comment, history and references global attributes may be found in the document: CMIP5_output_metadata_requirements ([http://cmip-pcmdi.llnl.gov/cmip5/docs/CMIP5_output_metadata_requirements.pdf](http://cmip-pcmdi.llnl.gov/cmip5/docs/CMIP5_output_metadata_requirements.pdf)).

13. The wording of the “license” attribute is up to the dataset creator, but it is recommended that you reference one of the “Creative Commons” licenses. Here is some possible text: “Data in this file produced by &lt;Your Centre Name> is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License ([https://creativecommons.org/licenses](https://creativecommons.org/licenses/)/). Use of the data must be acknowledged following guidelines found at &lt;a URL maintained by you>.  Further information about this data, including some limitations, can be found via &lt;some URL maintained by you>.”

14. tracking_id should be of the form hdl:21.14102/&lt;uuid> (e.g., “hdl:21.14102/02d9e6d5-9467-382e-8f9b-9300a64ac3cd”). The tracking_id should be unique for each file published in ESGF. CMOR automatically generates a tracking_id. You can review the python built-in UUID library documentation [here](https://docs.python.org/2/library/uuid.html).

15. Except when variant_label=”BE”, it is recommended that variant_info include information identifying major distinguishing features of a variant, but care should be taken to record correct information.

16. When multiple versions are provided with the same source_id, the first one should be labeled “r1” and all subsequent versions (derived from different processing choices) will follow the “realization nomenclature of CMIP with “r2”, “r3”, … “rN”.


# Data Reference Syntax (DRS) components:

The DRS is used, for example, in file names, directory structures, the further_info_url, and in facets of some search tools. The following components are needed for obs4MIPs:

activity_id	(original obs4MIPs "activity")

realm		(original obs4MIPs "activity")

frequency	(original obs4MIPs: "frequency")

product		(original obs4MIPs: "product")

institution_id	(original obs4MIPs: "institute")

source_id	(original obs4MIPs: "model")

source_label	(new in obs4MIPs)

variable_id	(original obs4MIPs: "variable name")

region		(new in obs4MIPs)

grid_label	(new in obs4MIPs)

variant_label	(original obs4MIPs: "ensemble member")

version		(original obs4MIPs: "version number")


# File name template:

The obs4MIPs file name must be constructed consistent with the following template.

**New obs4MIPs file name template =** 

**&lt;variable_id>_&lt;frequency>_&lt;source_id>_&lt;variant_label>_&lt;grid_label>[_&lt;time_range>].nc**

For time-invariant fields, the last segment (time_range) above is omitted.

All strings appearing in the file name are constructed using only the following characters: a-z, A-Z, 0-9, and the hyphen ("-"), except the hyphen must not appear in variable_id. Underscores are prohibited throughout except as shown in the template. \
 \
Note that the last segment of the file name indicates the time-range spanned by the data in the file, and is omitted when inappropriate. The format for this segment is the same as in CMIP6 (see Table 2 of the CMIP6 specs document: [http://goo.gl/v1drZl](http://goo.gl/v1drZl)). 

For comparison, here is the CMIP6 file name template:

&lt;variable_id>_&lt;table_id>_&lt;source_id>_&lt;experiment_id >_&lt;member_id>_&lt;grid_label>[_&lt;time_range>].nc

and the legacy obs4MIPs file name template:

&lt;_variable_>___&lt;_instrument_>__&lt;processing_level>__&lt;_processing version_>__&lt;start_date>_-&lt;_end_date_>.nc


# 


# Directory structure template:

The obs4MIPs directory structure must be constructed consistent with the following template.

**New obs4MIPs directory structure =**

**&lt;activity_id>/**

**&lt;institution_id>/**


    **&lt;source_id>/**


        **&lt;frequency>/**


            **&lt;variable_id>/**


                **&lt;grid_label>/**


                    **&lt;version>**

For comparison, here is the CMIP6 directory structure:

&lt;mip_era>/

&lt;activity_id>/


    &lt;institution_id>/


        &lt;source_id>/


            &lt;experiment_id>/


                &lt;member_id>/


                    &lt;table_id>/


                        &lt;variable_id>/


                            &lt;grid_label>/


                                &lt;version>

and the legacy obs4MIPs directory structure:

obs4MIPs/

observations/


    &lt;realm>/


        &lt;variable_id>/


            &lt;frequency>/


                &lt;grid>/


                    &lt;Institution_id>


                        &lt;instrument>/


                            &lt;version>/

<span style="text-decoration:underline;">Notes</span>:

&lt;version> here refers to the CMOR-assigned version number which has the form “vYYYYMMDD” (e.g., “v20170921”), indicating a representative date for the version was produced for obs4MIPs. For those not using CMOR, the convention must be followed.


# Sample file header {#sample-file-header}

The example below was produced from the following demo: [https://github.com/PCMDI/obs4MIPs-cmor-tables/demo](https://github.com/PCMDI/obs4MIPs-cmor-tables/tree/master/demo)

KEY:  yellow means "absolutely essential" 

netcdf prw_mon_REMSS-PRW-6-6-0_BE_gn_198701-198812 {

dimensions:

    time = UNLIMITED ; // (24 currently)

    lat = 72 ;

    lon = 144 ;

    bnds = 2 ;

variables:

    double time(time) ;

   	 time:bounds = "time_bnds" ;

   	 time:units = "days since 1987-1-1 0:0:0" ;

   	 time:calendar = "gregorian" ;

   	 time:axis = "T" ;

   	 time:long_name = "time" ;

   	 time:standard_name = "time" ;

    double time_bnds(time, bnds) ;

    double lat(lat) ;

   	 lat:bounds = "lat_bnds" ;

   	 lat:units = "degrees_north" ;

   	 lat:axis = "Y" ;

   	 lat:long_name = "latitude" ;

   	 lat:standard_name = "latitude" ;

    double lat_bnds(lat, bnds) ;

    double lon(lon) ;

   	 lon:bounds = "lon_bnds" ;

   	 lon:units = "degrees_east" ;

   	 lon:axis = "X" ;

   	 lon:long_name = "longitude" ;

   	 lon:standard_name = "longitude" ;

    double lon_bnds(lon, bnds) ;

    float prw(time, lat, lon) ;

   	 prw:standard_name = "atmosphere_water_vapor_content" ;

   	 prw:long_name = "Water Vapor Path" ;

   	 prw:comment = "vertically integrated through the atmospheric column" ;

   	 prw:units = "kg m-2" ;

   	 prw:cell_methods = "area: time: mean" ;

   	 prw:missing_value = 1.e+20f ;

   	 prw:_FillValue = 1.e+20f ;

   	 prw:valid_min = 2.f ;

   	 prw:valid_max = 3.f ;

// global attributes:


<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :Conventions = "CF-1.7 ODS-2.1" ;


<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :activity_id = "obs4MIPs" ;


<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :contact = "RSS (support@remss.com)" ;


<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :creation_date = "2017-11-08T20:36:13Z" ;


<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :data_specs_version = "2.1.0" ;


<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :frequency = "mon" ;


<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :further_info_url = "https://furtherinfo.es-doc.org/obs4MIPs.RSS.REMSS-PRW.REMSS-PRW-6-6-0.prw" ;


<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :grid = "2.5x2.5 degree latitude x longitude" ;


<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :grid_label = "gn" ;


<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :history = "2017-11-08T20:36:13Z; CMOR rewrote data to be consistent with obs4MIPs, and CF-1.7 ODS-2.1 standards" ;


<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :institution = "Remote Sensing Systems, Santa Rosa, CA 95401, USA" ;


<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :institution_id = "RSS" ;


<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :nominal_resolution = "250 km" ;


<p id="gdcalert23" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert24">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :product = "observations" ;


<p id="gdcalert24" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert25">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :realm = "atmos" ;


<p id="gdcalert25" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert26">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :region = "global" ;


<p id="gdcalert26" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert27">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :source = "REMSS-PRW 6.6.0 (2017): Water Vapor Path" ;


<p id="gdcalert27" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert28">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :source_id = "REMSS-PRW-6-6-0" ;


<p id="gdcalert28" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert29">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :source_label = "REMSS-PRW" ;


<p id="gdcalert29" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert30">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :source_type = "satellite_blended" ;


<p id="gdcalert30" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert31">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :source_version_number = "6.6.0" ;


<p id="gdcalert31" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert32">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :table_id = "obs4MIPs_Amon" ;


<p id="gdcalert32" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert33">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :table_info = "Creation Date:(04 October 2017) MD5:9516b952d4e1c5084ec8c8e481e6cf35" ;


<p id="gdcalert33" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert34">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :title = "PRW v6.6.0 prepared for obs4MIPs (ODS-v2.1.0)" ;


<p id="gdcalert34" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert35">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :tracking_id = "hdl:21.14102/0dc9218d-6923-4415-8fb0-93cd9fa734c1" ;


<p id="gdcalert35" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert36">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :variable_id = "prw" ;


<p id="gdcalert36" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert37">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :variant_info = "Best Estimate" ;


<p id="gdcalert37" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert38">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :variant_label = "BE" ;


<p id="gdcalert38" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert39">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :license = "Data in this file produced by &lt;Your Centre Name> is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License (https://creativecommons.org/licenses/). Use of the data must be acknowledged following guidelines found at &lt;a URL maintained by you>. Further information about this data, including some limitations, can be found via &lt;some URL maintained by you>" ;


<p id="gdcalert39" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert40">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


   	 :cmor_version = "3.2.8" ;

}


# Appendix 1: Coordinate bounds {#appendix-1-coordinate-bounds}

While climate models have grid cells with boundaries that have exact definitions allowing analysts to precisely compute area integrals (such as a domain average), they are often not well defined for gridded observational products. If the analyst wants to compute a similar integral from observations, the area associated with each gridded value must be estimated. We therefore recommend that the data provider include their own estimates of the latitude-longitude grid cell bounds from which the grid cell areas can be calculated (since they are most familiar with the data). This will help insure uniformity among different researchers analyzing the data.


# 


# Appendix 2: Guidance for defining and registering source information (product description)

**_We need 7 pieces of information from obs4MIPs data providers to enable search functioning and other services on ESGF. (Note that we are referring here to only the “source” information which collectively is used to identify a dataset; data providers will also need to register their institution, and if they are contributing a new variable, not already defined by CMIP6, they will need to register the variable.). The 7 attributes are listed below, each with 3 examples:_**

1. **source_name** ("brand name") of the dataset. (See below for further guidance.)

"REMSS PRW"

"GPCP"

"NOAA NCEI AVHRR NDVI"

2. **release_year **(year this version of the data was produced and made available; the year that the data was reformatted for obs4MIPs is irrelevant):   

"2017"

"2003"

“2013"

3.  **source_description** of the dataset which usually is simply an expansion of the acronyms or abbreviations appearing in source_name 

"Remote Sensing Systems precipitable water" 

"Global Precipitation Climatology Project"

"NOAA Nat Cent ... AVHRR Normalized difference vegetation index"

4. **source_version_number** of the dataset (following whatever convention the data provider prefers)

"V6.6.0"

"2.3"

"V4.0"

5.  **institution_id** (acronym(s) used to identify the institution, group, or consortium responsible for producing the data set) 


    "RSS"


    "UofMD"


    "NOAA NCEI"

6.  the **region** covered by the dataset (see [obs4MIPs_region.json](https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_region.json) for options; the smallest appropriate region among the options should be used)


    "global"


    "global_ocean"

"global_land" 

7.  the **source_type** (see [obs4MIPs_source_type.json ](https://github.com/PCMDI/obs4MIPs-cmor-tables/blob/master/obs4MIPs_source_type.json)for options)


    "gridded_insitu"


    "satellite_blended"


    "satellite_retrieval"

**_From the information above, the obs4MIPs team constructs the following 3 items:_**

8. **source_label** = &lt;source_name>, but substituting "-" for certain forbidden characters (including ".", “_”, “(“, “)”, “/”, and " ").  


    "REMSS-PRW"


    "GPCP"


    "NOAA-NCEI-AVHRR-NDVI"

9. **source_id** = &lt;source_label>-&lt;source_version_number> but substituting  "-" for certain forbidden characters (including ".", “_”, “(“, “)”, “/”, and " "). 


    "REMSS-PRW-6-6-0"


    "GPCP-2-3"


    "NOAA-NCEI-AVHRR-NDVI-4-0"

 10.  **source** = &lt;source_name> &lt;source_version_number> (&lt;release_year>): &lt;source_description>   

"REMSS PRW v6.6.0 (2017):  Remote Sensing Systems precipitable water"

"GPCP 2.3 (2003): Global Precipitation Climatology Project"

"NOAA NCEI AVHRR NDVI v4.0 (2013): NOAA Nat Cent ... AVHRR Normalized difference vegetation index"

In summary, data providers need to _register content_ for the following: 1) source_name, 2) release_year, 3) source_description, 4) source_version_number, 5) institution_id, 6) region and 7) source_type. They can do this by submitting an issue on the [obs4MIPs-cmor-tables github repository](https://github.com/PCMDI/obs4MIPs-cmor-tables). From this information the source_label, source_id and source are constructed. CMOR will record as global attributes all items except the first 3: source_name, release_year, and source_description (because they are included in "source").

**Notes:**



1. The _source_name _must be unique across all obs4MIPs datasets. It should be as short as possible because it appears in file names, directory structures, search lists, and the like.
2. For an existing dataset that is now being prepared for obs4MIPs, the _source_name_ might be an established name associated with the dataset and recognizable by the community (e.g., GPCP, GHCN). For new data sets that do not yet have a recognized brand name, _source_name_ might (but is not required to) include an acronym with some indication of: who the data provider is, what instrument the observations are based on, and/or the name of the observed variable. The _source_name_ should not be too generic because each separate contribution to obs4MIPs (current or future) must have a unique source_name. [If, for example, you are currently contributing a sea surface temperature dataset, but expect later to prepare a surface salinity dataset, you should anticipate that when constructing your source_name.  In this case you wouldn't want the source_name to just be the name of your group. Similarly, you wouldn't want your source name to be just the name of the variable because it is likely other groups will also want to contribute the same variable to obs4MIPs.] Consider what name you would like the dataset to be known by in the years to come.
3. If an obs4MIPs contribution includes multiple, related datasets (i.e., more than one variable), coming, for example, from a self-consistent analysis procedure, then all the variables would normally share a common source_name and source_version_ number.
4. If a single group plans to prepare multiple *unrelated* datasets, then each dataset should be assigned a different source_label. By "unrelated" we mean they would normally be independently assigned "release" (or version) numbers. If these multiple, unrelated datasets each deals with a different variable, then one option would be to include the variable name as part of the source_label, but this is not a requirement. The provider might have other ways to distinguish between these datasets.

Note: If a minor problem is found in obs4MIPs datasets (e.g., a mistake in one of the global attributes), the mistake can be corrected without issuing a new "release" with a new version. The data can be republished on ESGF, and ESGF's versioning system will hide the deprecated file(s) (and make it easy for users to determine whether they have the most up-to-date files).


# 


# Appendix 3: Document version information {#appendix-3-document-version-information}

0.1 (23 October, 2016) - Document initiated with CMIP6 analog. _Not public_

0.2 (23 October - 22 February 2017) - working on draft document in relation to CMIP6, CMIP5 and original obs4MIPs specs

0.3 (March 01 - April 05 2017) - Added “region” as global attribute, finessing Table 1 footnotes

0.4 (April 25) - Draft made public on obs4MIPs CoG site enabling broader feedback

2.0 beta (June 25) - Public on obs4MIPs CoG site

**[2.0 released (June 30, 2017)](https://docs.google.com/document/d/1NClSyjl0RMaj0poT0WoCSnVDen3-dTIabQBniQA8tbk/edit#) **

**2.1 released (September 22, 2017)**



* source_id now is a compound structure with source_label followed by the version number. Example: source_label=”GPCP”, source_id=”GPCP-2-4-1”. This is described in Appendix 2 
* table_id was eliminated since table names have very little meaning now in CMIP. “frequency” will be used in place of table name to distinguish between a variable sampled at different frequencies. This is expected to be more compatible with CMIP7
* source_version_number was added
* “region” is now a required attribute (so that we can populate a search facet)
* typos and links were corrected and clarifying text and links were added
* CMOR software has been incremented from 3.2.x to 3.2.7 with changes made to implement the revised specifications


