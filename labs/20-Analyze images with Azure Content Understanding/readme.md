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
