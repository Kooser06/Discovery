# Discovery
## Search Algorithm
### Backward Pruning
- [Mate Distance Pruning](https://www.chessprogramming.org/Mate_Distance_Pruning)
### Returning Alpha
### Returning Beta
- [Null Move Pruning](https://www.chessprogramming.org/Null_Move_Pruning)
- [Multi-Cut](https://www.chessprogramming.org/Multi-Cut)
### Skipping Moves
### Extensions
- [PV Extensisons](https://www.chessprogramming.org/PV_Extensions): The idea behind PV extensions is to extend nodes along the PV line to achieve higher search depths in the critical part of the tree. To prevent a [search explosions](https://www.chessprogramming.org/Search_Explosion) we do not allow two consecutive extensions back to back along the PV line.
- [Capture Extensions](https://www.chessprogramming.org/Capture_Extensions): We do extend the search on capture moves but we do not extend every capture. We only extend the search on moves that capture high-value target like a queen for example so moves like PxQ, NxQ, BxQ, RxQ, and QxQ. We also do it if our oppening is capturing our queen. We do not extend on other captures to [search explosions](https://www.chessprogramming.org/Search_Explosion).
- [Check Extensions](https://www.chessprogramming.org/Check_Extensions)
- [Mate Threat Extensions](https://www.chessprogramming.org/Mate_Threat_Extensions)
- [One Reply Extensions](https://www.chessprogramming.org/One_Reply_Extensions)
- [Passed Pawn Extensions](https://www.chessprogramming.org/Passed_Pawn_Extensions)
## Evaluation
