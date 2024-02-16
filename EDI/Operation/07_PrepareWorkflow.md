# Prepare workflow

Extend your workflows by adding actions for exporting the EDIFACT messages.


To integrate the export to the workflow, you must insert an
Execute PHP code core action, for detailed information see [Execute PHP code](../../ActindoWorkFlow/UserInterface/08_CoreActions.md#execute-php-code).


#### Prerequisites

- The export definition is activated, see [Activate definition](01_ManageDefinitions.md#activate-definition).
- Your workflow handles with the business document (for example, INVOIC) for which you have created the EDIFACT export definition. 

#### Procedure

*Workflow > Select workflow > Select version*




## PHP

```
$exportController = new \Actindo\Modules\Actindo\DataHubExporter\ExportController();
$exportRequest = new \Actindo\Modules\Actindo\DataHubExporter\Request\ExportRequest(4);
$exportRequest->definitionId = ; 
$exportRequest->entityId = $in0->getId();
$exportRequest->connectionIds = []; 
$exportRequest->entityClass = \Actindo\Core\Database\ClassUtils::getRealClass(get_class($in0));  
$exportController->export($exportRequest);
```

|php code | Meaning |
|--------|----|
|$exportController = new \Actindo\Modules\Actindo\DataHubExporter\ExportController();| Get exporter|
| $exportRequest = new |Create export request|
|$exportRequest->definitionId = []; | ID of the export definition|
|$exportRequest->entityId = $in0->getId(); | Primary identifier of the entity that is to be exported (e.g. business document that have been loaded at the start point and is input in *in0* input port).|
|$exportRequest->connectionIds = [];| List of connection IDs (comma-separated)|
|$exportRequest->entityClass = \Actindo\Core\Database\ClassUtils::getRealClass(get_class($in0));| Entity type (class name) input in *in0* input port

