---
Accuracy1: SameAsBaseMove
Accuracy2: ''
AddedEffects: {}
Attributes:
  ZMove: true
Category: Support/Physical/Special
Damage1: SameAsBasePower
Damage2: ''
Description: ''
Effect: 'Single Target. Suggested effects: Roll 3 Chance Dice to Flinch, Attribute
  Increase, Damage Increase See p. 610 for more info.'
Name: Black Hole Eclipse
Power: Happiness + Loyalty
Target: Foe
Type: Dark
---

#PokeroleSRD/Moves

### `= this.name`
*`= this.Description`*

**Accuracy:** `= this.Accuracy1` + `= this.Accuracy2`
**Damage:** `= this.Power` `= choice(length(this.Damage1)=0, "","\+ "+ this.Damage1)` `= choice(length(this.Damage2)=0, "","\+ "+ this.Damage2)`

| Type          | Target          | Category          | Power          |
| ------------- | --------------- | ----------------  | -------------- |
| `= this.Type` | `= this.Target` | `= this.Category` | `= this.Power` | 

**Effect:** `= this.Effect`