---
StrengthPoints: 0
DexterityPoints: 0
VitalityPoints: 0
SpecialPoints: 0
InsightPoints: 0
Tough: 0
Cool: 0
Beauty: 0
Cute: 0
Clever: 0
Brawl: 0
Throw: 0
Clash: 0
Evasion: 0
Alert: 0
Athletic: 0
nature: 0
Stealth: 0
Allure: 0
Etiquette: 0
Intimidate: 0
Perform: 0
Crafts: 0
Lore: 0
Medicine: 0
Science: 0
maxAbility: 0
Money: 0
Inventory:
---

# Name

**Age**:
**Concept**: 
**HP**: `= 4 + this.VitalityPoints`
**Current HP** :  Scrivere hp attuali
**Will**:: `= 1 + this.InsightPoints + 2`
**Will used**: 0
**Initiative**:: `= 1+this.DexterityPoints+this.Alert`
**Rank**:: 
**Nature**::
**Gender**: 
**Money**: `= this.Money`

|           |                                                                                                                                                                            |                                                                               |        |                                                     |                     |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ------ | --------------------------------------------------- | ------------------- |
| Strength  | `= padleft("",1,"⬤")+padleft("",this.StrengthPoints,"⦿")+padright("",5 - (1+this.StrengthPoints),"⭘")`      | `= 1+this.StrengthPoints`/`= 5`    | Tough  | `= padright(padright("⬤",this.Tough+1,"⦿"),5,"⭘")`  | `= this.Tough+1`/5  |
| Dexterity | `= padleft("",1,"⬤")+padleft("",this.DexterityPoints,"⦿")+padright("",5 - (1+this.DexterityPoints),"⭘")` | `= 1+this.DexterityPoints`/`= 5` | Cool   | `=padright(padright("⬤",this.Cool+1,"⦿"),5,"⭘")`    | `= this.Cool+1`/5   |
| Vitality  | `= padleft("",1,"⬤")+padleft("",this.VitalityPoints,"⦿")+padright("",5 - (1+this.VitalityPoints),"⭘")`      | `= 1+this.VitalityPoints`/`= 5`    | Beauty | `= padright(padright("⬤",this.Beauty+1,"⦿"),5,"⭘")` | `= this.Beauty+1`/5 |
| Special   | `= padleft("",0,"⬤")+padleft("",this.SpecialPoints,"⦿")+padright("",5 - (this.SpecialPoints),"⭘")`           | `= this.SpecialPoints`/`= 5`       | Cute   | `=padright( padright("⬤",this.Cute+1,"⦿"),5,"⭘")`   | `= this.Cute+1`/5   |
| Insight   | `= padleft("",1,"⬤")+padleft("",this.InsightPoints,"⦿")+padright("",5 - (1+this.InsightPoints),"⭘")`           | `= 1+this.InsightPoints`/`= 5`       | Clever | `= padright(padright("⬤",this.Clever+1,"⦿"),5,"⭘")` | `= this.Clever+1`/5 |

|Quick Reference|
|-|-|
|**Initiative**:|`= 1 + this.DexterityPoints + this.Alert`
|**Defence**: | `= 1 + this.VitalityPoints`
|**Special Defence**: | `= 1 + this.InsightPoints`
|**Evasion Dice**:| `= 1 + this.DexterityPoints + this.Evasion`

| Fight   |
| ------- | --------------------------------- | --------------- |
| Brawl   | `=padleft("",this.Brawl, "⦿") + padleft("",this.maxAbility - this.Brawl, "⭘")`   | `=this.Brawl`   |
| Throw | `=padleft("",this.Throw, "⦿") + padleft("",this.maxAbility - this.Throw, "⭘")` | `=this.Throw` |
| Clash   | `=padleft("",this.Clash, "⦿") + padleft("",this.maxAbility - this.Clash, "⭘")`   | `=this.Clash`   |
| Evasion | `=padleft("",this.Evasion, "⦿") + padleft("",this.maxAbility - this.Evasion, "⭘")`   | `=this.Evasion`   |

| Survival |                                                                   |               |
| -------- | ----------------------------------------------------------------- | ------------- |
| Alert    | `=padleft("",this.Alert, "⦿") + padleft("",this.maxAbility - this.Alert, "⭘")` | `=this.Alert` |
| Athletic   | `=padleft("",this.Athletic, "⦿") + padleft("",this.maxAbility - this.Athletic, "⭘")`   |   `=this.Athletic`  | 
| Nature   | `=padleft("",this.nature, "⦿") + padleft("",this.maxAbility - this.nature, "⭘")`   |   `=this.nature`  | 
| Stealth   | `=padleft("",this.Stealth, "⦿") + padleft("",this.maxAbility - this.Stealth, "⭘")`   |   `=this.Stealth`  | 

| Social |                                                                   |               |
| -------- | ----------------------------------------------------------------- | ------------- |
| Allure    | `=padleft("",this.Allure, "⦿") + padleft("",this.maxAbility - this.Allure, "⭘")` | `=this.Allure` |
| Etiquette   | `=padleft("",this.Etiquette, "⦿") + padleft("",this.maxAbility - this.Etiquette, "⭘")`   |   `=this.Etiquette`  | 
| Intimidate   | `=padleft("",this.Intimidate, "⦿") + padleft("",this.maxAbility - this.Intimidate, "⭘")`   |   `=this.Intimidate`  | 
| Perform   | `=padleft("",this.Perform, "⦿") + padleft("",this.maxAbility - this.Perform, "⭘")`   |   `=this.Perform`  | 

| Knowledge |                                                                   |               |
| -------- | ----------------------------------------------------------------- | ------------- |
| Crafts    | `=padleft("",this.Crafts, "⦿") + padleft("",this.maxAbility - this.Crafts, "⭘")` | `=this.Crafts` |
| Lore   | `=padleft("",this.Lore, "⦿") + padleft("",this.maxAbility - this.Lore, "⭘")`   |   `=this.Lore`  | 
| Medicine   | `=padleft("",this.Medicine, "⦿") + padleft("",this.maxAbility - this.Medicine, "⭘")`   |   `=this.Medicine`  | 
| Science   | `=padleft("",this.Science, "⦿") + padleft("",this.Science - this.Science, "⭘")`   |   `=this.Science`  | 


## Party 

- 
