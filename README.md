# Analysis Of Moja Global Datasets To Evaluate Crossriver Forest In Nigeria


# **DATASETS GUIDE**

> Note that this compilation is focused in datasets that include Nigeria, Africa.

1. **Adminitrative Boundaries**

  NOTE: The first 2 geodataframes are **NOT HOSTED IN THE MOJA GOBAL DATASET**. They below to Level 0 adminitration boundaries.

  * `world_df` - **World boundaries** - (Level 0, data source: [Natural Earth](https://www.naturalearthdata.com/downloads/110m-cultural-vectors/110m-admin-0-boundary-lines/))
  * `africa_df` - **Africa boundaries** - Clipped from (*world_df*).
  * `boundary_df` - **Nigeria boundaries** (Level 2, data source: [OpenStreetMap](https://planet.openstreetmap.org/)
    * `crossriverboundary_df` - **boundary of Crossriver State** (Level 4, data source : same as 1)
    * `regionsBoundary_df` - **boundary of Crossriver State**

2. **Soil resources**

  The dataset uses the World Referece Base ([WBR](https://www.fao.org/soils-portal/data-hub/soil-classification/world-reference-base/en/)) which is the international standard for soil classification system endorsed by the International Union of Soil Sciences, this system also includes a modern soil classification concepts and [USDA Soil Taxonomy](https://www.fao.org/soils-portal/data-hub/soil-classification/usda-soil-taxonomy/en/). 

  * `soil_df` - **World soil resources** (data source: World Soil Resources Coverage in Geographic Projection (ARC/Info Export format) "wsrll" Reports from [FAO](https://www.fao.org/soils-portal/data-hub/soil-maps-and-databases/other-global-soil-maps-and-databases/en/))
  * `africasoil_df` - **Africa soil resources** clipped from the *World soil resources* (above).
  * `Nigeriansoil1_df` - **Nigeria soil resources** (data source: same as *World soil resources*)
    * `CrossriverSoil_df` - **Soil resources of Crossriver**
    * `regionSoil_df` - **Soil resources of Crossriver**

3. **Biodiversity Hotspots** Contains information of the 36 recognzed bioidiversity hotspots in the earth. Contains a lot of biodiversity criteria , this dataaset focus on endemism on many plants species.
  * `bioHot_df` - **World Biodiversity Hotspots** (data source: [Zenodo](https://zenodo.org/record/3261807#.YX9zib_MK03))
  * `AfricaBioHot_df` - **Africa Biodiversity Hotspots** clipped from the (*bioHot_df*)
  * `NigeriaBioHot_df` - **Nigeria Biodiversity Hotspots** clipped from the (*bioHot_df*)
    * `CrossriverBioHot_df` - **Biodiversity Hotspots of Crossriver** clipped from the (*bioHot_df*)
    * `regionsBioHot_df` - **Biodiversity Hotspots of Crossriver** clipped from the (*bioHot_df*)

4. **Bioclimatic and ecological zones**  This dataset has developed over the years from covering only the tropical areas (1990) to the globe (2000), due constant changes in climate and landcover, a new map where develoaped in 2010 (the one is loaded in this notebook).

5. **Agro ecological zones.**  The GAEZ programs utilize the land resources inventory to assess all feasible agricultural land-use options and to quantify expected production of cropping activities relevant in a particular agro-ecological context, for specified management conditions and levels of inputs. The characterization of land resources includes all relevant components of climate, soils and landform, which are basic for the supply of water, energy, nutrients and physical support to plants.) Support for the used codes from the [documentation](https://webarchive.iiasa.ac.at/Research/LUC/GAEZv3.0/docs/GAEZ_User_Guide.pdf) (pag 49).
  * `agroEco_df` - **World Agro ecological zones** (data source: [The Global Agro‐Ecological Zones system (GAEZ) developed by the FAO](https://webarchive.iiasa.ac.at/Research/LUC/GAEZv3.0/))
  * `africaagroEco_df` - **Agro ecological zones of Africa** clipped from the (*agroEco_df*).
  * `NigeriaagroEco_df` - **Agro ecological zones of Nigeria**, clipped from the (*agroEco_df*).
    * `crossriveragroEco_df` - **Agro ecological zones of Crossriver** clipped from the (*agroEco_df*).
    * `regionsagroEco_df` - **Agro ecological zones of Crossriver**, clipped from the (*agroEco_df*).

6. **Planted Forest.** Taken from the Spatial Database of Planted Trees (SDPT), compiled by Global Forest Watch using data obtained from national governments, non-governmental organizations and independent researchers). Also, some features where review from the [documentation](https://www.wri.org/research/spatial-database-planted-trees-sdpt-version-10).
  * `forest_df`- **Planted Forest in Peru** (data source: [Arcgis](https://www.arcgis.com/home/item.html?id=224e00192f6d408fa5147bbfc13b62dd))

7. **Climate zones.** Based on the classification of IPCC.The zones are defined by a set of rules based on : annual mean daily, temperature, total annual precipitation, total annual potential evapo-transpiration (PET) and elevation. Extra featuures where revied from the [documentation](https://maps3.arcgisonline.com/arcgis/rest/services/A-16/Koeppen-Geiger_Observed_and_Predicted_Climate_Shifts/MapServer).
  
  Class names labels where collected from the [Guidelines for the calculation of land carbon stocks for the purpose of Annex V to Directive 2009/28/EC](https://eur-lex.europa.eu/LexUriServ/LexUriServ.do?uri=OJ:L:2010:151:0019:0041:EN:PDF) (Page 3).

  * `climate_df` - **World Climate zones** (data source: The [Climatic Zone layer](https://esdac.jrc.ec.europa.eu/projects/RenewableEnergy/).
  * `africaClimate_df` - **Climate zones of Africa** clipped from the (*climate_df*).
  * `NigeriaClimate_df` - **Climatic zones of Nigeria**, clipped from the (*climate_df*).
    * `crossriverClimate_df` - **Climatic zones of Crossriver state** clipped from the (*climate_df*).
    * `regionsClimate_df` - **Climatic zones of Crossriver state**, clipped from the (*climate_df*).
