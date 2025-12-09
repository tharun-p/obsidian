
## 1. Rewards Factors

|**Component**|**Weight**|**Calculation Formula (Pythonic)**|**Spec Version**|
|---|---|---|---|
|**Base Reward**|N/A|`eff_bal * 64 // isqrt(total_stake)`|Phase0|
|**Source Vote**|14|`base_reward * 14 // 64`|Altair|
|**Target Vote**|26|`base_reward * 26 // 64`|Altair|
|**Head Vote**|14|`base_reward * 14 // 64`|Altair|
|**Sync Committee**|2|`base_reward * 2 // 64`|Altair|
|**Proposer**|8|`(sum_included_rewards * 8) // 56`|Bellatrix|
|**Initial Slashing**|N/A|`eff_bal // 4096`|Electra|
|**Max Balance**|N/A|`2048 ETH`|Electra|

## 2. Effective Balance 

HYSTERESIS_UPWARD = 1.25 * 109 # Gwei
HYSTERESIS_DOWNWARD = 0.25 * 109 # Gwei 
MAX_EFFECTIVE_BALANCE = 2048 * 109 # Gwei (Post-Pectra)

