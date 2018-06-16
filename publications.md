---
layout: page
title: Publications
permalink: /publications/
---

<script type="text/javascript">

var ref_thesis = `
@phdthesis{brousset_thesis, \r\n
	author = "Brousset, Mathias", \r\n
	title  = "Simulation et rendu de vagues déferlantes", \r\n
	school = "Université de Poitiers", \r\n
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
	issn    = "0097-8493" \r\n
	}
`;

var ref_vp = `
	@inproceedings {Brousset15, \r\n
	title     = "A New Force Model for Controllable Breaking Waves", \r\n
	author    = "Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Poulin, Pierre and Crespin, Benoît", \r\n
	booktitle = "Workshop on Virtual Reality Interaction and Physical Simulation", \r\n
	editor    = "Fabrice Jaillet and Florence Zara and Gabriel Zachmann", \r\n
	year      = "2015", \r\n
	publisher = "The Eurographics Association", \r\n
	ISBN      = "978-3-905674-98-9", \r\n
	DOI       = "10.2312/vriphys.20151334" \r\n
}
`;

var ref_afig = `
@inproceedings{brousset_afig, \r\n
  TITLE       = "Un nouveau modèle pour la génération et le contrôle de vagues déferlantes", \r\n
  AUTHOR      = "Brousset, Mathias and Darles, Emmanuelle and Meneveaux, Daniel and Pierre, Poulin and Crespin, Benoît", \r\n
  URL         = "https://hal.archives-ouvertes.fr/hal-01255224", \r\n
  BOOKTITLE   = "Journées de l'AFIG", \r\n
  ADDRESS     = "Lyon, France", \r\n
  YEAR        = "2015", \r\n
  MONTH       = Nov, \r\n
  HAL_ID      = "hal-01255224",\r\n
  HAL_VERSION = "v1", \r\n
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
	case "afig":
		selected = ref_afig;
		break;
	}

	var input = $('<textarea>');
	$("body").append(input);
	var strcopy = input.val(selected).select();

	document.execCommand('copy');
	input.remove();
}

$(document).ready(function() {

	$("#toggle_thesis").click(function(){
		copyClipboard("thesis");
	});

	$("#toggle_cg").click(function(){
		copyClipboard("cg");
	});

	$("#toggle_vp").click(function(){
		copyClipboard("vp");
	});

	$("#toggle_afig").click(function(){
		copyClipboard("afig");
	});

});

</script>

|                                                 | Download preprint                                                                                                                    | Journal/Conf.                                                                              | Bibtex                                                                                          |
| :---------------------------------------------: | :--------------------------------------------------------------------:                                                               | :----------------------------------------------------------------------------------------: | :--------------:                                                                                |
| ![teaser vriphys](/images/teaser_thesis.png)    | [Simulation and Rendering of Breaking Waves](https://github.com/Mathiasb17/mathiasb17.github.io/raw/master/files/BROUSSET_THESE.pdf) | Thesis                                                                                     | <button id = "toggle_thesis" title="Reference copied to clipboard !">Copy to clipboard</button> |
| ![teaser cg](/images/teaser_cg16.png)           | [Simulation and Control of Breaking Waves using an External Force Model](/files/CG_2015_soliton_extended.pdf)                        | [C&G vol. 57](http://www.sciencedirect.com/science/article/pii/S0097849316300164)          | <button id = "toggle_cg" title="Reference copied to clipboard !">Copy to clipboard</button>     |
| ![teaser vriphys](/images/teaser_vriphys15.png) | [A New Force Model for Controllable Breaking Waves ](/files/CG_2015_soliton_extended.pdf)                                            | [VRIPHYS 2015](http://vriphys2015.sciencesconf.org/)                                       | <button id = "toggle_vp" title="Reference copied to clipboard !">Copy to clipboard</button>     |
| ![teaser vriphys](/images/teaser_vriphys15.png) | [Un nouveau modèle pour la génération et le contrôle de vagues déferlantes](/files/paper-AFIG-2015.pdf)                              | [AFIG 2015](https://projet.liris.cnrs.fr/afig2015/)                                        | <button id = "toggle_afig" title="Reference copied to clipboard !">Copy to clipboard</button>   |

<script>

tippy('button',
	{
		arrow : true,
		delay : 0,
		trigger : 'click',
		duration : 300,
		placement : 'right'
	});
</script>
