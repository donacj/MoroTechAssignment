# MoroTechAssignment
## USer Journey 1 - Station location
```mermaid
sequenceDiagram
    actor User
    participant MA as Mobile App
    participant CMS as Charging Management system
    participant DB as Database
    User->>MA: Find charging station
    MA->>CMS:Location Request
    activate CMS
    CMS->> DB: Nearby Station/Availability
    activate DB
    DB->> CMS:Response
    deactivate DB
    CMS->> MA: Response
    deactivate CMS
    MA->> User:Available Stations & Status
```
