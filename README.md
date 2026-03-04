# EGDI Keyword Thesaurus
:soon: `latest version` -> see - **[v2.2](#version-22-2026)**   
:red_circle: `currently available at` https://resource.geosphere.at/graphdb/graphs  
:red_circle: `Sparql endpoint at` https://resource.geosphere.at/graphdb/repositories/keyword (REST API)  

A collection of ~2500 geoscientific terms in English (keywords), with unique web addresses (URIs), delivered in RDF format, with translations in different languages, with links to standardized codelists (INSPIRE, GeoSciML, GEMET), thesaurus like modeled in accordance with the search use case and metadata tagging in MICKA. Hosted in an EGDI central repository, online available via web API (Sparql) to drive search systems.
Deployed in versioned updates according to a governance workflow. 
___
## Version 1.0 (2019)
[GeoERA-Keyword-Thesaurus_v1](https://github.com/GeoEra-GIP/WP4-Semantics/blob/master/Keyword%20Thesaurus/GeoERA-Keyword-Thesaurus_1.0.zip)
includes a selection of evaluated and compiled vocabularies, mainly from resources like GEMET, INSPIRE or CGI - see our [report](https://geoera.eu/wp-content/uploads/2019/11/D4.2-GeoERA-Keyword-Thesaurus.pdf)
___
## Version 1.1 (2020)
**Release notes (draft 3.2.2020):**  

Fully translated into German language (where not English labels used)  
  
**1) Concepts merged, URI voided, and preserved name as hiddenLabel:**  
natural hazard category => natural hazard  
composition chemistry category => chemical composition  
resource assessment category => resource assessment   
aquifer type => aquifer  
geophysical station type => geophysical station rank => geophysical station  
energy type => energy  
soil layer type => soil layer  
spatial data service type => spatial data service  
geographic processing services => spatial data service  
Pan-European Code for Reporting of Exploration Results, Mineral Resources and Reserves (PERC) => PERC Code  
freshwater => fresh water

**2) Concepts renamed, URI changed, and preserved name as hiddenLabel:**  
exposed element category => exposed element  
reserve assessment category => reserve assessment   
exploration activity type => exploration activity  
active well type => active well   
aquifer media type => aquifer media  
anthropogenic geomorphologic feature type => anthropogenic geomorphologic feature   
geologic unit type => geologic unit  
commodity type => commodity   
geophysical campaign type => geophysical campaign  
geophysical station type => geophysical station  
human health and safety consequence type => human health and safety consequence  
fossil fuel type => fossil fuel  
mining activity type => mining activity  
mineral occurence type => mineral occurence  
mineral exploration activity type => mineral exploration activity  
natural geomorphologic feature type => natural geomorphologic feature  
natural hydrogeological object type => natural hydrogeological object  
geological objects collection type => geological objects collection  
curve model type => curve model  
controlled activity type => controlled activity  
oil, gas and chemicals appurtenance type => oil, gas and chemicals appurtenance  
thermal appurtenance type => thermal appurtenance  
water appurtenance type => water appurtenance  
soil plot type => soil plot  
resource type => data resource  
Norwegian Petroleum Directorate classification (NPD-2001) => NPD-2001  
mmonazite => monazite  
  
**3) Concepts only renamed**  
resource type => data resource  
processing activity type => mining activity process  
classification of spatial data services => geographic processing services  
metadata codelist => metadata  
climate and climatic change => climate  
geographic processing services => spatial data service  
land use categories of Hierarchical INSPIRE Land Use Classification System => HILUCS  
categories of Hierarchical Supplementary Regulation Code List (HSRCL) => HSRCL  
United States Geological Survey => USGS classification  
HREE => heavy rare-earth elements  
LREE => light rare-earth elements  
geographic communication services => communication service  
geographic human interaction services => human interaction service  
geographic data-structure viewer => data-structure viewer  
geographic spreadsheet viewer => spreadsheet viewer  
geographic symbol editor => symbol editor  
geographic model/information management service => model and information management service  
geographic processing services – metadata => geographic processing service  
geographic workflow/task management services = > workflow and task management service  
geographic processing services – thematic => thematic processing service  
geographic processing services – temporal => temporal processing service  
geographic processing services – spatial => spatial processing service  
flow => flow (member)  
processing => geophysical processing  
measurement => geophysical measurement  
interpretation => geophysical interpretation   
  
**4) Concepts deleted without substitution**  
topic categories in accordance with EN ISO 19115  
  
**5) Concepts newly created**  
vocabulary  
thesaurus  
codelist  

**6) New skos:broader**  
chemical composition => chemical property  
natural gas, oil, .. extraction => extraction   
Search category "Information System" partly rearranged  
  
**7) New search category**  
not yet  

**8) Correction of "displaced" INSPIRE mappings for ..**  
alluvial plain, anthropogenic geomorphologic feature, artificial drainage, artificial levee, borehole logging, cave, cone penetration test, flight line, geophysical measurement, geophysical profile, geophysical station, geophysical swath, georadar profile, hydroelectric energy, Ludfordian, multi-electrode dc profile, pond, renewable energy source, reservoir lake, river basin, seismic line, valley, watershed  
  
**Correction of "displaced" GEMET mappings for ..**  
global warming, greenhouse effect, ozone layer depletion, sea level rise, climatic change, climate change adaptation, climate change mitigation, climate change impact  
  
**9) Removed remaining commas or slashes from URIs**  
http://resource.geolba.ac.at/geoera_keyword/oil,-gas-and-chemicals-network-node => http://resource.geolba.ac.at/geoera_keyword/oil-gas-and-chemicals-network-node
___
## Version 2.0 (2020)
**Release notes (20.3.2020):**  

download latest version of **GeoERA Keyword Thesaurus** v2.0 at this GitHub page or directly from **European Geoscience Registry** at https://data.geoscience.earth/ncl/geoera/keyword  

**1) new URIs according to new EGS domain name:**  
All keyword concepts have got new identifiers based on the new domain name **"data.geoscience.earth"** registered by EGS. URI patterns are adapted to the naming conventions of geoscience.earth host. E.g. for the keyword ***hazard*** the URI was changed from previous testing environment ***http://resource.geolba.ac.at/geoera_keyword/hazard*** to ***https://data.geoscience.earth/ncl/geoera/keyword/1358***. The previous URIs remain in the Keyword Thesaurus to query with property "http://purl.org/dc/terms/replaces". As soon as the Keyword Thesaurus is in the registry all URIs will be resolvable at data.geoscience.earth. Meanwhile and for testing purposes we provide a [Sparql endpoint](https://resource.geolba.ac.at/PoolParty/sparql/keyword) to query the data base (triple store).

**2) Fully translated into Slovenian, Spanish and German language:**  
Initially the Keyword Thesaurus is already available in 4 languages. In some cases, no translation was carried out. Especially for abbreviations in international context.

**3) All previous changes included:**  
The Keyword Thesaurus now contains all modifications as described under v1.1 above.  

**4) All concepts under a single concept scheme:**  
Now all concepts are modelled under a single concepts scheme "keyword". Search categories are available as properties (dbPedia/category attributes) of almost each concept. Additionally Search categories have been changed from concept schemes in v1 to top concepts in v2.

**5) How to query a list of all keywords:**
Here an example how to get a table of all GeoERA keywords with URIs and translations into a selected language. Available languages are en, cs, da, el, de, es, et, fi, fr, hr, hu, is, it, lt, nl, no, pl, pt, ro, sk, sl, sv, uk.

The European Geoscience Registry shows the GeoERA Keyword Thesaurus v2 at https://data.geoscience.earth/ncl/geoera/keyword. By clicking around you should be able to navigate to each single keyword. But there is also a link to download a list of all available keywords in different formats. On the upper right you find download links for ttl, rdf/xml or json-ld. If you open the Sparql query form at https://data.geoscience.earth/ncl/ui/sparql-form you can run a query script to show the results in table, txt, json or xml. 
This code example below would generate a list of all keywords with URI and translations in Finnish (as many as already translated). If you want to fill the column in another language lets say Portuguese just change the filter for “**fi**” to “**pt**”.

```
prefix skos: <http://www.w3.org/2004/02/skos/core#>  
select distinct ?uri (str(?k) as ?keyword) (str(?t) as ?translation)  
(group_concat(?c;separator="; ") as ?categories)  
where {  
?uri a skos:Concept; skos:prefLabel ?k  
filter(regex(str(?uri), 'ncl/geoera/keyword'))  
filter(lang(?k)="en")  
optional{?uri skos:prefLabel ?t filter(lang(?t)="fi")}  
optional{?uri <http://dbpedia.org/ontology/category> ?c}  
}  
group by ?uri ?k ?t  
order by desc (?t)  
```

Scripts like above also could be (url encoded) embedded into URLs in order to get a file download. This method provides some different useful formats like CSV. 

https://data.geoscience.earth/ncl/system/query?query=prefix%20skos%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F2004%2F02%2Fskos%2Fcore%23%3E%0Aselect%20distinct%20%3Furi%20%28str%28%3Fk%29%20as%20%3Fkeyword%29%20%28str%28%3Ft%29%20as%20%3Ftranslation%29%20%28group_concat%28%3Fc%3Bseparator%3D%22%3B%20%22%29%20as%20%3Fcategories%29%0Awhere%20%7B%0A%3Furi%20a%20skos%3AConcept%3B%20skos%3AprefLabel%20%3Fk%0Afilter%28regex%28str%28%3Furi%29%2C%20%27ncl%2Fgeoera%2Fkeyword%27%29%29%0Afilter%28lang%28%3Fk%29%3D%22en%22%29%0Aoptional%7B%3Furi%20skos%3AprefLabel%20%3Ft%20filter%28lang%28%3Ft%29%3D%22fi%22%29%7D%0Aoptional%7B%3Furi%20%3Chttp%3A%2F%2Fdbpedia.org%2Fontology%2Fcategory%3E%20%3Fc%7D%0A%7D%0Agroup%20by%20%3Furi%20%3Fk%20%3Ft%0Aorder%20by%20desc%20%28%3Ft%29&format=text/csv

**Note**: special characters are always coded to utf-8 standard. Do not mistake with ANSI.  
___
## Version 2.1 (2021)
**Release notes (May 17, 2021):**  

**1) Concepts merged, URI voided, and preserved names as hiddenLabel:**  
mineral occurence (1204) => mineral occurrence (1195) - misspelling  
geophysical measurement (377) => geophysical measurement (405) - double entry  

**2) Concepts renamed, URI changed, and preserved name as hiddenLabel:**  
none  
**3) Concepts only renamed**  
acidic ingeous rock (53) -> acidic igneous rock  
arkoze -> arkose (88)  
foid diorte (13) -> foid diorite  
intergrated hydrological modelling (2477) -> integrated hydrological modelling  

**4) Concepts deleted without substitution**  
none  
**5) Concepts newly created**  
almost all new concepts were created in relation to the HIKE project to support the "Knowledge Sharepoint":  
Please find more details to this HIKE specific extension on https://gist.github.com/schmar00/ee728afd38969097d80c918a3a436dff   
  
helium (2561), Instaneous deformation (2562), facility failure (2563), explosions (2564), fluid spills (2565), leakage and migration along constrained path (2566), leakage and migration along unconstrained path (2567), Critical facilities out of use or malfunction (2568), Disruption of transportation (2569), Employment rate (2570), Biosphere impacts (2571), Atmospheric Impacts (2572), Anthropogenic causes (2573), Unconventional oil production (2574), Water production (2575), injection (2576), Fracking (2577), EOR (2578), Cyclic injection and extraction (2579), Geothermal doublet production (2580), Hydrogen storage (2581), Natural gas storage (2582), Nitrogen storage (2583), Compressed air energy storage (2584), engineering activities (2585), tunnel building (2586), solid earth (2587), rock falls (2588), atmospheric causes (2589), lightening (2590), interpreted datasets (2591), case studies (2592), instruments (2593), regional geological definitions (2594), basins (2595), oregenies (2596), shields (2597), stratigraphy (2598)  
  
**6) New skos:broader**  
none  
**7) New search category**  
none  
**8) Correction of "displaced" mappings**  
none  
**9) download a graphical display of v2.1**  
https://github.com/schmar00/keyword-thesaurus/blob/cf094666a23d23d20b275fa9b294bc1e4b647641/img/keywords_v21.pdf  

**published 2023 at**  
[![DOI](https://zenodo.org/badge/168712415.svg)](https://zenodo.org/doi/10.5281/zenodo.10057196) 
___
## Version 2.2 (2026)
**Release notes (minor release):**  
Additions to Thesaurus terms according to GSEU project, change of the base URI (domain name) urgently required for upcoming releases  

**Overview**

- Number of concepts: 2,752

- 16 categories 

- Number of supported languages: 27
    - 9 languages have a translation coverage of over 80% and are therefore suitable for use (see statistics below)
    - en (100%), de (99%), pt (98%), cs (98%), fi (93%), es (92%), sl (86%), hu (81%), it (80%), nl (65%), fr (34%), pl (34%), da (34%), lt (29%), et (29%), sk (29%), no (28%), sv (27%), hr (27%), ro (23%), el (23%), is (22%), uk (22%), sq (6%), sr (6%), bs (6%), mt (1%)  

**Changes Compared to Version 2.1:**

**1) Concepts merged, URI voided, and preserved name as hiddenLabel** <br>

"time-domain electromagnetic survey"@en: https://data.geoscience.earth/ncl/geoera/keyword/375 (skos:prefLabel) and https://data.geoscience.earth/ncl/geoera/keyword/2742 (skos:hiddenLabel)


**2) Concepts renamed, preserved name as altLabel or related** <br>

"HILUCS" (1530) - prefLabel@de changed from "HILUCS" into "Landnutzungskategorien des hierarchischen INSPIRE-Landnutzungsklassifizierungssystems" and preserved as altLabel@de

"CO2 storage" (2391)  prefLabel@en changed into "carbon storage" and preserved as altLabel@en

"Thermal capacity" (2425) prefLabel@en  changed into "thermal heat capacity" under category Geothermal Energy and skos:related to newly created "Thermal capacity" (2739 - GSEU-WP3 keyword) below geological information within Linked Data Terms Category


**3) Concepts only renamed** <br>

"other use" (1552) pref label@en changed into "other land use" 

 

**4) Concepts deleted without substitution** <br>
None

**5) Concepts newly created** <br>

156 added concepts, mostly provided by GSEU-WP3 Geoenergy group

4D seismic survey (2753),  Abandoned well (2599),  Active project (2601),  aquifer depth (2602),  Aquifer Thermal Energy Storage (2603),  Arias intensity (2604),  Borehole Thermal Energy Storage (2605),  Bottomhole pressure (2606),  Brine (2607),  carbon capture (2610),  carbon capture and storage (2750),  carbon capture and storage infrastructure (2608),  Closed project (2609),  CO2 leakage (2611),  CO2 thermal energy storage (2613),  CO2 transport (2612),  coking coal (2754),  commercial capacity (2614),  Conductive heat (2615),  Construction phase (2616),  Convective heat (2617),  DC resistivity (2618),  Debris flow (2619),  deep geothermal energy (2620),  Demonstration phase (2621),  Depleted gas field (2622),  Depleted oil field (2623),  Development phase (2624),  direct air capture and storage (2625),  dynamic capacity (2626),  Dynamic model (2627),  Earthquake intensity (2628),  Earthquake magnitude (2751),  Earthquake parameters (2629),  Effective porosity (2630),  electromagnetic survey (2631),  emission points (2632),  energy infrastructure (2633),  energy output (2634),  enhanced geothermal system (2635),  Enhanced Oil Recovery (2636),  Enthalpy (2637),  environmental conflicts (2638),  environmental protected areas (2639),  Epicentre (2640),  exploitation permitting (2641),  Exploitation phase (2752),  Exploitation potential (2642),  exploration permitting (2643),  Exploration phase (2644),  extractable heat (2645),  Fluid chemistry (2646),  Fluid physical properties (2647),  Fluid temperature (2648),  geoenergy hazard (2650),  Geological cross section (2651),  geological information (2652),  geological pressure (2653),  Geothermal modelling (2654),  geothermal powerplant (2655),  ground penetrating radar (2656),  Groundwater composition monitoring (2657),  groundwater heat exchanger (2658),  Groundwater temperature (2659),  Hard rock cave (2660),  Heat flow (2661),  Heat in place (2662),  heat transfer (2663),  heating potential (2664),  Hot dry rock (2665),  Hot dry rock system (2666),  hydraulic stimulation (2667),  Hydrogeothermal (2668),  hydrogeothermal regions (2669),  hydrological feature (2670),  hydrostatic pressure (2671),  hydrothermal system (2672),  Hypocentre (2673),  induced polarization (2674),  injection points (2675),  injection rate (2676),  injection zone (2677),  injectivity (2678),  isotherms (2679),  leakage pathway (2680),  limitations of use (2681),  lithium brine (2682),  lithostatic pressure (2683),  migration (2684),  mine thermal energy storage (2685),  mineral scaling (2686),  mineralisation (2687),  monitoring well (2688),  multi channel surface wave analysis (2689),  net aquifer thickness (2690),  offshore and onshore area (2755),  offshore and onshore mining (2757),  offshore area (2691),  onshore area (2756),  original oil in place (2692),  orphan wells (2693),  passive seismic survey (2694),  peak ground acceleration (2695),  Pilot phase (2696),  pipeline terminals (2697),  Plant decommissioning (2698),  pore pressure (2699),  Primary porosity (2700),  Project status (2701),  prospective area (2702),  regional aquifer (2703),  regulatory requirements (2704),  renewable accelerated areas (2705),  renewable thermal energy (2706),  reservoir depth (2707),  reservoir flow rate (2708),  reservoir pressure (2709),  reservoir thickness (2710),  resistivity contact (2711),  rock-fluid interaction (2712),  saline aquifer (2713),  salt cavern (2714),  seal efficiency (2715),  seal properties (2716),  seismic reflection (2717),  seismic refraction (2718),  seismic site effects (2719),  seismic survey (2720),  seismic tomography (2721),  self-potential (2722),  soil gas monitoring (2723),  spill point (2724),  Static model (2725),  storage capacity (2726),  storage efficency (2727),  storage potential (2728),  storage readiness level (2729),  stratigraphic trap (2730),  structural trap (2731),  subsoil classes (2732),  surface rupture (2733),  technical potential (2734),  temporal underground storage (2735),  temporary underground gas storage (2736),  theoretical potential (2737),  theorical capacity (2738),  thermal capacity (2739),  thermal conductivity (2740),  thermophysical data (2741),  trans-national (2743),  trap (2744),  underground thermal energy storage (2745),  very low frequency electromagnetic survey (2746),  volumetric capacity (2747),  water chemistry (2748),  wellhead pressure (2749)

**6) New ScopeNotes**
"GSEU-WP3" remark for all newly implemented GSEU-WP3 keywords


**7) New skos:broader** <br>
Only regarding to newly imported keywords

**8) New search category** <br>
None

**9) Mappings to INSPIRE and/or GEMET**  <br>

- No - INSPIRE mappings are not added to the new created concepts in this release
- No - GEMET mappings are not added to the new created concepts in this release

**10) Correction of "displaced" INSPIRE mappings** <br>
None

**11) Correction of "displaced" GEMET mappings** <br>
None

**12) Removed remaining commas or slashes from URIs** <br>
None


**13) Translation into other languages (ISO 639-1 codes)** <br>
<br>
bs, cs, da, de, el, en, es, et, fi, fr, hr, hu, is, it, lt, mt, nl, no, pl, pt, ro, sk, sl, sq, sr, sv, uk
(new added languages in Vs. 2.2 are sq, sr, mt, bs)
⚠️ Note: Translation coverage is incomplete. Not all keyword concepts are available in all listed languages.


**14) Open Issues** <br>
1. governance
- discussion on a potential new base URI for a general EGDI keyword vocabulary is ongoing  
- use case description - requested contributions from the EGS-SIEG Editorial Board
 
2. content
- overlapping labels
- incomplete language coverage



**15) Outlook Keyword Thesaurus** <br>

A future major release in form of an EGDI keyword vocabulary is planned, potentially including:
- a new base URI (subject to EGDI approval)  

**published 2026 at**  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18868253.svg)](https://doi.org/10.5281/zenodo.18868253)  




  






