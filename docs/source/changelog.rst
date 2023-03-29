
.. figure:: /images/changelog.png
   :alt: Alex Configuration
   :scale: 60%
   :align: center



**CLO Changelog**
=================


v4.1.1, February, 2022
----------------------

-   Added **GetNestingTime** call in PatternAPI to get the time of running the Nesting feature via API
-   Added **StopNesting** call in PatternAPI to stop nesting feature via API
-   Added **SetSchematicSilhouetteLineWidth** call in UtilityAPI to set schematic silhouette line width value via API 
-   Added **SetSchematicSeamlineWidth** call in UtilityAPI to set schematic seamline width value via API
-   Added **SetSchematicInternalLineWidth** call in UtilityAPI to set schematic internal line width value via API
-   Added **SetSchematicTopstitchLineScalePercent** call in UtilityAPI to set schematic topstitch line scale percent value via API
-   Added **SetSchematicSBrightness** call in UtilityAPI to set schematic brightness value via API
-   Added **SetSchematicSilhouetteLine** call in UtilityAPI to set schematic silhouette value via API
-   Added **SetSchematicSeamLine** call in UtilityAPI to set schematic seamline value via API
-   Added **SetSchematicInternalLine** call in UtilityAPI to set schematic internal line value via API
-   Added **SetSchematicTopstitchLine** call in UtilityAPI to set schematic topstitch line value via API
-   Added **SetSchematicClothRenderType** call in UtilityAPI to set schematic cloth rendering type via API
-   Added **SetStyleLineColor** call in UtilityAPI to set Style Line Color via API
-   Added **SetSchematicClothColor** call in UtilityAPI to set schematic cloth color via API
-   Added **Setcurrentfabric** call in FabricAPI to set schematic cloth color via API
-   Fixed issues where library window tab items were duplicating continuously 
-   Fixed issues where tab switching issue in Library Window
-   Fixed issues where add colorsawtch behavior changed 
-   Fixed issues where setting fabric APIs does not work if called continuously


v4.1.0, December, 2022
----------------------

-   Added **GetCurrentStatusofAvatar** call in UtilityAPI to get current status of avatar via API 
-   Added **GetSchematicRenderStatus** call in UtilityAPI to get status of schematic render via API 
-   Added **ImportOBJ** call in UtilityAPI to importobj with more option via API 
-   Added **SETFabricColor** call in FabricAPI to set fabric color via API 
-   Added **SetUseSameMaterialasFront** call in UtilityAPI to set same materials as front on different sides via API 
-   Added **Set3DviewwithIndex** call in UtilityAPI to set 3Dview with Index via API 
-   Added **Get/SetStrainStressMap** call in UtilityAPI to get/set strain and stress map via API 
-   Added **RefreshAPI** call in UtilityAPI to refresh APIs via API 


v4.0.4, November, 2022
----------------------
- Fixed maps rotating issue when using export glB/glTF API in Mac M1

v4.0.3, October, 2022
---------------------

-   Added **SetAnimationRecording** call in UtilityAPI to set animation recording via API 
-   Added **Get/SetCurrentAnimationFrame** call in UtilityAPI to get/set current status of the animation frame via API 
-   Added **GetStart/EndAnimationFrame** call in UtililtyAPI to get Start and the End of the Animation frames via API 
-   Added **More Options** within ImportExportOption when calling import FBX and glTF via API. 
	- bAutoTranslate
	- bCreateCamera
	- bCreateAnimation
	- bCreateCacheAniamtion
	- bMoveGarment
	- bAddArrangementPoints
	- bAutoCreateFittingSuit
	- bAdd
-   Added **ImportSMP** call in ImportAPI to import in SMP files via API  
-   Added **ImportSubstanceFileAsFaceType** call in UtilityAPI to set Substance Materials on different faces via API 
-   Added **ExportAVT** call in ExportAPI to export as AVT via API 
-   Added **PatternAnnotation** call in PatternAPI to get/set pattern annotation via API  
-   Added **SetSubstanceProperties** call in FabricAPI to set Texture Mapping, Preset, Resolution via API 
-   Fixed Issues where Zpac was not loaded properly via Importfile API in Headless Mode

v4.0.2, August, 2022
--------------------

-   Added **ImportFileByObjType** call in ImportAPI to import external 3D formats with their types(Avatar/Trim) via API 
-   Added **SetAvatarBodyTexture** call in UtilityAPI to change Avatar textures via API
-   Added **Get/SetFabricWidth** call in FabricAPI to get information of Fabric Width via API
-   Added **GetFabricLength** call in FabricAPI to get information of Fabric Length via API
-   Added **StartNesting** call in UtilityAPI to start the Nesting via API
-   Added **Set/GetNestingBufferSpacing** call in UtilityAPI to get and set informaiton for buffer spacing of nesting via API
-   Added **Get/SetNestingTargetColorway** call in UtilityAPI to get and set target colorway index via API
-   Added **Get/SetNestingPatternPieceGrainDirection** call in PatternAPI to get information of Grain on Pattern via API
-   Added **Get/SetNestingFixedPatternPiecePos** call in PatternAPI to get fixed position of pattern piece via API

v4.0.1, July, 2022
------------------

-   Added **ImportAVAC** call in ImportAPI to import Alvanon avatar via API 
-   Added **CreatePatternWithPoint** call in PatternAPI to create pattern via API

v4.0.0, June, 2022
------------------

- PatternAPI 
     - Added **Copy Pattern Piece Position** call in PatternAPI
     - Added **Copy Pattern Piece Move** call in PatternAPI
     - Added **Delete Pattern Piece** call in PatternAPI
     - Added **Delete Line** call in PatternAPI
     - Added **Delete Point** call in PatternAPI
     - Added **Flip Pattern Piece** call in PatternAPI
     - Added **Layer Clone Pattern Piece Position** call in PatternAPI
     - Added **Layer Clone Pattern Peice Move** call in PatternAPI
     - Added **Offset as Internal Line** call in PatternAPI
     - Added **Unfold Pattern Piece** call in PatternAPI
     - Added **Convert to Base Line** call in PatternAPI
     - Added **Convert to Internal Line** call in PatternAPI
     - Added **Distibute Internal Lines Between Segments** call in PatternAPI
     - Added **Get/Set Pattern Piece Position** call in PatternAPI
     - Added **Set Pattern Piece Move** call in PatternAPI
     - Added **Elastic** call in PatternAPI
     - Added **Elastic Strength** call in PatternAPI
     - Added **Elastic Strength Ratio** call in PatternAPI
     - Added **Elastic Segment Length** call in PatternAPI
     - Added **Elastic Total Length** call in PatternAPI
     - Added **Shrring** call in PatternAPI
     - Added **Shirring Interval** call in PatternAPI
     - Added **Shirring Height** call in PatternAPI
     - Added **Shirring Extend** call in PatternAPI
     - Added **Seamtaping** call in PatternAPI
     - Added **Seamtaping Width** call in PatternAPI
     - Added **Pattern Piece Info** call in PatternAPI
     - Added **Pattern Piece Fabric Style Info** call in PatternAPI
     - Added **Pattern Piece Solidify Info** call in PatternAPI
     - Added **Get Fabric Style Name List** call in PatternAPI
     - Added **Get/Set Pattern Layer** call in PatternAPI
     - Added **Set Pattern Strengthen** call in PatternAPI
     - Added **Set Pattern Lock** call in PatternAPI
     - Added **Set Pattern Hide** call in PatternAPI
     - Added **Set Pattern Lock** call in PatternAPI
     - Added **Set Pattern Hide 3D** call in PatternAPI
     - Added **Set Pattern Freeze** call in PatternAPI
     - Added **Add Segment Topstitch** call in PatternAPI
     - Added **Get Topstitch Style list** call in PatternAPI
     - Added **Get Pattern Assigned Topstitch Count/Style/StyleIndex** call in PatternAPI
     - Added **Set Pattern Assigned Toptstich Style** call in PatternAPI
     - Added **Is/Set Pattern Assigned Topstitch Extend Start** call in PatternAPI
     - Added **Is/Set Pattern Assigned Topstitch Extend End** call in PatternAPI
     - Added **Is/Set Pattern Assigned Topstitch Curved** call in PatternAPI
     - Added **Get/Set Pattern Assigned Toptstitch Curved Length** call in PatternAPI
     - Added **Is/Set Pattern Assigned Topstitch Curved Right Angled** call in PatternAPI
     - Added **Get/Set Pattern Assigned Topstitch Zoffset** call in PatternAPI
     - Added **Import Topstitch Style** call in PatternAPI
- Utility API
     - Added **Import Graphic Styles** call in UtilityAPI
     - Added **Replace Graphic Styles** call in UtilityAPI
     - Added **Simulate** call in UtilityAPI
     - Added **SetSimulationQuality** call in UtilityAPI
     - Added **SetSimulationTimestep** call in UtilityAPI
     - Added **SetSimulationNumberofSimulation** call in UtilityAPI
     - Added **SetSimulationCGFinishCondition** call in UtilityAPI
     - Added **SetSimulationCGIterationCount** call in UtilityAPI
     - Added **SetSimulationSelfCollisionIterationCount** call in UtilityAPI
     - Added **SetSimulationAirDamping** call in UtilityAPI
     - Added **SetSimulationGravity** call in UtilityAPI
     - Added **SetSimulationNumberOfCPUInUse** call in UtilityAPI
     - Added **SetSimulationCGResidual** call in UtilityAPI
     - Added **SetSimulationGroundCollision** call in UtilityAPI
     - Added **SetSimulationGroundHeight** call in UtilityAPI
     - Added **SetSimulationSelfCollisionAvoidanceStiffness** call in UtilityAPI
     - Added **SetSimulationLayerBasedCollisionDetection** call in UtilityAPI
     - Added **SetSimulationNonlinearSimulation** call in UtilityAPI
     - Added **SetSimulationNonlinearSimulation** call in UtilityAPI
- Import API
     - Added **ImportSubstanceFile** call in Import API 

v3.2.2, April, 2022
-------------------

-   Added **DeleteColorway** call in UtilityAPI to delete colorways with Index via API 

v3.2.1, January, 2022 
---------------------

-   Added **ExportFBX** call in ExportAPI to Export FBX files via API 

v3.2.0, December 2021 
---------------------

-   Added **ImportDXF** call in ImportAPI to Import DXF files via API 
-   Added **GetPatternPieceArea** call in PatternAPI to Get the Area of a Pattern Piece via API 
-   Added **GetLineLength** call in PatternAPI to Get the Line Length via API 
-   Added **GetPatternInputInformation** call in PatternAPI to Get the Information of a Pattern Piece via API 
-   Added **GetPattern/PatternsBoundingBox** call in PatternAPI to Get the Size of a Pattern Piece via API
-   Added **Get/SetPatternParticleDistance** call in PatternAPI to Get the Current Particle Distance of a Pattern Piece via API
-   Added **Get/SetPatternMeshType** call in PatternAPI to change the Pattern Mesh Type of a Pattern Piece via API
-   Added **GetPatternMeshCount** call in PatternAPI to Get the Count of a Mesh within a Pattern Piece via API
-   Added **GetPatternShrinkagePercent** call in PatternAPI to Get the Value of Shrinkage Percent of a Pattern Piece via API  
-   Added **Get/SetArrangement**  call in PatternAPI to Get the information of the pattern Piece by Index via API
-   Added **SetFabricName** call in FabricAPI to change the name of the Zfab via API
-   Added Export Turntable Images based on Colorway Index in ExportAPI to export turntable images based on the colorway index
-   Added **ExportPose** call in ExportAPI to export .pos of current avatar via API
-   Added **ColorwayUpdate** call in UtilityAPI to update the colorway window via API 

v3.1.4, September 2021
----------------------

-   Added Export Option Dialog Window Popup at ExportglTF in ExportAPI
-   Added **ExportPOM** call in ExportAPI
-   Added **SetShowHideAvatar** call in UtilityAPI to Toggle On&Off Avatar via API 
-   Added **SetSchematicRender** call in UtilityAPI to Toggle On&Off Schematic Render via API
-   Added **ImportVMP** call in ImportAPI to Import Render Image / Video Properties via API
-   Added **ImportVLP** call in ImportAPI to Import Render Light Properties via API
-   Added **ImportCPT** call in ImportAPI to Import Camera Properties via API 
-   Added **ImportVRP** call in ImportAPI to Import Render Properties via API 
-   Fixed Reverse Compatibility Failure Issue
-   Added Fragment Mesh Option Included in the Dialog of exportglTF 
  
