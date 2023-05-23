# RandomCodeToolbox

Creating this repo to hold random scripts or tools or workarounds that were developed by me


## Python pipe into tee work around
So apparently python will push stdout to buffer if it is not connected to shell or if you piped the output to another program/tool

Solution:
a solution is to use ```stdbuf``` in linux to extract out the buffer
- ```stdbuf -oL ./<yourscripthere> | tee <logfilehere>```