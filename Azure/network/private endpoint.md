- to 'Deny public access', private endpoint is required before turn on 'Deny public access'


- create private end point
1. Home > Create a resouce > Private Endpoint
    1. Basics
        - Resource Group: ***_VNets
        - Name: endp-test
        - Region: (Canada)...
    1. Resouces
        - Subscription: Ms Azure Enterpise
        - Resouce type: Microsoft.Sql/Servers
        - Resource: server-...
    1. Configureation
        - Virtal network: ..._Vnet
        - Subnet: ..._Subnet(###.###.###.###/25)
        - private DNS integration
            -Private DNS zone: privatelink.database.windows.net
    1. ...
1. allow VPN route to the ip of endpoint