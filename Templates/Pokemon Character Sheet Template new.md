---
Species: "[[SRD-Rockruff]]"
Abilità: "[[SRD-Keen Eye]]"
Strength: 2
Dexterity: 0
Vitality: 0
Special: 0
Insight: 0
Tough: 0
Cool: 0
Beauty: 0
Cute: 0
Clever: 0
Brawl: 0
Channel: 0
Clash: 0
Evasion: 0
Alert: 0
Athletic: 0
Nature: 0
Stealth: 0
Allure: 0
Etiquette: 0
Intimidate: 0
Perform: 0
maxAbility: 15
Moves: "[[SRD-Tackle]]"
TrainerPoints: "0"
---

# `= this.Species.name`

**Species**: `= this.Species`
**DexID**: `= this.Species.number`
**Rank**: Rookie
**Nature**: Timida
**Gender**: Maschio
**Abilities**: `= this.Abilità`
**Current Training Points** `= this.TrainerPoints`

**Type**: `= this.Species.Type1 + this.Species.Type2`

**Max HP**: `= this.Species.Vitality + this.Vitality + this.Species.BaseHP`
**Current HP** :  5
**Will**:: `= this.Species.Insight + this.Insight + 3`
**Will used**: 0
**Held Item**:  

|Quick Reference|
|-|-|
|**Initiative**:|`= this.Species.Dexterity + this.Dexterity + this.Alert`
|**Defence**: | `= this.Vitality + this.Species.Vitality`
|**Special Defence**: | `= this.Insight + this.Species.Insight`
|**Clash Dice**:| `= max(this.Species.Strenght + this.Strenght, this.Species.Special + this.Special) + this.Clash`
|**Evasion Dice**:| `= this.Dexterity + this.Species.Dexterity + this.Evasion`

```dataviewjs
if (false){
    let select_html = "<select>"
    //let items_paths = dv.pagePaths('"Pokerole SRD/SRD v3.0/SRD-Items"')
    let items = dv.pages('"Pokerole SRD/SRD v3.0/SRD-Items"')
    for (let i = 0; i < items.length; ++i) {
        let itemData = items[i]//dv.page(items_paths[i])
        
        select_html += "<option>" + dv.fileLink(itemData.file.path, false, itemData.name) + "</option>"
    }
     select_html += "</select>"
     
    dv.el("div",select_html)
}
```




| Physical Attributes |
|:-:|:-:|:-:|
| Strength  | `= padleft("",this.Species.Strength,"⬤")+padleft("",this.Strength,"⦿")+padright("",this.Species.MaxStrength - this.Strength - this.Species.Strength,"⭘")`      | `= this.Species.Strength+this.Strength`/`= this.Species.MaxStrength`    | Tough  | `= padright(padright("⬤",this.Tough+1,"⦿"),5,"⭘")`  | `= this.Tough+1`/5  |
| Dexterity | `= padleft("",this.Species.Dexterity,"⬤")+padleft("",this.Dexterity,"⦿")+padright("",this.Species.MaxDexterity - this.Dexterity - this.Species.Dexterity,"⭘")` | `= this.Species.Dexterity+this.Dexterity`/`= this.Species.MaxDexterity` | Cool   | `=padright(padright("⬤",this.Cool+1,"⦿"),5,"⭘")`    | `= this.Cool+1`/5   |
| Vitality  | `= padleft("",this.Species.Vitality,"⬤")+padleft("",this.Vitality,"⦿")+padright("",this.Species.MaxVitality - this.Vitality - this.Species.Vitality,"⭘")`      | `= this.Species.Vitality+this.Vitality`/`= this.Species.MaxVitality`    | Beauty | `= padright(padright("⬤",this.Beauty+1,"⦿"),5,"⭘")` | `= this.Beauty+1`/5 |
| Special   | `= padleft("",this.Species.Special,"⬤")+padleft("",this.Special,"⦿")+padright("",this.Species.MaxSpecial - this.Special - this.Species.Special,"⭘")`           | `= this.Species.Special+this.Special`/`= this.Species.MaxSpecial`       | Cute   | `=padright( padright("⬤",this.Cute+1,"⦿"),5,"⭘")`   | `= this.Cute+1`/5   |
| Insight   | `= padleft("",this.Species.Insight,"⬤")+padleft("",this.Insight,"⦿")+padright("",this.Species.MaxInsight - this.Insight - this.Species.Insight,"⭘")`           | `= this.Species.Insight+this.Insight`/`= this.Species.MaxInsight`       | Clever | `= padright(padright("⬤",this.Clever+1,"⦿"),5,"⭘")` | `= this.Clever+1`/5 |

| Social Attributes |
|:-:|:-:|:-:|
| Tough    | `=padleft("",this.Tough, "⦿") + padleft("",this.maxAbility - this.Tough, "⭘")` | `=this.Tough` |
| Cool   | `=padleft("",this.Cool, "⦿") + padleft("",this.maxAbility - this.Cool, "⭘")`   |   `=this.Cool`  | 
| Beauty   | `=padleft("",this.Beauty, "⦿") + padleft("",this.maxAbility - this.Beauty, "⭘")`   |   `=this.Beauty`  | 
| Cute   | `=padleft("",this.Cute, "⦿") + padleft("",this.maxAbility - this.Cute, "⭘")`   |   `=this.Cute`  | 
| Clever   | `=padleft("",this.Clever, "⦿") + padleft("",this.maxAbility - this.Clever, "⭘")`   |   `=this.Clever`  | 

| Fight |
|:-:|:-:|:-:|
| Brawl   | `=padleft("",this.Brawl, "⦿") + padleft("",this.maxAbility - this.Brawl, "⭘")`   | `=this.Brawl`   |
| Channel | `=padleft("",this.Channel, "⦿") + padleft("",this.maxAbility - this.Channel, "⭘")` | `=this.Channel` |
| Clash   | `=padleft("",this.Clash, "⦿") + padleft("",this.maxAbility - this.Clash, "⭘")`   | `=this.Clash`   |
| Evasion | `=padleft("",this.Evasion, "⦿") + padleft("",this.maxAbility - this.Evasion, "⭘")`   | `=this.Evasion`   |

| Survival |
|:-:|:-:|:-:|
| Alert    | `=padleft("",this.Alert, "⦿") + padleft("",this.maxAbility - this.Alert, "⭘")` | `=this.Alert` |
| Athletic   | `=padleft("",this.Athletic, "⦿") + padleft("",this.maxAbility - this.Athletic, "⭘")`   |   `=this.Athletic`  | 
| Nature   | `=padleft("",this.Nature, "⦿") + padleft("",this.maxAbility - this.Nature, "⭘")`   |   `=this.Nature`  | 
| Stealth   | `=padleft("",this.Stealth, "⦿") + padleft("",this.maxAbility - this.Stealth, "⭘")`   |   `=this.Stealth`  | 

| Social |
|:-:|:-:|:-:|
| Allure    | `=padleft("",this.Allure, "⦿") + padleft("",this.maxAbility - this.Allure, "⭘")` | `=this.Allure` |
| Etiquette   | `=padleft("",this.Etiquette, "⦿") + padleft("",this.maxAbility - this.Etiquette, "⭘")`   |   `=this.Etiquette`  | 
| Intimidate   | `=padleft("",this.Intimidate, "⦿") + padleft("",this.maxAbility - this.Intimidate, "⭘")`   |   `=this.Intimidate`  | 
| Perform   | `=padleft("",this.Perform, "⦿") + padleft("",this.maxAbility - this.Perform, "⭘")`   |   `=this.Perform`  | 

## Learnset
![[Pokemon Sheet Embedded Views.base#Learnsets v3.0]]



## Selected Moves
**Moves**::
```dataviewjs
function is_species_stat(stat){
    let l = ["Strength","Dexterity","Vitality","Special","Insight"]
    for (s in l){
        if (l[s] === stat)
            return true
        }
    return false
}

if (dv.current().Moves[0] == null){
    dv.paragraph("Aggiungi le mosse al parametro Moves usando le parentesi [[]]")
} else {
    for (let i = 0; i < dv.current().Moves.length-1; i++) { 

            let MovePage = dv.page(dv.current().Moves[i]) 
            let SpeciesPage = dv.page(dv.current().Species)
            
            dv.header(3, MovePage.name)
            dv.span("- [ ] Used")
        
            let acc = "F";
        
            if (MovePage.Accuracy1 === "Will")
            {
                let selected = is_species_stat(MovePage.Accuracy1) ? SpeciesPage : dv.current()
                acc = SpeciesPage["Insight"] + dv.current()["Insight"] + 2 + selected[MovePage.Accuracy2];
            } else
            {
                let acc1_stat = 0
                if (MovePage.Accuracy1 != ""){
                    let parts = MovePage.Accuracy1.split("/")
                    if (parts.length != 0){
                        let selected_bool = is_species_stat(parts[0])
                        let selected = selected_bool ? SpeciesPage : dv.current()
                        let acc_selected1 = selected[parts[0]] +  (selected_bool ? dv.current()[parts[0]] : 0)
                        if (parts.length == 2) {
                            let selected2_bool = is_species_stat(parts[0])
                            let selected2 = selected2_bool ? SpeciesPage : dv.current()
                            let acc_selected2 = selected2[parts[1]] +  (selected2_bool ? dv.current()[parts[1]] : 0)
                            acc1_stat = (acc_selected1 > acc_selected2 ? acc_selected1 : acc_selected2)
                        } else {
                            acc1_stat = acc_selected1
                        }
                    }
                }
    
               
                let acc2_stat = 0
                if (MovePage.Accuracy2 != ""){
                    let parts = MovePage.Accuracy2.split("/")
                    if (parts.length != 0){
                        let selected_bool = is_species_stat(parts[0])
                        let selected = selected_bool ? SpeciesPage : dv.current()
                        let acc_selected1 = selected[parts[0]] +  (selected_bool ? dv.current()[parts[0]] : 0)
                        if (parts.length == 2) {
                            let selected2_bool = is_species_stat(parts[0])
                            let selected2 = selected2_bool ? SpeciesPage : dv.current()
                            let acc_selected2 = selected2[parts[1]] +  (selected2_bool ? dv.current()[parts[1]] : 0)
                            acc2_stat = (acc_selected1 > acc_selected2 ? acc_selected1 : acc_selected2)
                        } else {
                            acc2_stat = acc_selected1
                        }
                    }
                }
     
     
                
                acc = acc1_stat + acc2_stat
            }
            let dmg = 0
            if (MovePage.Category != "Support"){
    
                let dmg1_stat = 0
                if (MovePage.Damage1 != ""){
                    let parts = MovePage.Damage1.split("/")
                    
                    if (parts.length != 0){
                        let selected_bool = is_species_stat(parts[0])
                        let selected = selected_bool ? SpeciesPage : dv.current()
                        let dmg_selected1 = selected[parts[0]] +  (selected_bool ? dv.current()[parts[0]] : 0)
                        if (parts.length == 2) {
                            let selected2_bool = is_species_stat(parts[0])
                            let selected2 = selected2_bool ? SpeciesPage : dv.current()
                            let dmg_selected2 = selected2[parts[1]] +  (selected2_bool ? dv.current()[parts[1]] : 0)
                            dmg1_stat = (dmg_selected1 > dmg_selected2 ? dmg_selected1 : dmg_selected2)
                        } else {
                            dmg1_stat = dmg_selected1
                        }
                    }
                }
    
                let dmg2_stat = 0
                if (MovePage.Damage2 != ""){
                    parts = MovePage.Damage2.split("/")
                    if (parts.length != 0){
                        let selected_bool = is_species_stat(parts[0])
                        let selected = selected_bool ? SpeciesPage : dv.current()
                        let dmg_selected1 = selected[parts[0]] +  (selected_bool ? dv.current()[parts[0]] : 0)
                        if (parts.length == 2) {
                            let selected2_bool = is_species_stat(parts[0])
                            let selected2 = selected2_bool ? SpeciesPage : dv.current()
                            let dmg_selected2 = selected2[parts[1]] +  (selected2_bool ? dv.current()[parts[1]] : 0)
                            dmg2_stat = (dmg_selected1 > dmg_selected2 ? dmg_selected1 : dmg_selected2)
                        } else {
                            dmg2_stat = dmg_selected1
                        }
                    }
                }
    
                dmg = MovePage.Power + dmg1_stat + dmg2_stat + ((SpeciesPage.Type1.includes(MovePage.Type) || SpeciesPage.Type2.includes(MovePage.Type))? 1:0)
            }
            //let dmg = MovePage.Power + ((SpeciesPage[MovePage.Damage1]) ? SpeciesPage[MovePage.Damage1] + dv.current()[MovePage.Damage1] : 0) + ((SpeciesPage[MovePage.Damage2]) ? SpeciesPage[MovePage.Damage2] + dv.current()[MovePage.Damage2] : 0) + ((SpeciesPage.Type1.includes(MovePage.Type) || SpeciesPage.Type2.includes(MovePage.Type))? 1 : 0);
             
            dv.span(((MovePage.Category != "Support") ? ("**Damage: **" + MovePage.Power + ((MovePage.Damage1) ? " + "+MovePage.Damage1 : "") + ((MovePage.Damage2) ? " + "+MovePage.Damage2 : "") +((SpeciesPage.Type1.includes(MovePage.Type) || SpeciesPage.Type2.includes(MovePage.Type))? " + STAB" : "") +  " = **" + dmg + "**\n") : "") +"**Accuracy: **" + MovePage.Accuracy1 +" + "+MovePage.Accuracy2 + " = **" + acc +"**");
        
         
             dv.paragraph("| Type | Target | Category | Power |\n"+
         "| ------------- | --------------- | ---------------- | -------------- |\n"+
         "| "+MovePage.Type+" | "+MovePage.Target+" | "+MovePage.Category +" | "+MovePage.Power+" |")
         
             dv.span(MovePage.effect+"<br>")
             dv.span("*"+ MovePage.description + "*")

    }
    
}
```
