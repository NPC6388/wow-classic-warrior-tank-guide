# WoW Classic BiS Optimizer Session Context - August 28, 2025

## Project Overview
This session focused on creating a comprehensive WoW Classic warrior tanking guide based on extensive research from multiple simulators and theorycrafting sources. The guide serves as foundational research for building a BiS (Best in Slot) gear optimization tool.

## Key Accomplishments

### 1. Comprehensive Research Completed
- **9 Major Sources Researched:** WoWSims, Guybrush Simulator, FurySim, Royal Giraffe, Marrow's Compendium, OwnedCore, Wowhead Threat Guide, Classic Warrior GitHub Wiki, Evil Empire Guild guides
- **Combat Mechanics Documented:** Precise formulas for miss chance, glancing blows, threat generation, stat conversions
- **Attack Tables Analyzed:** Both player attacks vs boss and boss attacks vs player with exact percentages

### 2. HTML Tanking Guide Created
**File:** `C:\Users\matth\Desktop\AI\BiS\wow_classic_tanking_guide.html`

**Key Features:**
- Four-stage progression showing combat performance at different gear levels
- Eye-catching damage/threat improvement indicators (+15-20%, +25-30%, +35-40%)
- Dual combat tables (defensive vs offensive)
- Comprehensive stat priority guides
- Complete source references with links

### 3. Critical Mechanics Discoveries

#### Attack Table Mechanics (Level 63 Bosses)
**Baseline (300 skill, 0% hit, dual-wield, from behind):**
- 28% miss (9% base + 19% dual-wield penalty)
- 5.6% dodge  
- 0% parry (attacking from behind)
- 0% block (attacking from behind)
- 40% glancing blows (65% damage at 300 skill)
- 26.4% remaining space for crits + normal hits

#### Weapon Skill Critical Thresholds
- **305 Weapon Skill:** 
  - Removes 1% hit suppression (9% → 6% hit requirement)
  - Improves glancing damage (65% → 85%)
  - Reduces boss parry chance (prevents parry-haste)
  - Each point 301-305 worth ~10 hit rating equivalent
- **308 Weapon Skill:** Glancing damage cap at 95%

#### Shield Block Mechanics (Evil Empire Research)
- Increases block chance by 75% for 5 seconds
- Pushes both critical hits AND crushing blows off attack table
- Must maintain 100% uptime against raid bosses
- More important than any single piece of gear

#### Threat Formulas (Confirmed)
- **Base Generation:** 1:1 damage, 1:0.25 healing, 5:1 rage
- **Defensive Stance:** 130% base (149.5% with Defiance)
- **Ability Values:** Revenge (315), Sunder (260), Shield Slam (250), Heroic Strike (175)

### 4. User Experience Improvements Made
- **Combat Tables Split:** Separate defensive vs offensive perspectives
- **Practical Progression:** Showed concrete performance at each gear stage
- **Visual Emphasis:** Color-coded damage improvements with emojis
- **Asterisk Cleanup:** Removed redundant explanations after mechanics established
- **Priority Ordering:** Stats ordered by actual importance (Weapon Skill > Hit Rating)

### 5. Key Corrections and Refinements
- **Parry Mechanics:** Corrected that parry doesn't require weapon/shield equipped
- **Hit Suppression:** Added 1% suppression mechanic vs level 63 bosses
- **Dual-Wield Miss:** Confirmed as flat +19% penalty (not multiplicative)
- **Crit Cap:** 26.4% represents combined crit+hit space, not just crit cap
- **Attack Power:** Dual-wield scaling (8.62 AP = 1 DPS) needs verification

## Research Sources Documented
1. [WoWSims Classic Tank Warrior](https://wowsims.github.io/classic/tank_warrior/)
2. [Guybrush Warrior Simulator](https://guybrushgit.github.io/WarriorSim/classic.html)
3. [FurySim](https://furysim.github.io/)
4. [Royal Giraffe Theorycrafting](https://royalgiraffe.github.io/)
5. [Marrow's Compendium](https://bookdown.org/marrowwar/marrow_compendium/)
6. [OwnedCore Warrior Mechanics](https://www.ownedcore.com/forums/world-of-warcraft/world-of-warcraft-guides/2206-warrior-damage-mechanics.html)
7. [Wowhead Threat Overview](https://www.wowhead.com/classic/guide/threat-overview-classic-wow)
8. [Classic Warrior GitHub Wiki](https://github.com/magey/classic-warrior/wiki)
9. [Wowhead Fury Warrior Guide](https://www.wowhead.com/classic/guide/classes/warrior/fury/dps-stat-priority-attributes-pve)
10. [Evil Empire Block Guide (Archived)](https://web.archive.org/web/20061109034808/http://evilempireguild.org/guides/block.php)
11. [Evil Empire Crushing Blow Guide (Archived)](https://web.archive.org/web/20070105001918/http://evilempireguild.org/guides/crushblock.php)

## Next Steps for Implementation

### Todo List Status:
1. ✅ Create comprehensive WoW Classic tanking guide HTML file
2. ✅ Research additional warrior mechanics from multiple sources  
3. ✅ Research comprehensive attack table and stat mechanics
4. ✅ Update tanking guide with comprehensive research findings
5. ✅ Split combat table into boss attacks vs player attacks
6. ⏳ Design gear optimization algorithms based on research
7. ⏳ Create project structure and initial codebase
8. ⏳ Implement gear set generation logic

### Key Technical Requirements for BiS Optimizer:
- **Character Data Extraction:** WoW addon using GetInventoryItemLink, GetContainerItemInfo APIs
- **Gear Database:** Complete item database with stats for all Classic gear
- **Optimization Engine:** Algorithm incorporating all researched combat mechanics
- **Multiple Build Types:** DPS-focused, mitigation-focused, balanced builds
- **Validation:** Compare results against established simulators

## Files Created This Session
- `wow_classic_tanking_guide.html` - Comprehensive tanking guide with all research
- `project_context.md` - Updated with complete research findings
- `session_context.md` - This context document

## Outstanding Questions for Next Session
1. **Attack Power Scaling:** Verify 8.62 AP = 1 DPS for dual-wield vs 14 AP = 1 DPS for 2H
2. **Addon Development:** Create WoW Classic addon for gear data extraction  
3. **Algorithm Design:** Translate research into optimization algorithms
4. **Database Schema:** Design item database structure for gear optimization

## Session Learning Highlights
- **Weapon Skill is King:** 305 weapon skill provides threat AND survivability benefits
- **Shield Block Priority:** More important than gear pieces for tank survival
- **Attack Table Complexity:** Level differences create caps and penalties everywhere
- **Guide Clarity:** User repeatedly caught unclear explanations, leading to better documentation
- **Research Depth:** Required 11+ sources to get complete picture of combat mechanics

This comprehensive research provides the mathematical foundation needed for building an accurate BiS gear optimization tool for WoW Classic warriors.