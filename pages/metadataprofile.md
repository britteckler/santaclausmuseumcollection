---
title: Metadata Profile for The Santa Claus Museum & Village
layout: about
permalink: /metadataprofile.html
# include CollectionBuilder info at bottom
credits: true
---
{% include feature/jumbotron.html objectid="scmv_035" heading="About: Metadata Application Profile" text="The descriptive and bibliographic metadata for The Santa Claus Museum & Village." %} 

<div class="table-responsive">
<table class="table table-sm table-striped">

<thead>
<tr>
	<th><strong>Metadata</strong></th>
	<th><strong>Dublin Core Mapping</strong></th>
	<th><strong>Cardinality</strong></th>
	<th><strong>Obligation</strong></th>
	<th><strong>Content Guidelines</strong></th>
	<th><strong>Controlled Vocabulary</strong></th>
	<th><strong>Examples</strong></th>
	<th><strong>Notes</strong></th>
</tr>
</thead>

<tbody>
<tr>
	<td>objectid</td>
	<td>Identifier</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>A unique and unambiguous identification given to the resource. Follows the format: scmv_###</td>
	<td></td>
	<td><ul><li><code>scmv_001</code></li><li><code>scmv_016</code></li><li><code>scmv_024</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>filename</td>
	<td>Identifier</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>The unique identification given to a resource when uploaded to Github. To match the objectid, i.e., scmv_###.</td>
	<td></td>
	<td><ul><li><code>scmv_001</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>title</td>
	<td>Title</td>
	<td>Repeatable</td>
	<td>Mandatory</td>
	<td>A name given to the resource with the first letter of each word capitalized.</td>
	<td></td>
	<td>
		<ul>
			<li><code>Souvenir Fan</code></li>
			<li><code>December 1948 Dear Santa Letter from Friedley</code></li>
			<li><code>Photograph of Santa Jim Yellig and Band</code></li>
		</ul>
	</td>
	<td>If no proper title name can be given, context clues will be used to create a title.</td>
</tr>
<tr>
	<td>format</td>
	<td>Format</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>The file format of the digital object i.e., .JPG...Follow format on IANA </td>
	<td><a href="https://www.iana.org/assignments/media-types/media-types.xhtml">IANA Media Types</a></td>
	<td><ul><li><code>image/jpg</code></li><li><code>application/pdf</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>material</td>
	<td>Format</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>The physical material culture used to create the artifact. List the basic material item is made from.</td>
	<td><a href="https://www.getty.edu/research/tools/vocabularies/aat/index.html">AAT</a></td>
	<td><ul><li><code>Plastic</code></li><li><code>Wood</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>description</td>
	<td>Description</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>A concise and brief description of object item. Typically, 1 sentence in length, no more than 2 sentences.</td>
	<td></td>
	<td><ul><li><code>A souvenir fan from Santa Claus Land.</code></li><li><code>Program that reads: "United States 1963 Christmas Stamp Dedication Ceremony Santa Claus, Indiana November 1, 1963"</code></li><li><code>Dear Santa Letter written in German.</code></li>
	<td></td>
</tr>
<tr>
	<td>date</td>
	<td>Date</td>
	<td>Not Repeatable</td>
	<td>Mandatory, if applicable</td>
	<td>The year an artifact was originally manufactured or the year a Dear Santa Letter was written. "YYYY, YYYY-MM, or YYYY-MM-DD"</td>
	<td><a href="https://www.iso.org/iso-8601-date-and-time-format.html">ISO 8601</a></td>
	<td><ul><li><code>1952</code></li><li><code>1949-12-13</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>location</td>
	<td>Coverage</td>
	<td>Not Repeatable</td>
	<td>Mandatory, if applicable</td>
	<td>This field is for the Dear Santa Letters by children from various geographical locations. "City, Sate, Country" or "City, Country"</td>
	<td><a href="https://www.getty.edu/research/tools/vocabularies/tgn/index.html">TGN</a></td>
	<td><ul><li><code>Sandusky, Ohio, USA</code></li><li><code>Hamburg, Germany</code></li></ul></td>
	<td>Depending on letter or item we might not have detailed location information so a lot might just be "Santa Claus, Indiana" if more detailed locations are available then it will be provided as best as possible.</td>
</tr>
<tr>
	<td>creator</td>
	<td>Creator</td>
	<td>Repeatable</td>
	<td>Mandatory, if applicable</td>
	<td>The child who wrote the letter to Santa if applicable. Follows Last Name/Initial, First Name/Initial. If multiple names on one letter, names separated by semicolons and if no name, it will be left blank. For artifacts, creator will typically be Santa Claus Land.</td>
	<td></td>
	<td><ul><li><code>Friedley, Mary Ann</code></li><li><code>Santa Claus Land</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>display</td>
	<td>Coverage</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>The current location of an item - either on display or in storage. There are only two options to keep it simple and controlled: On Display or In Storage.</td>
	<td></td>
	<td><ul><li><code>In Storage</code></li><li><code>On Display</code></li></ul></td>
	<td>Some items within the collection are currently on display in the museum, this field is used to note if they are on display or are in storage. This field can be used to help with media inquiries if they need pictures of the item or more information.</td>
</tr>
<tr>
	<td>type</td>
	<td>Type</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>The type of the physical item. There is only two options currently for first iteration of collection: Physical Artifact or Text.</td>
	<td><a href="https://www.dublincore.org/specifications/dublin-core/dcmi-type-vocabulary/2003-02-12/">DCMI: Dublin Core™ Metadata Type Vocabulary</a></td>
	<td><ul><li><code>Physical Object</code></li><li><code>Comic Book Plus</code></li><li><code>Text</code></li></ul></td>
	<td></td>
</tr>
<tr>
	<td>rights</td>
	<td>Rights</td>
	<td>Repeatable</td>
	<td>Mandatory, if applicable</td>
	<td>A rights statement for select items.</td>
	<td><a href="http://rightsstatements.org/vocab/NKC/1.0/">Rights Statement</a></td>
	<td>"The organization that has made the Item available reasonably believes that the Item is not restricted by copyright or related rights, but a conclusive determination could not be made. Please refer to the organization that has made the Item available for more information. You are free to use this Item in any way that is permitted by the copyright and related rights legislation that applies to your use."</td>
	<td>The Santa Claus Museum owns photographs of the artifacts and digitized letters. Commercial status is unknown at this time.</td>
</tr>
<tr>
	<td>rightsstatement</td>
	<td>Rights</td>
	<td>Not Repeatable</td>
	<td>Mandatory</td>
	<td>A rights statement for select items.</td>
	<td><a href="https://rightsstatements.org">RightsStatements.org</a></td>
	<td></td>
	<td>The Santa Claus Museum owns photographs of the artifacts and digitized letters. Commercial status is unknown at this time.</td>
</tr></tbody></table></div>

