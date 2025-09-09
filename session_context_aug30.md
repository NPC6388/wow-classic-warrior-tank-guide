# WoW Classic Warrior Tanking Guide - Session Context (Aug 30)

## Project Overview
This project involves creating and maintaining a comprehensive World of Warcraft Classic warrior tanking guide with verified source documentation. The guide is stored in `wow_classic_tanking_guide.html` and includes 49 archived sources in the `Sources/` folder.

## Key Files
- **Main Guide**: `wow_classic_tanking_guide.html` - Comprehensive HTML guide with CSS styling
- **Sources Folder**: `Sources/` - Contains 49 archived sources with authentic styling
- **Context Document**: `session_context_aug30.md` - This file for session continuity

## Current Guide Structure
The guide includes the following major sections:
1. **Combat Mechanics** - Threat system, combat table, world buffs impact, weapon mechanics
2. **Stat Priorities** - Defense cap, hit requirements, crit analysis
3. **Defensive Stats** - Armor, defense skill, avoidance mechanics
4. **World Buffs** - Impact on warrior performance (50-70% DPS increase)
5. **Rotations** - Fury DPS and Fury-Prot tank rotations
6. **Builds** - Various warrior build options
7. **Consumables** - Potions, elixirs, food buffs

## Critical Combat Mechanics & Formulas
- **Armor Reduction Formula**: DR = AC/(AC+400+85*Moblvl)
- **Defense Skill Benefits**: +0.04% to miss/dodge/parry/block per point
- **Shield Block**: +75% block chance increase (not total 75%)
- **Dual-wield Miss Penalty**: +19% miss chance for both hands
- **Heroic Strike/Cleave Queuing**: Removes dual-wield miss penalty for next attack

## Recent Major Changes in This Session
### Fury-Prot Tank Rotation Updates
1. **Pre-Pull Setup Refinements**:
   - Added "rage mob" technique - pulling nearby trash for all warriors to build rage before boss
   - Changed "Diamond Flask" to generic "DPS/Threat trinket"
   - Restructured sequence: rage mob → Bloodrage → trinket → Death Wish → queue HS → Bloodthirst

2. **Threat Priority Corrections**:
   - Added clarification that Shield Block is "only for fights requiring a shield"
   - Corrected Shield Block description to include both "crit and crush immunity" (not just crush)

3. **Source Verification**:
   - Searched for Sunder Armor miss mechanics - found no explicit sources confirming it cannot miss
   - Sources show special attacks have 9% hit requirement (6% with 305+ weapon skill)
   - Maintained accuracy by not claiming unverified mechanics

## Current Fury-Prot Tank Pre-Pull Setup
1. **Build full rage** - Pull a "rage mob" for all warriors to white-hit before boss, then use Bloodrage
2. **DPS/Threat trinket** - Pop before pull for attack power/threat boost  
3. **Death Wish** - Activate for +20% damage/threat
4. **Queue Heroic Strike** - Ready to fire immediately
5. **Bloodthirst** - First GCD as fight begins

## Threat Priority (Defensive Stance)
1. **Revenge** - Highest threat ability (471 with Defiance)
2. **Sunder Armor** - Maintain 5 stacks (389 threat each)
3. **Bloodthirst** - Cannot be avoided, solid threat
4. **Heroic Strike** - Rage dump for threat
5. **Shield Block** - Only for fights requiring a shield, maintain for crit and crush immunity

## Source Verification System
- All claims must be backed by archived sources in the `Sources/` folder
- Comprehensive search methodology using multiple patterns
- Systematic removal of unsupported information
- 49 total verified sources with authentic styling

## Key Corrections Made Previously
1. **Armor Formula**: Corrected using `blizzard_forum_armor_cap.html`
2. **Shield Block Mechanics**: Clarified as +75% increase
3. **Dual-wield Mechanics**: Removed unsupported parry values
4. **Hamstring Usage**: Removed after source verification failed
5. **Shield Slam**: Removed from fury-prot rotation (not available to fury-prot)
6. **Stance Dancing**: Removed from fury-prot (they stay in defensive)

## Outstanding Verification Items
- **Sunder Armor Miss Mechanics**: Sources show special attacks have hit requirements but no specific confirmation of Sunder immunity
- Any other combat mechanics needing source verification

## Working Methodology
1. **Source-First Approach**: All information must be backed by archived sources
2. **Accuracy Over Completeness**: Remove unsupported claims rather than include unverified information  
3. **Comprehensive Search**: Use multiple search patterns when verifying mechanics
4. **Cross-Reference**: Validate information across multiple sources when possible

## CSS Styling Classes
- `.stat-priority` - General stat information
- `.survival-build` - Tank-specific information (green styling)
- `.dps-build` - DPS-specific information (blue styling)
- `.threat-build` - Threat/fury-prot specific information

## Session Status
- **Last Action**: Searched for Sunder Armor miss mechanics but found no explicit confirmation in sources
- **Current State**: Guide is accurate and complete with all user-requested changes implemented
- **Next Session**: Continue with any new corrections or additions, maintaining source verification standards

## Important Reminders for Next Session
- Never add information without source backing
- Always search comprehensively before claiming something cannot be found
- Maintain balance between theoretical understanding and practical application
- Keep guide focused on Classic WoW mechanics only
- Use TodoWrite tool for complex multi-step tasks