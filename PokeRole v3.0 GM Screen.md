## Skills

| Attributes    | Fight    | Survival | Social     | Knowledge | Social Attributes |
| ------------- | -------- | -------- | ---------- | --------- | ----------------- |
| **Strength**  | Brawl    | Alert    | Charm      | Crafts    | **Tough**         |
| **Dexterity** | Throw*   | Athletic | Empathy    | Lore      | **Cool**          |
| **Vitality**  | Weapons* | Nature   | Etiquette  | Medicine  | **Clever**        |
| **Special**   | Evasion  | Stealth  | Intimidate | Science   | **Beauty**        |
| **Insight**   | Clash^   |          | Perform    |           | **Cute**          |
|               | Channel^ |          |            |           |                   |

\* - Typically a human skill

\^ - Typically a Pokemon skill
## Will Points

#### Spending Will 
- **Power Through the Pain** - Spend 1 Will to ignore one Pain Penalty for the rest of the scene.
- **Take Your Chances** - Spend 1 Will to re-roll one unsuccessful die from all Action Rolls this round. 
- **Pushing Fate** - Spend 1 Will to add one success to a single roll. Doesn't work for Damage or Chance rolls.

> [!tip] Important
> - In a single round, you may only use **Take Your Chances** or **Pushing Fate**, you can't use both in the same round!
> - Spending all your Will Points in a scene causes that character to faint at the end of the scene!

#### Recovering Will 
- Rest for a few days
- Complete an achievement 
- Win a battle
- Train with your Pokemon

## Combat Flow

1. Combat Starts! Roll Initiative for each combatant: `1d6+Dexterity+Alert`
    1. Each Pokemon combatant declares which Ability is active on their Pokemon. 
    2. Storyteller informs the combatants about Weather and Terrain effects. 
2. Round Starts! Take turns in initiative order. On each Pokemon's turn:
    1. Use a Move or another action. 
    2. Choose to Pass your turn and do nothing! If you've already taken 5 Actions this round, you must pass.
3. When every Pokemon in the Initiative Order Passes, the Round ends. 
    1. At the end of the round, Trainers who are *not* In the Fray may take an action. 
4. If the combatants want to continue battling, start another round. 

#### Using a Move

1. Attacker rolls the Move's Accuracy Dice. Use the [[#Successes Required|Multiple Action Table]] to determine how many successes you need.
    1. If you have less successes than you need, your move failed to hit. 
    2. If you have any *Pain Penalties*, you subtract them from your Accuracy Dice.
2. Defender may choose to react to the Move: 
    1. Use a **Reaction**, executing that move before the attacker's move rolls it's damage. (Evade and Clash are Maneuvers with Reaction.)
        1. The Attacker may use a **Reaction** move in response to the Defenders *if* the Reaction's number is *Higher* than the Defender's!
    2. Use a **Late Reaction**, executing that move *after* the attacker's move resolves. 
        1. The Attacker may use a **Late Reaction** move in response to the Defenders. Resolve the one with the *Lowest* number first. 
        2. The Attacker may *not* use a **Reaction** against the Defender's **Late Reaction**.
3. The Attacker determines their Damage Dice, subtracts the defender's Defense or Special Defense, and rolls the Move's Damage. 
    1. If the Move's Accuracy was 3 successes *higher* than it needed to be, you've rolled a Critical Hit! Add two more dice to the damage pool.
4. Before dealing the damage, add any final modifiers to the result rolled.
    1. Each Weakness to the Attacker's Move adds one damage to the total. *Don't* add this bonus if you rolled 0 successes on your Damage Dice
    2. Each Resistance to the Attacker's Move removes one damage from the total.
5. Deal damage, then resolve any **Late Reactions** declared earlier. 

> [!danger] Lethal Damage
> - A Character tracks Lethal Damage separately from Regular Damage. 
> - When a Character suffers Lethal Damage, it counts as both Lethal and Regular Damage. 
> - A Character that has more Lethal Damage than their Total Hit Points dies.
> - A Move with the Lethal Damage icon can do Lethal Damage. *It does not have to,* and can be used to only deal regular damage. 
> - Damage dealt to a Character who has no Hit Points left is dealt as Lethal Damage.
> - *Lethal Damage is an Optional Rule!*

#### Pain Penalties

When you first reach <= Half your Hit Point total, you suffer your first pain penalty. You suffer a second at 1 Hit Point. Each Pain Penalty subtracts one success from all of your Rolls, and can be negated for the rest of the scene by paying one Will Point.

#### Trainer Actions


| Action Done as a...  | In a Trainer Area                                                        | In the Fray         |
| -------------------- | ------------------------------------------------------------------------ | ------------------- |
| Giving Commands      | Free Action on your Pokemon's Turn                                       | Action on your Turn |
| Switching Pokemon    | Twice per Round Free at anytime, <br>then Action on your Pokemon's Turn. | Action on your Turn |
| Use an Item          | Action on your Pokemon's Turn                                            | Action on your Turn |
| Enter the Fray       | End of Round Action or at Start of Battle.                               | End of Round Action |
| Search for Cover     | -                                                                        | Action on your Turn |
| Run Away from Battle | End of Round Action                                                      | End of Round Action |


![[Cover Table.png]]

#### Healing


| Damage Type | Over Time         | Potion Units     |
| ----------- | ----------------- | ---------------- |
| Regular     | 1 Damage/8 Hours  | 1 Damage/1 Unit  |
| Lethal      | 1 Damage/16 Hours | 1 Damage/2 Units |


### Rank Summary

| Rank     | Max Targets | Skill Max | Attribute Points | Skill Points |
| -------- | ----------- | --------- | ---------------- | ------------ |
| Starter  | 1           | 1         | 0                | 5            |
| Rookie   | 2           | 2         | 2                | 10           |
| Standard | 3           | 3         | 4                | 14           |
| Advanced | 4           | 4         | 6                | 17           |
| Expert   | 5           | 5         | 8                | 19           |
| Ace      | 6           | 5         | 10               | 20           |
| Master   | 8           | 5         | 10               | 22           |
| Champion | 10          | 5         | 14               | 25           |

### Successes Required 

![[Successes Difficulty.png]]


## Status Effects

| Status          | Effect                                                                                                                                                                | Resist                                                                     | Duration                        |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- | ------------------------------- |
| 1st Degree Burn | 1 Damage end/round. Fire Types Immune.                                                                                                                                | `Dex+Athletic` as action: 4 Cumulative Successes, Cured                    | Until Fainting                  |
| 2nd Degree Burn | 2 Lethal Damage end/round. Fire Types Immune.                                                                                                                         | `Dex+Athletic` as action: 6 Cumulative Successes, Cured                    | Until Fainting/Death            |
| 3rd Degree Burn | 3 Lethal Damage end/round. Increase by 2 each round.<br>Fire Types Immune.                                                                                            | `Dex+Athletic` as action: 8 Cumulative Successes, Cured                    | Until Fainting/Death            |
| Confused        | If an action fails, suffer 1 damage. <br>Action Roll Penalty:<br>> Standard Rank and Lower: -1 Success <br>> Advanced to Ace: -2 Successes<br>> Master+: -3 Successes | `Insight` @ round start, 2+ successes ignore this effect for the round     | End of Scene or<br>Switched Out |
| Disabled        | Cannot used Disabled Move. Max one Move per Pokemon.                                                                                                                  | N/A                                                                        | 5 Minutes out of Combat         |
| Paralysis       | -2 Dex, moves 1/2 speed. Electric Types Immune.                                                                                                                       | N/A                                                                        | 12 Hours                        |
| Flinched        | Next Turn takes no Action. <br>Cannot use Reactions till end of next turn. <br>Can only be Flinched once per round.                                                   | N/A                                                                        | 1 Action                        |
| Poison          | 2 Damage end/round. Poison and Steel Types Immune.                                                                                                                    | Subject remains immobile: Damage per hour instead                          | Until Fainting or 8 Hours       |
| Frozen          | No Actions. Ice Types Immune.                                                                                                                                         | Use Moves against Ice(HP 5, Def 2), Super Effective Moves break instantly. | Until ice melts, Pokemon Faints |
| Badly Poisoned  | 2 Lethal Damage end/round. Increase by 2 each round. <br>Poison and Steel Types Immune.                                                                               | Subject remains immobile: Damage per hour instead                          | Until Fainting/Death            |
| In Love         | 1/2 Damage against Foe and foe's allies                                                                                                                               | `Loyalty or Insight` when attacking, 3+ successes deal full damage.        | 24 hours                        |
| Sleep           | No Actions                                                                                                                                                            | `Insight`/action: 5 Cumulative Successes, wakes up.                        | Few Hours                       |

## Battlefield Conditions

#### Weather

- **Sunny**
    - +1 to Fire Move Power 
    - -1 Damage from Water Moves
    - Cannot be Frozen
- **Rain**
    - +1 to Water Move Power
    - -1 Damage from Fire Moves
    - No one can gain the 2nd Degree or 3rd Degree Burn conditions.
- **Sandstorm**
    - 1 Typless Damage to Non Rock, Ground, or Steel Types at end of Round. Full Body Cover prevents this Damage.
    - +1 Special Defense to Rock types
    - Moves that Complete Heal in Sunny Weather only restore 1 HP
- **Snowy**
    - +1 to Ice Move Power
    - +1 Defense to Ice types
    - +1 Chance die to inflict Frozen
    - Frozen Pokemon's ice blocks have 7 Hit Points and 3 Defense.
- **Hail**
    - 1 Damage to Non Ice Types at end of round. Full Body Cover prevents this Damage.
    - +1 Chance die to inflict Frozen
    - Moves that Complete Heal in Sunny Weather only restore 1 HP
- **Desolate Weather**
    - +2 to Fire Move Power
    - Water Type Moves cannot be used
    - Non Fire Types with 4 or less Vitality must get 2 success on a `Vitality` roll at the start of each round or suffer 2 Fire Damage. 
    - Cannot be Frozen
    - Non Typhoon/Strong Winds Weather effects fail
- **Typhoon**
    - +2 to Water Move Power
    - Fire Type Moves cannot be Used
    - Cannot be Burned
    - Non Water Types with 4 or less Vitality must get 2 success on a `Vitality` roll at the start of each round or suffer 2 Water Damage. 
    - Non Desolate/Strong Winds Weather effects fail
- **Strong Winds**
    - +2 to Flying Type Move Damage. Flying types do not get super effective damage bonuses.
    - Electric, Ice, and Rock types moves are Neutral to Flying Types
    - Non Flying Types without the Levitate ability with 4 or less Dexterity must get 2 success on a `Dexterity` roll at the start of each round or suffer 2 Typeless Damage. 
    - Non Desolate/Strong Winds Weather effects fail

#### Environmental Conditions


| Condition              | Effect                                                                                                       |
| ---------------------- | ------------------------------------------------------------------------------------------------------------ |
| Fog                    | -1 success from Accuracy Rolls                                                                               |
| Muddy                  | All pokemon on the ground are Blocked and have -1 Dexterity.                                                 |
| Underwater             | End of Round, non water types roll Vitality to not faint.<br>2 successes required for each round underwater. |
| On Fire!               | End of round, roll 3 Chance dice to inflict 2nd Degree Burn to everyone present.                             |
| Electric Poles         | +1 Damage to Electric type moves                                                                             |
| Lovely Flowers         | -2 Damage from all Moves. Pokemon cannot Evade.                                                              |
| Sewers                 | End of round, roll 3 Chance dice to inflict Poisoned to everyone present.                                    |
| Deep in <br>the Jungle | +2 to rolls involving `Nature` and `Stealth`.                                                                |
| High Poles             | Non Flying types roll `Dexterity+Athletic`, need 2 successes or suffer two typeless damage.                  |
| Sprinklers             | All Pokemon have their type changed to Water.                                                                |
| Pkmn Semantary         | +2 to rolls involving `Intimidate`. Non Ghost types gain the ability "Run Away."                             |
| Minefield              | Pokemon entering the battlefield suffer 1 typeless damage.                                                   |
| Healing Pits           | Battlefield has one or more areas that heal 1 Hit Point when touched, then are used up.                      |
| Torn World             | All moves have their target changed at random.                                                               |
| Final Destination      | No Items. No Evasion or Clash.                                                                               |


## Catching

Catch rolls are: `Seal Potency` + `Bonus Successes`

![[Seal Potency.png|left]]
![[Catch Bonuses.png|right]]
![[Catch Difficulty.png]]
## Training Points

#### Getting Training Points


| After a Battle...                                      | TP Earned |
| ------------------------------------------------------ | --------- |
| Your Pokemon is higher Rank than the most powerful foe | 0         |
| Your Pokemon is same Rank as the most powerful foe     | 1         |
| Your Pokemon is one Rank below the most powerful foe   | 2         |
| Your Pokemon is two Ranks below the most powerful foe  | 3         |
| You won the Battle                                     | 2         |
| The lose the Battle                                    | 1         |
| You won, but this Pokemon fainted/switched out         | 1         |
| There were more opponents than you                     | 2         |


##### Training Session 
Training session take 2 hours and you can train a Pokemon once a day. 

- Decide on how your Pokemon will train and what Action Roll represents it
- Storyteller assigns a [[#Successes Required|Difficulty]] for the Pokemon's training.
- The Pokemon rolls the action roll, and can re-roll the first failure. Two failures ends the session.
- The Trainer rolls the same Action Roll, and gets bonus successes equal to the difficulty the Difficulty assigned to the Pokemon.
- The Pokemon earns Training Points equal to the the Trainer's result. 
- The Pokemon and Trainer recovers 2 Will Points. (When training multiple Pokemon, the Trainer only gets 2 points total.)

#### Spending Training Points

##### Rank Up & Retraining


| Rank     | TP to Next Rank | Retraining |
| -------- | :-------------: | :--------: |
| Starter  |        5        |     1      |
| Rookie   |       15        |     10     |
| Standard |       25        |     20     |
| Advanced |       30        |     25     |
| Expert   |       35        |     30     |
| Ace      |       40        |     35     |
| Master   |       50        |     40     |
| Champion |        -        |     45     |


##### Evolve 


| Evolution Speed | TP to Evolve |
| --------------- | ------------ |
| Fast            | 10           |
| Medium          | 30           |
| Slow            | 50           |


##### Learn Moves 


| Pokemon Stage | Current Rank Move | Prior Rank Move | Pre-Evolution Move | TM  | Overrank Move |
| ------------- | ----------------- | --------------- | ------------------ | --- | ------------- |
| First         | 2                 | 1               | -                  | 5   | 5 per Rank    |
| Second        | 4                 | 2               | 5                  | 5   | 15 per Rank   |
| Final         | 6                 | 3               | 10                 | 5   | 20 per Rank   |


## Types

![[Type Chart.png]]