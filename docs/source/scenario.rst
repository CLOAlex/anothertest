**API Scenario**
=======================

Simulation
----------

.. code-block:: python

   import import_api
   import utility_api
   import cloApiTypes
       
       print("API Test Scenario - 01_Simulation")

       ######################################################
       
       # Initialize
       cloAssetFolderPath = utility_api.GetCLOAssetFolderPath(False)
       utility_api.NewProject()

       ######################################################
       
       # Import Avatar File(avt)
       avtfilePath = cloAssetFolderPath + "\\Avatar\\Avatar\\Female_V2\\FV2_Camila.avt"
       import_api.ImportFile(avtfilePath)
       #options = cloApiTypes.ImportExportOption()
       #import_api.ImportFile(avtfilePath, options)
       
       ######################################################
       
       # Import Cloth File(zpac)
       zpacfilePath = cloAssetFolderPath + "\\Garment\\Female_T-shirt.zpac"
       import_api.ImportFile(zpacfilePath)
       #options = cloApiTypes.ImportExportOption()
       #import_api.ImportFile(zpacfilePath, options)
       
       ######################################################
       
       # Simulation
       utility_api.Simulate(100)

.. figure:: /images/woah.gif
   :align: center
   
|
|
|



Rendering
---------

.. code-block:: python

   import import_api
   import utility_api
   import cloApiTypes
   import export_api
   import fabric_api
   import pattern_api
       print("API Test Scenario - 02_Rendering")

       ######################################################
       
       # Initialize
       cloAssetFolderPath = utility_api.GetCLOAssetFolderPath(False)
       utility_api.NewProject()

       ######################################################
       
       # Import Cloth File(zpac)
       zpacfilePath = cloAssetFolderPath + "\\Garment\\Female_T-shirt.zpac"
       import_api.ImportFile(zpacfilePath)
       
       ######################################################
       
       # Import Fabric(zfab)
       #zfabFilePath = cloAssetFolderPath + "\\Materials\\Fabric\\Sherpa_Cuddie_Fleece_Poly_230gsm.zfab"
       zfabFilePath = cloAssetFolderPath + "\\Materials\\Fabric\\Cotton_Oxford.zfab" 
       addedFabricIndex = fabric_api.AddFabric(zfabFilePath)
       
       # Assign Fabric to Pattern
       patternCount = pattern_api.GetPatternCount()
       for i in range(patternCount):
         fabric_api.AssignFabricToPattern(addedFabricIndex, i)
         
       ######################################################
       
       # Rendering
       savedFilepathList = export_api.ExportRenderingImage(False)
       #print(savedFilepathList) #utility_api.GetCLOTemporaryFolderPath()


.. figure:: /images/auto.gif
   :alt: automatic
   :align: center
