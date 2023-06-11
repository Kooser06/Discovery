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
- [PV Extensisons](https://www.chessprogramming.org/PV_Extensions)
The idea behind PV extensions is to extend nodes along the PV line to achieve higher search depths in the critical part of the tree. To prevent a search explosion we do not allow two consecutive extensions back to back along the PV line.
- [Capture Extensions](https://www.chessprogramming.org/Capture_Extensions)
- [Check Extensions](https://www.chessprogramming.org/Check_Extensions)
- [Mate Threat Extensions](https://www.chessprogramming.org/Mate_Threat_Extensions)
- [One Reply Extensions](https://www.chessprogramming.org/One_Reply_Extensions)
- [Passed Pawn Extensions](https://www.chessprogramming.org/Passed_Pawn_Extensions)
## Evaluation
