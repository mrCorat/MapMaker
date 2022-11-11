# MapMaker
Generate Map for game
Our idea will get on generate multipoligons with some roles. Maybe in little segmentations it can be looks like simple polygon clusters, but we know that it too simple variant. We can make more accurate variant with special class Border. But we should say, that first points is dividing points between localization clusters. In some abstraction map will be like planar graph with edges - 3-ple and more dimention intersection between local objects.
There forming algoritm structure:
```mermaid
stateDiagram-v2;   
    [*] --> Lanscapeform;
    Landscapeform --> RiverMake;
    RiverMake --> ForrestMake;
    ForrestMake -- > MakeHumanInfrastructure;
    MakeHumanInfrastructure --> ConnectionInfrastructure;
    ConnectionInfrastructure --> [*];
```
