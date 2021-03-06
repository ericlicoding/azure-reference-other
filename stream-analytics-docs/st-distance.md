---
title: ST_DISTANCE (Azure Stream Analytics) | Microsoft Docs
description: Returns the distance between two points in meters. If used with Polygons will return 0.
applies_to: 
  - "Azure"
services: stream-analytics
author: mamccrea
ms.author: mamccrea
manager: kfile
ms.service: stream-analytics
ms.topic: reference
ms.assetid: 80550bf3-96a8-47a2-8287-181e1992008c
caps.latest.revision: 2
ms.workload: data-services
ms.date: 02/01/2017
---

# ST_DISTANCE  (Azure Stream Analytics)
  Returns the distance between two points in meters. If used with Polygons will return 0.  
  
 ## Syntax  
  
```SQL   
ST_DISTANCE ( pointA, pointB )  
```  
  
## Argument  
 **PointA**  
  
 The point to measure distance from.  
  
 **PointB**  
  
 The point to measure distance to.  
  
## Return Type  
 Returns the distance between two points in meters.  
  
## Example  
  
```SQL  
SELECT  
     ST_DISTANCE(input.car1Position, input.car2Position)  
FROM input  
  
```  
  
### Input Example  
  
|carPosition|warehouse|  
|-----------------|---------------|  
|{“type”:”Point”, “coordinates”: [-5.0, -5.0]}|{“type”:”Point”, “coordinates”: [0.0, 0.0]}|  
  
### Output Example  
 784028.74077501823  
  
## See Also  

  
