# Update-CWMCatalog
## SYNOPSIS
This will update a catalog item.
## SYNTAX
```powershell
Update-CWMCatalog [-CatalogID] <Object> [-Operation] <Object> [-Path] <Object> [-Value] <Object> [<CommonParameters>]
```
## PARAMETERS
### -CatalogID &lt;Object&gt;
The ID of the catalog that you are updating. Get-CWMCatalogs
```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Operation &lt;Object&gt;
What you are doing with the value. 

replace
```
Required                    true
Position                    2
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Path &lt;Object&gt;
The value that you want to perform the operation on.
```
Required                    true
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Value &lt;Object&gt;
The value of that operation.
```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$Update = @{

CatalogID = $testProduct.id
    Operation = 'replace'
    Path      = 'price'
    Value     = $Price                            
}
Update-CWMCatalog @Update
```

## NOTES
Author: Chris Taylor

Date: 10/10/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/manage/rest?a=Procurement&e=CatalogsItem&o=UPDATE
