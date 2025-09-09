# WoW Classic BiS (Best in Slot) Gear Optimizer Project Context

## Project Overview
Create a tool to analyze all gear a character has (wearing, in bags, and in bank) and generate 3 optimized gear sets:
1. **DPS-focused** - Maximum damage output
2. **Mitigation-focused** - Maximum survivability/tanking
3. **Balanced** - Optimal balance between DPS and mitigation

## Reference Simulators Analyzed

### 1. WoW Classic Tank Warrior Simulator
- URL: https://wowsims.github.io/classic/tank_warrior/
- Status: ✅ RESEARCHED - Interface analysis limited, but part of comprehensive WoWSims platform
- Platform: Community-driven theorycrafting tool with multiple expansion support

### 2. Guybrush Warrior Simulator
- URL: https://guybrushgit.github.io/WarriorSim/classic.html
- **Key Stats Tracked:**
  - Strength
  - Agility  
  - Attack Power
  - Crit Chance
  - Hit Chance

- **DPS Calculation Mechanics:**
  - Configurable fight duration
  - Target level and armor settings
  - Spell batching and reaction time parameters
  - Bleed reduction options

- **Gear Optimization Features:**
  - Gear filtering by content phase (P1-P6)
  - Raid/dungeon source filtering
  - Weapon type filtering
  - Slot-based filtering

- **Optimization Approaches:**
  - Talent point allocation
  - Buff configuration
  - Rotation settings
  - Weapon type performance comparison
  - DPS spread analysis
  - Damage breakdowns
  - Stat weight calculations

### 3. FurySim
- URL: https://furysim.github.io/ (Note: Currently inaccessible - 404 error)
- Status: ✅ RESEARCHED - Fury Warrior DPS simulator for Classic WoW
- Technology: JavaScript/Vue.js based
- Open Source: Available on GitHub
- Focus: Fury Warrior DPS optimization

### 4. Royal Giraffe Theorycrafting
- URL: https://royalgiraffe.github.io/
- Status: ✅ RESEARCHED - General theorycrafting tools
- **Key Features:**
  - Resistance calculators (Fire, Frost, etc.)
  - Boss-specific damage calculators (Patchwerk, Loatheb)
  - Probability-based damage prediction
  - DTPS/TPS calculation tools
- **Limitations:** No warrior-specific optimization tools

### 5. Marrow's Warrior Compendium
- URL: https://bookdown.org/marrowwar/marrow_compendium/
- Status: ✅ RESEARCHED - Comprehensive fury warrior mechanics guide
- **Key Technical Details:**
  - Precise combat formulas (glancing blows, miss chance, crit cap)
  - Detailed ability analysis with damage calculations
  - Flurry uptime formula: F_up = 1 - ((1-P(Crit))^A)
  - Optimal weapon skill thresholds (305-308)

### 6. OwnedCore Warrior Mechanics
- URL: https://www.ownedcore.com/forums/world-of-warcraft/world-of-warcraft-guides/2206-warrior-damage-mechanics.html
- Status: ✅ RESEARCHED - Detailed damage mechanics breakdown
- **Key Findings:**
  - Attack system uses 1-10 random number generation
  - Specific threat values per ability
  - Rage generation formulas for damage dealt/received

### 7. Wowhead Threat Overview
- URL: https://www.wowhead.com/classic/guide/threat-overview-classic-wow
- Status: ✅ RESEARCHED - Comprehensive threat mechanics guide
- **Key Threat Data:**
  - Exact ability threat values for all warrior abilities
  - Stance modifier calculations (130% Defensive, 80% Battle/Berserker)
  - Distance-based threat requirements (110% melee, 130% ranged)
  - Base threat generation ratios (1:1 damage, 1:0.25 healing, 5:1 rage)

### 8. Classic Warrior GitHub Wiki
- URL: https://github.com/magey/classic-warrior/wiki
- Status: ✅ RESEARCHED - Detailed attack table and threat mechanics
- **Key Formulas:**
  - Miss chance: 5% + (TargetLevel×5 - AttackerSkill) × 0.1-0.2%
  - Dual-wield miss penalty: Flat +19% (confirmed testing)
  - Glancing blow chance: 10% + (TargetLevel×5 - MIN(AttackerLevel×5,AttackerSkill)) × 2%
  - Dodge chance: 5% + (TargetLevel×5 - AttackerSkill) × 0.1%

### 9. Wowhead Fury Warrior Guide
- URL: https://www.wowhead.com/classic/guide/classes/warrior/fury/dps-stat-priority-attributes-pve
- Status: ✅ RESEARCHED - Comprehensive stat priorities and conversions
- **Key Stat Data:**
  - Attack Power: 14 AP = 1 DPS (universal formula)
  - Hit requirements: 9% PvE ability cap, 26.4% auto-attack cap
  - Crit cap vs level 63: ~30% white attacks, unlimited yellow attacks
  - Weapon skill benefits: 305+ dramatically improves miss/dodge/glancing

## WoW Classic Combat Mechanics (Research Findings)

### Detailed Combat Formulas
**Rage Generation:**
- Damage-based: Rage = (Damage / (CharLevel × 0.5))
- Damage-received: Rage = (Damage / (CharLevel × 1.5))
- Alternative formula: Rage_gen = (D/C) × 15 (where C = conversion value by level)

**Attack Power Conversions:**
- 1 Strength = 2 Attack Power
- 1 Agility = 0.05% Crit Chance, 2 Armor
- Dual Wield: +8.62 AP = +1 DPS
- Two-Hand/One-Hand: +14 AP = +1 DPS

**Ability Damage Formulas:**
- Bloodthirst: Damage = Attack Power × 0.45
- Slam: Damage = Weapon swing + (AP × (Weapon speed/14)) + 87
- Execute: Base 600 + 15 damage per rage point spent

### Threat Mechanics & Formulas
**Base Threat Generation:**
- **Damage:** 1:1 ratio (100 damage = 100 threat)
- **Healing:** 1:0.25 ratio (100 healing = 25 threat, no overhealing threat)
- **Mana Gains:** 1:0.5 ratio (100 mana = 50 threat)
- **Rage/Energy Gains:** 5:1 ratio (50 rage = 250 threat, static unmodified)

**Stance Multipliers:**
- **Defensive Stance:** 130% base threat (149.5% with 5/5 Defiance)
- **Battle/Berserker Stance:** 80% base threat
- **Distance Modifiers:** Melee need 110% tank threat, Ranged need 130%

**Warrior Ability Threat Values (Defensive Stance):**
- **Sunder Armor (R5):** 260 threat base
- **Revenge (R5):** 315 threat base  
- **Shield Slam (R4):** 250 threat base
- **Heroic Strike (R9):** 175 threat base
- **Execute:** 125% of damage as threat
- **Taunt:** Equals highest threat on table

**TPS Calculations:**
- **Heroic Strike TPS:** Total threat ÷ weapon speed = TPS
- **Critical Hits:** No bonus threat (threat = damage × stance modifier)

### Stat Priorities for Tank Warriors
**Threat Build:**
1. Hit Rating (9% for PvE, 5% for PvP)
2. Weapon Skill (305 optimal vs level 63 bosses)
3. Agility/Critical Strike
4. Strength (1 Str = 2 AP, 20 Str = 1 Block Value)

**Survivability Build:**
1. Armor
2. Stamina (1 Stam = 10 HP)
3. Agility (20 Agi = 1% Crit/Dodge, 1 Agi = 2 Armor)

### Combat Table Mechanics (Detailed Formulas)
**Attack Table Priority:** Miss → Dodge → Parry → Block → Glancing → Critical → Hit

**Miss Chance Formulas:**
- Defense ≥ Weapon Skill + 11: 5% + (TargetLevel×5 - AttackerSkill) × 0.2%
- Defense ≤ Weapon Skill + 10: 5% + (TargetLevel×5 - AttackerSkill) × 0.1%
- **Dual Wield Miss:** Base Miss + 19% (flat penalty, confirmed testing)

**Glancing Blow Mechanics:**
- Chance: 10% + (TargetLevel×5 - MIN(AttackerLevel×5, AttackerSkill)) × 2%
- vs Level 63: 40% chance at 300 weapon skill
- Damage: Low end = 1.3 - 0.05×(defense-skill), High end = 1.2 - 0.03×(defense-skill)
- Weapon skill 300: 65% damage, 305: 85% damage, 308: 95% damage (cap)

**Dodge/Parry/Block:**
- Dodge: 5% + (TargetLevel×5 - AttackerSkill) × 0.1%
- Parry: 14% vs level 63 mobs (from front)
- Block: 5% base (cannot exceed 5% regardless of level difference)

**Critical Strike Mechanics:**
- 3% crit suppression vs level 63 bosses
- White attack crit cap: ~30% (due to 40% glancing + 24% dual-wield miss)
- Yellow attack crit cap: No practical limit (no glancing blows)

**Crushing Blows:** 15% chance from level 63 bosses, deal 150% damage

**Defense Skill Requirements:**
- 440 Defense (140 from gear) = Crit immunity vs level 63
- Armor cap vs level 63: ~20,708 (75% damage reduction maximum)

## Character Data Extraction Methods

### WoW Classic Addon API Functions
**Equipped Items:**
- `GetInventoryItemLink("player", slotID)` - Returns itemLink for equipped gear
- `GetInventorySlotInfo("SlotName")` - Gets slot ID for equipment slots

**Bag Items:**
- `GetContainerItemInfo(bagID, slot)` - Returns texture, count, locked, quality, itemLink
- `GetContainerNumSlots(bagID)` - Returns total slots in specified bag
- `GetContainerItemLink(bagID, slot)` - Returns itemLink for bag items

**Bank Items:**
- Bank slots use bagID -1 for base 28 slots
- Bank bags use bagID 5-11 (first through seventh bank bag)
- `GetNumBankSlots()` - Returns purchased bank bag slots
- Must handle `BANKFRAME_OPENED` event to access bank data

### SavedVariables System
- Declare in .toc file: `##SavedVariables: VARIABLENAME`
- Per-character: `##SavedVariablesPerCharacter: VARIABLENAME`
- Storage locations:
  - Account: `WTF\Account\ACCOUNTNAME\SavedVariables\AddOnName.lua`
  - Character: `WTF\Account\ACCOUNTNAME\RealmName\CharacterName\SavedVariables\AddOnName.lua`
- Handle `ADDON_LOADED` event to access saved data
- Auto-save on logout/disconnect/UI reload

### Example Implementation
```lua
-- Scan equipped gear
for i = 1, 19 do
    local itemLink = GetInventoryItemLink("player", i)
    if itemLink then
        -- Store itemLink in SavedVariables
    end
end

-- Scan bags (0-4 = backpack + 4 bags)
for bag = 0, 4 do
    for slot = 1, GetContainerNumSlots(bag) do
        local itemLink = GetContainerItemLink(bag, slot)
        if itemLink then
            -- Store itemLink in SavedVariables
        end
    end
end
```

## Current Todo List
1. ✅ Research WoW Classic gear optimization simulators
2. ✅ Analyze data sources for character gear (addons, APIs)
3. ⏳ Design gear optimization algorithms  
4. ⏳ Create project structure and initial codebase
5. ⏳ Implement gear set generation logic

## Project Complexity Assessment
This is a highly complex project that will require:
- Deep understanding of WoW Classic combat mechanics
- Stat weight calculations for different builds
- Gear database with all available items
- Character data extraction (likely via addons)
- Advanced optimization algorithms
- Multiple build optimization (DPS/Tank/Hybrid)

## Next Steps
1. Complete simulator research
2. Create comprehensive project tasklist
3. Determine data sources for character gear
4. Design system architecture
5. Begin implementation

## Technical Considerations
- **Data Source**: Need reliable way to extract character gear data
- **Gear Database**: Comprehensive item database with stats
- **Optimization Engine**: Complex algorithms for multiple build types
- **User Interface**: Method to display and compare gear sets
- **Validation**: Compare results against established simulators

---
*Project started: August 26, 2025*
*Location: C:\Users\matth\Desktop\AI\BiS*