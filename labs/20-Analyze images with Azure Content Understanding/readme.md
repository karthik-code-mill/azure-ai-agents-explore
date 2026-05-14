20-Analyze images with Azure Content Understanding
This project shows the capability to utilize the Azure content understandding service.
The setup goes as follows,
1) Create a azure foundry resource to host the entire flow & resources
2) create a azure storage account for storage of input image files while processing & service storage spot
3) go to content under studio https://contentunderstanding.ai.azure.com/
    i) Add resource & setup teh azure resources created under setting azure foundry
   ii)  create a project with the resource linked & model selection - build the analyser
   iii) publish the built analyser
 4) Then this analyzer can be used to invoke via foundry resource


Azure components used includes

from azure.ai.contentunderstanding import ContentUnderstandingClient
from azure.ai.contentunderstanding.models import AnalysisInput, AnalysisResult
from azure.core.exceptions import AzureError
from azure.identity import DefaultAzureCredential


output from the service
Choose a file (1, 2, or 3), or anything else to exit: 1
Analyzing with project6_build_analyser analyzer...
  File: images/image1.jpg

Description:
A giraffe standing in a grassy savanna landscape under a partly cloudy sky. The giraffe is facing left and is the main subject of the image. The background features dry grass and a dramatic sky with large white clouds.

Tags:
