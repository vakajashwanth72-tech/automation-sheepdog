## Herding Strategy

Sheep exhibit fear-based reactive behavior. When the Sheepdog approaches within a threshold distance
 sheep move directly away from it. Therefore, directly chasing sheep is ineffective.

The Sheepdog instead applies indirect control by positioning itself behind a target sheep along the line connecting the sheep and the safe zone.

### Target Selection
The Sheepdog selects the nearest sheep based on Euclidean distance.

### Herding Point Computation
Let S be the sheep position and Z be the safe zone center.

Direction = S − Z  
Herding point = S - Direction × offset
where offset is some finite ddistance

By moving to this herding point, the Sheepdog causes the sheep to move toward the safe zone.
