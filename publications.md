---
layout: page
title: Publications
permalink: /publications/
---

<script type="text/javascript">


var ref_thesis = `
@phdthesis{phdtheis, \n
	author = "Brousset, Mathias", \n
	title = "Simulation et rendu de vagues d\'eferlantes", \n
	school = "Universit\'e de Poitiers", \n
	year = "2017" \n
	}
`;

var ref_cg = `
@article{Brousset16, \n
	title   = "Simulation and control of breaking waves using an external force model", \n
	author  = "Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Poulin, Pierre and Crespin, Benoît", \n
	journal = "Computers & Graphics", \n
	volume  = "57", \n
	pages   = "102 - 111", \n
	year    = "2016", \n
	issn    = "0097-8493", \n
	}
`;

var ref_vp = `
	@inproceedings {Brousset15, \n
	title = {{A New Force Model for Controllable Breaking Waves}}, \n
	author = {Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Poulin, Pierre and Crespin, Benoît}, \n
	booktitle = {Workshop on Virtual Reality Interaction and Physical Simulation}, \n
	editor = {Fabrice Jaillet and Florence Zara and Gabriel Zachmann}, \n
	year = {2015}, \n
	publisher = {The Eurographics Association}, \n
	ISBN = {978-3-905674-98-9}, \n
	DOI = {10.2312/vriphys.20151334} \n
}
`;

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

	var input = $('<input>');
	var strcopy = input.val(selected).select();

	document.execCommand('copy');
}

</script>

|                                                 | Title                                                                  | Journal/Conf.                                                                                      | Status            | Link to Preprint                                                                                        | Bibtex                                                               |
| :---------------------------------------------: | :--------------------------------------------------------------------: | :----------------------------------------------------------------------------------------:         | :---------------: | :--------------:                                                                                        | :--------------:                                                     |
| ![teaser vriphys](/images/teaser_vriphys15.png) | Simulation and Rendering of Breaking Waves                             | Thesis                                                                                             | Passed            | [Download here](https://github.com/Mathiasb17/mathiasb17.github.io/raw/master/files/BROUSSET_THESE.pdf) | <button onclick="copyClipboard('thesis')">Copy to clipboard</button> |
| ![teaser cg](/images/teaser_cg16.png)           | Simulation and Control of Breaking Waves using an External Force Model | [Computers & Graphics vol. 57](http://www.sciencedirect.com/science/article/pii/S0097849316300164) | Published         | [Here](/files/CG_2015_soliton_extended.pdf)                                                             | <button onclick="copyClipboard('cg')">Copy to clipboard</button>     |
| ![teaser vriphys](/images/teaser_vriphys15.png) | A New Force Model for Controllable Breaking Waves                      | [VRIPHYS 2015](http://vriphys2015.sciencesconf.org/)                                               | Honorable Mention | [see extended paper here](/files/CG_2015_soliton_extended.pdf)                                          | <button onclick="copyClipboard('vp')">Copy to clipboard</button>     |
