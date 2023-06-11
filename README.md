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
- [Check Extensions](https://www.chessprogramming.org/Check_Extensions): Extendind the search if we in check is a great idea to prevent the engine from missing critical moves that leads it to make mistakes. We also do not allow two consecutive searches back to back to prevent [search explosions](https://www.chessprogramming.org/Search_Explosion).
- [Mate Threat Extensions](https://www.chessprogramming.org/Mate_Threat_Extensions): After a null move we generally try to detect mate threats by conduction a zer-window search to see if there is a [mate threat](https://www.chessprogramming.org/Null_Move_Pruning#Mate_Threats).
- [One Reply Extensions](https://www.chessprogramming.org/One_Reply_Extensions): We should most definately extend the search on positions where there is only one legal move. For these types of extensions we don't allow consecutive extensions back to back to [search explosions](https://www.chessprogramming.org/Search_Explosion). This will help with the [horizon effect](https://www.chessprogramming.org/Horizon_Effect).
- [Passed Pawn Extensions](https://www.chessprogramming.org/Passed_Pawn_Extensions): Pawns that are at least 4 moves away from promotion are extended to allow the endgine so endgame/promotion tactics. We also don't allow consective extensions so if the pawn is for say 3 moves away then the search will be extended by one the the next passed pawn move will not be extended and then the 3 move will be. so for 3 moves it will be extended by 2 ply and same for 4 moves away.
## Evaluation
