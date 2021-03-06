# Update-CWMTicket
## SYNOPSIS
This will update a ticket.
## SYNTAX
```powershell
Update-CWMTicket [-TicketID] <Int32> [-Operation] <Object> [-Path] <String> [-Value] <Object> [<CommonParameters>]
```
## PARAMETERS
### -TicketID &lt;Int32&gt;
The ID of the ticket that you are updating.
```
Required                    true
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -Operation &lt;Object&gt;
What you are doing with the value. 

replace, add, remove
```
Required                    true
Position                    2
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Path &lt;String&gt;
The value that you want to perform the operation on.
```
Required                    true
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Value &lt;Object&gt;
The value of path.
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
PS C:\>$UpdateParam = @{

ID = 1
    Operation = 'replace'
    Path = 'name'
    Value = $NewName
}
Update-CWMTicket @UpdateParam
```

## NOTES
Author: Chris Taylor

Date: 10/22/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=Service&e=Tickets&o=UPDATE
