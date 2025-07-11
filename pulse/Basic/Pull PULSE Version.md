1. Go to **XXX.Releases**/Chart/Chart.yaml
2. Check version & Upgrade to your version

name: pulse  
    version: [replace]2.3.238-alpha [to]2.3.313-alpha

1. Create PR (After Approved, Do not Complete, wait to the end) 
2. Go to [Skopeo Sync – Pulse Helm Pull](https://dev.azure.com/nc-pulse/Pulse-Demo-2/_build?definitionId=453) 
3. Run PIPELINE - Input the upgrade version: eg., 2.3.313-alpha
4. ![[Pasted image 20250711161503.png]]
5. **Complete PR**