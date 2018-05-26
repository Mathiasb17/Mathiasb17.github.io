---
layout: page
title: Publications
permalink: /publications/
---

<script type="text/javascript">


var ref_thesis = `
@phdthesis{phdtheis, \r\n
	author = "Brousset, Mathias", \r\n
	title  = "Simulation et rendu de vagues d\'eferlantes", \r\n
	school = "Universit\'e de Poitiers", \r\n
	year   = "2017" \r\n
	}
`;

var ref_cg = `
@article{Brousset16, \r\n
	title   = "Simulation and control of breaking waves using an external force model", \r\n
	author  = "Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Poulin, Pierre and Crespin, Benoît", \r\n
	journal = "Computers & Graphics", \r\n
	volume  = "57", \r\n
	pages   = "102 - 111", \r\n
	year    = "2016", \r\n
	issn    = "0097-8493", \r\n
	}
`;

var ref_vp = `
	@inproceedings {Brousset15, \r\n
	title = {{A New Force Model for Controllable Breaking Waves}}, \r\n
	author = {Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Poulin, Pierre and Crespin, Benoît}, \r\n
	booktitle = {Workshop on Virtual Reality Interaction and Physical Simulation}, \r\n
	editor = {Fabrice Jaillet and Florence Zara and Gabriel Zachmann}, \r\n
	year = {2015}, \r\n
	publisher = {The Eurographics Association}, \r\n
	ISBN = {978-3-905674-98-9}, \r\n
	DOI = {10.2312/vriphys.20151334} \r\n
}
`;

$(document).ready(function() {
	$("#toggle_thesis").click(function(){
		copyClipboard("thesis");
		$("#toggle_thesis").effect("shake");
	});
	$("#toggle_cg").click(function(){
		copyClipboard("cg");
		$("#toggle_cg").effect("shake");
	});
	$("#toggle_vp").click(function(){
		copyClipboard("vp");
		$("#toggle_vp").effect("shake");
	});
});

function copyClipboard(article)
{
	var selected = "";
	switch(article)
	{
	case "thesis":
		selected = ref_thesis;
		break;
	case "cg":
		selected = ref_cg;
		break;
	case "vp":
		selected = ref_vp;
		break;
	}

	var input = $('<textarea>');
	var strcopy = input.val(selected).select();

	input.remove();
	document.execCommand('copy');
}

</script>

|                                                 | Title                                                                  | Journal/Conf.                                                                                      | Status            | Link to Preprint                                                                                        | Bibtex                                                  |
| :---------------------------------------------: | :--------------------------------------------------------------------: | :----------------------------------------------------------------------------------------:         | :---------------: | :--------------:                                                                                        | :--------------:                                        |
| ![teaser vriphys](/images/teaser_vriphys15.png) | Simulation and Rendering of Breaking Waves                             | Thesis                                                                                             | Passed            | [Download here](https://github.com/Mathiasb17/mathiasb17.github.io/raw/master/files/BROUSSET_THESE.pdf) | <button id = "toggle_thesis">Copy to clipboard</button> |
| ![teaser cg](/images/teaser_cg16.png)           | Simulation and Control of Breaking Waves using an External Force Model | [Computers & Graphics vol. 57](http://www.sciencedirect.com/science/article/pii/S0097849316300164) | Published         | [Here](/files/CG_2015_soliton_extended.pdf)                                                             | <button id = "toggle_cg">Copy to clipboard</button>     |
| ![teaser vriphys](/images/teaser_vriphys15.png) | A New Force Model for Controllable Breaking Waves                      | [VRIPHYS 2015](http://vriphys2015.sciencesconf.org/)                                               | Honorable Mention | [see extended paper here](/files/CG_2015_soliton_extended.pdf)                                          | <button id = "toggle_vp">Copy to clipboard</button>     |
