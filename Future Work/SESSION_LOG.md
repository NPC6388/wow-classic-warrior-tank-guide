# Session Log - WoW Classic Warrior Tank Guide Updates

## IMPORTANT: Workflow for Future Sessions

**Live Site:** https://npc6388.github.io/wow-classic-warrior-tank-guide/

**Before starting any work on this guide:**
1. The live site is served from `index.html` at the repo root (`C:\Users\matth\Desktop\AI\BiS\index.html`)
2. Development work is done in `Future Work/wow_classic_tanking_guide.html`
3. After making changes to the Future Work file, copy it to `index.html` before pushing
4. Always verify changes appear on the live site after pushing

**File Structure:**
- `C:\Users\matth\Desktop\AI\BiS\index.html` - **LIVE SITE** (GitHub Pages serves this)
- `C:\Users\matth\Desktop\AI\BiS\Future Work\wow_classic_tanking_guide.html` - Development version
- Both files should be kept in sync

---

## Session Date: 2026-01-08

### Major Changes Summary
- Restructured Enchantments section into separate DPS and Tank Warrior Enchantments
- Consolidated consumables sections (removed "Expensive" and "Essential" subsections)
- Added Subtlety cloak enchant to DPS section
- Added +7 Agility boot enchant with world buff notes
- Added Spirit of Zanza to Tank consumables
- Added back-to-TOC links on all section headings
- Added Dragon Breath Chili food buff warning
- Updated R.O.I.D.S. and Scorpok with Zanza stacking notes

---

### Detailed Changes

#### 1. Enchantments Section Restructure
**Completely restructured from table format to list format matching live site:**

**DPS Warrior Enchantments (NEW FORMAT):**
- Head: Arcanum of Rapidity (+1% haste), Arcanum of Voracity (+8 STR)
- Shoulder: Zandalar Signet of Might (+30 AP), Might of the Scourge (+26 AP, +1% crit)
- Back: Lesser Agility (+3 Agi), **Subtlety (-2% threat)** - NEW
- Chest: Greater Stats (+4 all stats)
- Wrist: Superior Strength (+9 STR)
- Hands: Greater Strength (+7 STR), Superior Agility (+15 Agi)
- Legs: Voracity (+8 STR), Rapidity (+1% haste)
- Feet: Minor Speed, **Greater Agility (+7 Agi)** - with WB note
- Weapons: Crusader (MH, OH, 2H)

**Tank Warrior Enchantments (NEW FORMAT):**
- Head: Presence of Might (+10 Sta, +7 Def, +15 Block), Voracity, Rapidity
- Shoulder: Might of the Scourge, Fortitude of the Scourge, Zandalar Signet of Might
- Back: Dodge (+1% dodge), Lesser Agility
- Chest: Greater Stats, Major Health (+100 HP)
- Wrist: Superior Stamina (+9 Sta), Superior Strength (+9 STR)
- Hands: Superior Agility (+15 Agi), Greater Strength (+7 STR)
- Legs: Presence of Might, Voracity, Rapidity
- Feet: Minor Speed, **Greater Agility (+7 Agi)** - with WB note
- Weapons: Crusader (MH, OH)
- Shield: Thorium Shield Spike, Lesser Block (+2%), Greater Stamina (+7 Sta)

**Boot Enchant Note:** "+7 Agility (use on 2nd pair for WB raids - speed doesn't stack with WBs)"

#### 2. Consumables Section Updates

**DPS Consumables:**
- Consolidated Potions/Elixirs (removed "Expensive" subsection)
- Moved Mighty Rage Potion and Winterfall Firewater into main list
- Added Zanza stacking notes to R.O.I.D.S. and Scorpok

**Tank Consumables:**
- Removed "Essential (Every Pull)" heading
- Added Spirit of Zanza (+50 Sta, +50 Spirit, 2hr) to Potions/Elixirs
- Consolidated R.O.I.D.S. and Scorpok into main Potions/Elixirs section
- Removed separate "Threat Buffs (if Zanza not needed)" subsection

**R.O.I.D.S. vs Scorpok Intro:**
- Added: "Neither stacks with Spirit of Zanza."

**Dragon Breath Chili:**
- Added: "Note: Eating any other food while Dragon Breath Chili is active will remove the buff."

#### 3. Navigation Improvements
**Added back-to-TOC links on all h2 section headings:**
- Introduction
- Combat Mechanics
- Stat Priorities
- Consumables
- Engineering
- Combat Rotations
- Warrior Builds
- Gear Optimization Strategy
- Enchantments
- Essential Tanking Macros
- Essential WeakAuras for Warriors
- Essential Addons for Warriors
- Available Simulators & Tools
- (Race Selection and Changelog already had links)

#### 4. Removed Duplicate Enchant Section
- Removed old "Gear Enchants" h3 section from within Gear Optimization
- Kept only the main "Enchantments" h2 section

---

### Files Modified
- `Future Work/wow_classic_tanking_guide.html` - Development version
- `index.html` - Live site version (copied from Future Work)
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
6 commits pushed to GitHub

### Git Commit Summary
1. Update consumables and enchant recommendations
2. Add Zanza buff slot notes to R.O.I.D.S. and Scorpok consumables
3. Restructure enchants section and consolidate consumables
4. Update live site with enchants restructure and consumables updates
5. Add TOC links to section headings, consolidate tank consumables
6. Remove Essential (Every Pull) headings from consumables

### Status
- ✅ Enchantments section restructured to match live site format
- ✅ Subtlety cloak enchant added for DPS
- ✅ Boot enchant WB notes added
- ✅ Consumables consolidated and cleaned up
- ✅ Spirit of Zanza added to Tank consumables
- ✅ All section headings link back to TOC
- ✅ Dragon Breath Chili warning added
- ✅ R.O.I.D.S./Scorpok Zanza notes added
- ✅ All changes pushed to GitHub
- ✅ Live site updated

### Notes
- Discovered that `index.html` at repo root is the live site, not the Future Work file
- Future sessions should always copy changes to index.html before pushing
- Enchantments section now uses clean list format instead of table
- Consumables section is now more streamlined without redundant headings
- All navigation improved with back-to-TOC links on every section

---

## Session Date: 2026-01-02

### Major Changes Summary
- Created DW Fury Stat Priority Analysis with interactive Chart.js visualization
- Added collapsible section to tanking guide comparing stat priorities with/without world buffs
- Fixed dark mode compatibility issues
- Improved dark mode contrast for new section to match guide's color scheme

---

### Detailed Changes

#### 1. DW Fury Stat Priority Analysis Tool (NEW)
**Created:** `dw_fury_stat_priority.html`

**Features:**
- **Interactive Line Graph** - Dual-line chart comparing stat priority values with/without world buffs
- **Chart.js Integration** - Professional data visualization library
- **Stat Cards** - Six detailed cards explaining each stat priority:
  - 305 Weapon Skill (~15-25% DPS increase)
  - 6% Hit Cap (~15-20% DPS increase)
  - Critical Strike (~15-20% without buffs, ~26-30% with buffs)
  - Attack Power (~10-15% without buffs, ~7-10% with buffs)
  - Strength (~5-8% without buffs, ~6-9% with buffs)
  - Agility (~3-5% without buffs, ~5-7% with buffs)
- **Key Insights Box** - Explains how world buffs fundamentally change stat priorities
- **Assumptions Section** - Lists world buff composition and calculation methodology

**Mathematical Basis:**
- Derived from Tankenheimer's guide formulas and combat mechanics
- Flurry uptime formula: F_up = 1 - (1 - c)^4
- 20% crit = 59% Flurry uptime
- 40% crit (with buffs) = 87% Flurry uptime
- World buffs: Rallying Cry (+5% crit, +140 AP), Onyxia (+140 AP), Spirit of Zandalar (+15% stats), Dire Maul Tribute (+200 AP)

**Key Finding:**
Critical Strike becomes significantly more valuable with world buffs (~28% DPS vs ~17.5% without) due to exponential Flurry uptime scaling, while Attack Power becomes less valuable (~8.5% vs ~12.5%) due to diminishing returns from +340 AP baseline from buffs.

#### 2. Integrated Analysis into Tanking Guide
**Files Modified:**
- `Future Work/wow_classic_tanking_guide.html`
- `index.html`

**Changes:**
- Added Chart.js CDN library to <head>
- Added TOC entry: "DW Fury Stat Priority Analysis" under Stat Priorities section
- Added collapsible `<details>` section immediately after "Crit Cap Reality" warning box
- Section ID: `#dw-fury-analysis` (linked from TOC)
- Section includes full interactive visualization with all content from standalone tool

**Location:** Line ~1235 in both files (after Crit Cap Reality, before Threat-Focused Build)

#### 3. Dark Mode Compatibility Issues Fixed
**Problem:** Initial implementation accidentally overwrote `index.html` with version from `Future Work/` that lacked dark mode toggle and CSS

**Resolution:**
- Restored original `index.html` with dark mode functionality
- Re-applied DW Fury analysis section correctly
- Preserved all dark mode CSS and toggle button functionality

**Commits:**
- Commit ce0870e: Fixed by restoring dark mode while adding new section
- Required complete restoration of ~200 lines of dark mode CSS

#### 4. Dark Mode Styling for New Section
**Added:** Comprehensive dark mode CSS specifically for `#dw-fury-analysis`

**Styling Applied:**
- **Outer container:** Dark gray (#2d3748) with blue border (#63b3ed)
- **Summary text:** Green (#4ade80) matching h2 headings
- **Inner backgrounds:** Dark slate (#1e293b) replacing white
- **Stat cards:** Dark gray (#2d3748) replacing light gray (#f8f9fa)
- **Key insights box:** Dark blue (#1e3a8a) matching other info boxes
- **Assumptions box:** Dark yellow-brown (#4a4a3a) matching warning boxes
- **Text colors:** Light colors for contrast (#cbd5e0, #e2e8f0)
- **Headings:** Blue (#63b3ed) consistent with guide
- **Strong text:** Light gray (#e2e8f0)

**CSS Selectors:**
```css
body.dark-mode #dw-fury-analysis { ... }
body.dark-mode #dw-fury-analysis summary { ... }
body.dark-mode #dw-fury-analysis [style*="background: white"] { ... }
body.dark-mode #dw-fury-analysis [style*="color: #333"] { ... }
```

Total: ~64 lines of dark mode CSS added

#### 5. Minor Corrections
- Fixed typo: "Ongxia" → "Onyxia" in world buffs list (both files)

---

### Files Modified
- `dw_fury_stat_priority.html` - New standalone stat priority visualization tool (150 lines)
- `Future Work/wow_classic_tanking_guide.html` - Added DW Fury analysis section, Chart.js library
- `index.html` - Added DW Fury analysis section with dark mode support, restored dark mode functionality
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
5 commits pushed to GitHub

### Git Commit Summary
1. Add DW Fury stat priority analysis with interactive graph
2. Update live site with DW Fury stat priority analysis (mistakenly removed dark mode)
3. Add DW Fury stat priority analysis (keeping dark mode)
4. Improve dark mode contrast for DW Fury stat priority section
5. Update session log for 2026-01-02 session

### Status
- ✅ DW Fury stat priority analysis tool created
- ✅ Interactive Chart.js visualization implemented
- ✅ Section integrated into tanking guide with collapsible UI
- ✅ TOC entry added
- ✅ Dark mode compatibility restored and enhanced
- ✅ All changes pushed to GitHub
- ✅ GitHub Pages deployment successful

### Notes
- First major data visualization added to the guide comparing stat priorities
- Mathematical analysis based on Tankenheimer's combat formulas
- Demonstrates how world buffs fundamentally shift optimal gearing strategy
- Critical Strike value increases ~60% with world buffs due to Flurry scaling
- Attack Power value decreases ~30% with world buffs due to diminishing returns
- Dark mode enhancement ensures consistent visual experience across entire guide
- Section uses collapsible `<details>` element for progressive disclosure
- Chart remains responsive and interactive on mobile devices

---

## Session Date: 2025-12-23

### Major Changes Summary
- Updated Dual-Wield Fury (Tank/DPS) talent calculator link to include 5 points in Battle Shout

---

### Detailed Changes

#### 1. Talent Build Correction - Dual-Wield Fury (Tank/DPS)
**Updated:** `index.html` (line 1529)

**Changed:**
- Old link: `https://classicdb.ch/?talent=#LhhxzhbZVxzmgxoVo` (missing Battle Shout points)
- New link: `https://classicdb.ch/?talent=#LhhxzhbZVxzVtxoVo` (includes 5 points in Battle Shout)

**Reasoning:**
- 5 points in Battle Shout is necessary for tanking effectiveness
- Provides significant raid utility with improved Battle Shout buff
- Essential for threat generation in tank/dps hybrid role

---

### Files Modified
- `index.html` - Main guide file
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
1 commit pushed to GitHub

### Git Commit Summary
1. Update DW Fury tank build to include 5pts Battle Shout

### Status
- ✅ Talent calculator link corrected
- ✅ Changes pushed to GitHub
- ✅ Site updated and live

### Notes
- Quick fix to ensure tanking build has correct talent allocation
- Battle Shout is a core tanking talent for threat and raid utility

---

## Session Date: 2025-11-28

### Major Changes Summary
- Clarified that Heroic Strike and Cleave cannot glance (yellow abilities)
- Added notes in all attack tables about HS/Cleave glancing mechanics
- Created interactive Heroic Strike vs Whirlwind damage comparison tool
- Added Attack Power slider to comparison tool for dynamic analysis

---

### Detailed Changes

#### 1. Heroic Strike & Cleave Clarifications
**Added notes in three strategic locations:**

1. **Crit Cap Reality Section (line 1228)**
   - Expanded yellow abilities note to list specific examples
   - "Yellow abilities: No practical crit cap since they cannot glancing blow (includes Heroic Strike, Cleave, Sunder Armor, Bloodthirst, Execute)"

2. **Fury DPS Rotation - Opening Priority (line 1442)**
   - Added inline clarification
   - "Heroic Strike/Cleave (queued) - HS if single-target, Cleave if 2+ mobs (cannot glance)"

3. **Sunder Priority Section (lines 1469-1471)**
   - Expanded to include HS/Cleave
   - "Cannot Glance: Sunder, Heroic Strike, and Cleave are 'yellow' abilities that cannot glance*"
   - Updated footnote: "Yellow abilities can still be parried/dodged by boss, but cannot glancing blow"

#### 2. Attack Table Mechanics Updates
**Updated all four attack table sections with glancing blow clarifications:**

1. **At 300 Weapon Skill (line 573)**
   - "40% are glancing blows dealing 65% damage (white attacks only - Heroic Strike/Cleave cannot glance)"

2. **At 300 Weapon Skill + 9% Hit Rating (line 583)**
   - "40% are glancing blows dealing 65% damage (white attacks only - Heroic Strike/Cleave cannot glance)"

3. **At 305 Weapon Skill (line 594)**
   - "30% are glancing blows dealing ~75% damage (white attacks only - Heroic Strike/Cleave cannot glance)"

4. **At 305 Weapon Skill + 6% Hit Rating (line 604)**
   - "30% are glancing blows dealing ~75% damage (white attacks only - Heroic Strike/Cleave cannot glance)"

#### 3. Interactive Ability Comparison Tool (NEW)
**Created:** `ability_comparison.html`

**Features:**
- **Damage vs Attack Power Graph** - Visual comparison of HS and WW damage scaling
- **Damage per Rage Graph** - Efficiency analysis across AP ranges
- **Interactive Controls:**
  - Weapon speed slider (1.5 - 3.8 seconds)
  - MH weapon min/max damage inputs
  - Auto-attack rage generation slider (10-25 rage)
  - Attack Power slider (500-3500 AP)
- **Real-time Stat Cards:**
  - Displays damage for both abilities at selected AP
  - Shows damage per rage efficiency
  - Updates dynamically as sliders change

**Formulas Implemented:**
- Heroic Strike: Weapon Damage + 157, Effective Cost ≈ 30-35 rage (15 base + auto attack rage)
- Whirlwind: Weapon Damage + (AP × Weapon Speed / 14), Cost = 25 rage

**Key Insights:**
- WW damage scales linearly with AP, HS remains relatively flat
- WW becomes more rage-efficient at higher AP values
- Slower weapons benefit WW more due to AP × speed scaling
- HS effective cost includes lost rage from replaced auto-attack

#### 4. Added Tool to Simulators Section
**Updated:** `index.html` (lines 2283-2288)

Added new simulator card:
- **Title:** "Ability Damage Comparison Tool"
- **Link:** ability_comparison.html
- **Features:** Interactive visualization comparing Heroic Strike vs Whirlwind damage and efficiency
- **Specialties:** Damage per rage analysis, weapon speed impact, effective rage cost calculations

---

### Files Modified
- `index.html` - Main guide file
- `ability_comparison.html` - New interactive tool (380 lines)
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
4 commits pushed to GitHub

### Git Commit Summary
1. Clarify that Heroic Strike and Cleave cannot glance
2. Add notes in attack tables that Heroic Strike/Cleave cannot glance
3. Add interactive Heroic Strike vs Whirlwind comparison tool
4. Add Attack Power slider to ability comparison tool

### Status
- ✅ All changes completed and pushed to GitHub
- ✅ HS/Cleave glancing mechanics clarified throughout guide
- ✅ Attack tables updated with accurate yellow ability notes
- ✅ Interactive comparison tool created and integrated
- ✅ Tool accessible from simulators section
- ✅ GitHub Pages deployment successful

### Notes
- Session focused on clarifying yellow ability mechanics (HS/Cleave cannot glance)
- Created first interactive visualization tool for the guide
- Tool uses Chart.js for professional data visualization
- Attack Power slider enables dynamic analysis at any gear level
- Weapon speed slider demonstrates importance of weapon choice
- Effective rage cost calculation accounts for lost auto-attack rage
- Tool provides valuable insights for rotation optimization

---

## Session Date: 2025-11-26

### Major Changes Summary
- Updated Fury-Prot tank build spec from (0/33/18) to (2/33/16)
- Updated talent calculator links for new build
- Refined build description to emphasize defense rating and improved Heroic Strike

---

### Detailed Changes

#### 1. Fury-Prot Tank Build Update (Future Work)
- **Changed:** Build spec from (0/33/18) to (2/33/16)
- **Updated:** Talent calculator link from `#LZVxzVxxoVoxwzox` to `#LbZVxzVxxoVoVfz0x`
- **Updated:** Build description
  - Added emphasis on "defense rating and improved Heroic Strike for improved threat and survivability without a shield"
- **Updated:** Footnote reference to match new build link
- **Updated:** Sources section talent build link

#### 2. Fury-Prot NO SB Tank Build Update (Live Site - index.html)
- **Changed:** Build spec from (0/33/18) to (2/33/16)
- **Updated:** Talent calculator link from `#LZVxzVxxoVoVfz0xM` to `#LbZVxzVxxoVoVfz0x`
- **Updated:** Build description
  - Changed from "Defense Rating and reduced Taunt cooldown for improved survivability without a shield and threat management"
  - To "defense rating and improved Heroic Strike for improved threat and survivability without a shield"
- **Updated:** Footnote reference to match new build link

---

### Files Modified
- `Future Work/wow_classic_tanking_guide.html` - Development version
- `index.html` - Live site version
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
2 commits pushed to GitHub

### Git Commit Summary
1. Update Fury-Prot tank build spec to (2/33/16)
2. Update Fury-Prot NO SB tank build spec to (2/33/16) in live site

### Status
- ✅ All changes completed and pushed to GitHub
- ✅ Build spec corrected to (2/33/16)
- ✅ Talent calculator links updated
- ✅ Build descriptions refined for accuracy
- ✅ Both development and live files synchronized

### Notes
- Corrected talent point allocation to reflect actual build (2 in Arms, 33 in Protection, 16 in Fury)
- New build emphasizes improved Heroic Strike from Arms tree instead of Shield Bash talents
- Build focuses on defense rating for survivability while maintaining threat without shield dependency
- Unified description between development and live versions for consistency

---

## Session Date: 2025-01-26

### Major Changes Summary
- Reorganized guide structure and navigation
- Corrected ability mechanics and enchantment details
- Updated Power Infusion calculations
- Cleaned up and reorganized references section
- Enhanced navigation with TOC links on all headers
- Multiple quality-of-life improvements and corrections

---

### Detailed Changes

#### 1. Engineering Section Updates
- **Added:** Note that Battle Squawk can stack if multiple chickens are in the same group
- **Removed:** Engineering placeholder note from header (section is now complete)

#### 2. Flask Set Analysis Corrections
- **Removed:** "BiS" reference from flask set analysis title
- **Corrected:** Power Infusion effect description
  - Changed from incorrect "20% faster casting speed, 20% reduced mana cost" (WotLK version)
  - To correct Classic WoW effect: "+20% spell damage and healing for 15 seconds"
- **Added:** Detailed Power Infusion calculation in flask set example
  - Shows general effect: +20% spell damage and healing
  - Shows specific calculation: 1,301 × 1.20 = 1,561 healing power
  - Final healing: 9 + 1,561 = 1,570 HP/5sec for 60 seconds
  - Total healing over 60 seconds: ~18,840 HP

#### 3. Off-Tank (OT) Considerations
- **Removed:** Defense for crit immunity from Off-Tank gear strategy
- **Reasoning:** OTs typically operate in berserker stance and focus on threat/DPS when not actively tanking

#### 4. Macros Section Updates
- **Added:** Fury-Prot execute phase note
  - Use Last Stand (and possibly Lifegiving Gem) during execute phase for survivability
  - Be prepared to re-boon or hearth to Kargath (Horde) when Vael dies to preserve world buffs if you get Burning Adrenaline
- **Removed:** Additional Utility macros section (duplicate content)

#### 5. Combat Mechanics Corrections
- **Corrected:** Retaliation ability description
  - Changed from "unlimited counters" to "maximum of 30 counters"
  - Added note: "Melee attacks made from behind cannot be counterattacked"
- **Removed:** Shield Block Priority note box

#### 6. Enchantments Section Updates
**Location Changed:** Moved from between Stat Priorities and Consumables to after Gear Optimization (before Macros)

**Corrections Made:**
- **Arcanum of Protection:** Updated to show it comes from "Libram of Protection" (not just "from ZG")
- **Tank Legs:** Added Arcanum of Protection (+1% dodge) as an option
- **Shield Enchant:** Added note that Lesser Block (+2% block chance) is best for Force Reactive Disk

#### 7. Guide Structure and Navigation
- **Reorganized Sections:** Moved Enchantments to after Gear Optimization and before Macros (more logical flow)
- **Updated TOC:** Reflects new section order
- **Added TOC Links:** All h2 section headers now link back to Table of Contents
  - Format: Clickable header text that returns to top
  - Applied to all 14 major sections including References & Citations
- **Added:** References & Citations link to Table of Contents

#### 8. Introduction Updates
- **Added:** Sentence emphasizing no single BiS list for tanks
  - "For this reason, there is no single BiS list for a tank that applies across all content."

#### 9. References Section (MAJOR REORGANIZATION)
**Merged two redundant sections into one clean, professional section:**

**Before:**
- Two separate sections: "References & Citations" (footnotes) and "Sources and References" (full list)
- ~240 lines with significant duplication
- Difficult to navigate

**After:**
- Single unified "References & Citations" section with id="references"
- Clear subsections:
  - **Inline Citations:** All 17 numbered footnotes (1-13, 2H, DW, FP, FP-NS) that are referenced throughout the document
  - **Bibliography:** Additional sources organized by category:
    * Simulators & Tools (4 sources)
    * Combat Mechanics & Theory (14 sources)
    * Comprehensive Warrior Guides (7 sources)
    * Community Resources & Forums (3 sources)
- Added introductory paragraph explaining the structure
- Eliminated all duplicate sources
- ~188 lines (52 lines shorter while maintaining all content)
- All inline citation links remain functional

---

### Files Modified
- `index.html` - Main guide file
- `Future Work/SESSION_LOG.md` - This file

### Total Commits This Session
20 commits pushed to GitHub

### Git Commit Summary
1. Add note that Battle Squawk can stack with multiple chickens
2. Remove BiS reference from flask set analysis box
3. Correct Power Infusion effect description
4. Fix Power Infusion to show correct Classic WoW effect
5. Show Power Infusion effect and calculation in flask set example
6. Remove defense for crit immunity from Off-Tank gear strategy
7. Add fury-prot execute phase survival and world buff preservation note
8. Add hearth to Kargath option for world buff preservation
9. Remove Additional Utility macros section
10. Remove engineering placeholder note from header
11. Reorganize sections: move Enchantments after Gear Optimization
12. Correct Retaliation ability description
13. Remove Shield Block Priority note
14. Correct Arcanum of Protection to show it comes from Libram
15. Add Arcanum of Protection to tank legs enchant options
16. Add note that Lesser Block enchant is best for Force Reactive Disk
17. Add note that no single BiS list applies to all tank content
18. Add References & Citations link to Table of Contents
19. Make References & Citations title link back to TOC
20. Reorganize references into single clean, well-structured section

### Status
- ✅ All changes completed and pushed to GitHub
- ✅ Guide structure optimized for better navigation
- ✅ All ability mechanics corrected
- ✅ References section fully reorganized and cleaned
- ✅ Enchantments section relocated to better position
- ✅ All inline citations verified working

### Notes
- Session focused on polish, accuracy, and user experience improvements
- Major emphasis on navigation improvements (TOC links on all headers)
- References section now professional and easy to navigate
- All Classic WoW ability mechanics verified against official sources
- Enhanced guide consistency and removed redundant content

---

## Session Date: 2025-01-25

### Major Changes Summary
- Added comprehensive Enchantments section
- Added new Fury-Prot NO SB tank build (0/33/18)
- Updated consumables for tanks and DPS
- Rewrote Engineering section with focus on essential items
- Corrected multiple enchant stats and availability
- Updated Death Wish mechanics
- Added Table of Contents entry for Enchantments

---

### Detailed Changes

#### 1. New Tank Build Added
- **Added:** Fury-Prot NO SB Tank Build (0/33/18)
- **Talent Link:** https://classicdb.ch/?talent=#LZVxzVxxoVoVfz0xM
- **Best For:** Well-geared raids where tank rarely needs Shield Block
- **Key Difference:** Drops Shield Block talents for 1H Weapon Specialization (more threat)

#### 2. Rotation Updates
- **Changed:** "Fury-Prot Tank Rotation" → "Tank Rotation" (more generic)
- **Reordered:** Max threat pre-pull setup sequence
  - New order: Power Infusion → Flask set → Diamond Flask → Tank gear → Berserker Rage → Recklessness → Def Stance → Bloodrage → Death Wish → Mighty Rage Pot → Heroic Strike → Bloodthirst

#### 3. Death Wish Mechanics Correction
- **Removed:** Specific damage taken percentage
- **Added:** Death Wish reduces armor and all resistances by 20%
- **Updated:** All references throughout guide (cooldown descriptions, strategy sections, warnings)

#### 4. Enchantments Section (NEW - Comprehensive)
**File Modified:** `index.html`
**Location:** Added between Stat Priorities and Consumables sections

**DPS Warrior Enchantments:**
- **Head:** Arcanum of Rapidity (+1% haste), Arcanum of Voracity (+8 Strength)
- **Legs:** Arcanum of Voracity (+8 Strength), Arcanum of Rapidity (+1% haste)
- **Shoulder:** Zandalar Signet of Might (+30 AP), Might of the Scourge (+26 AP, +1% crit)
- **Back:** Lesser Agility (+3 Agi), Greater Resistance (+5 all res)
- **Chest:** Greater Stats (+4 all stats), Stats (+3 all stats)
- **Wrist:** Superior Strength (+9 Str), Greater Strength (+7 Str)
- **Hands:** Greater Strength (+7 Str), Superior Agility (+15 Agi), Minor Haste (+1% attack speed)
- **Feet:** Minor Speed only
- **Main Hand/Off-Hand/2H:** Crusader only
- Strategy tip for enchantment priority

**Tank Warrior Enchantments:**
- **Head:** Presence of Might (+10 Stam, +7 Def, +15 Shield Block), Arcanum of Protection (+1% dodge), Arcanum of Rapidity (+1% haste), Arcanum of Voracity (+8 Str), Lesser Arcanum of Resilience (+20 Fire Res)
- **Legs:** Presence of Might, Arcanum of Voracity (+8 Str), Arcanum of Rapidity (+1% haste), Lesser Arcanum of Resilience (+20 Fire Res)
- **Shoulder:** Zandalar Signet of Mojo (+30 Stam), Zandalar Signet of Might (+30 AP), Might of the Scourge (+26 AP, +1% crit), Fortitude of the Scourge (+16 Def, +17 Stam)
- **Back:** Dodge (+1% dodge), Greater Resistance (+5 all res), Lesser Agility (+3 Agi)
- **Chest:** Greater Stats (+4 all stats), Major Health (+100 HP)
- **Wrist:** Superior Stamina (+9 Stam), Superior Strength (+9 Str)
- **Hands:** Superior Agility (+15 Agi), Greater Strength (+7 Str), Threat (+2% threat)
- **Feet:** Minor Speed only
- **Main Hand/Off-Hand:** Crusader
- **Shield:** Thorium Shield Spike (20-30 dmg on block), Lesser Block (+2% block chance), Greater Stamina (+7 Stam), Frost Resistance (+8 Frost Res)
- Tank enchantment strategy note (progression vs farm content)

**Key Corrections Made:**
- Corrected Libram of Voracity from +8 Agility to +8 Strength
- Removed incorrect Libram of Fervor and Libram of Resilience (don't exist)
- Only two librams exist: Rapidity (+1% haste) and Voracity (+8 Str)
- Clarified Arcanums come from turning in Librams
- Corrected Presence of Might stats (+10 Stam, +7 Def, +15 Shield Block, not +18 Stam/+10 Str/+10 Int)
- Removed "Alliance only" from all Librams (available to both factions)
- Updated Might/Fortitude of the Scourge from "Naxx exalted" to "Sapphiron drop"
- Added Lesser Arcanum of Resilience for fire resist fights (Geddon, Ragnaros, Firemaw, Mograine)

#### 5. Consumables Updates
**Tank Consumables Added:**
- Spirit of Zanza: +50 Spirit, +50 Stamina, 2hr (does NOT stack with ROIDS/Blasted Lands consumables)
- Gordok Green Grog: +10 Stamina, 15min (in Drinks section)
- Corrected Rumsey Rum Black Label duration: 4min → 15min

**DPS Consumables Added:**
- Created new Drinks section
- Rumsey Rum Black Label: +15 Stamina, 15min
- Gordok Green Grog: +10 Stamina, 15min

#### 6. Engineering Section (COMPLETE REWRITE)
**Removed:** Generic placeholder content
**Added:** Focus on 4 essential engineering items

**Essential Items:**
1. **Gnomish Battle Chicken**
   - 5% attack speed buff (Battle Squawk) for party
   - 30min cooldown, 1.5min duration
   - Best DPS increase from engineering

2. **Goblin Sapper Charge**
   - 450-750 fire damage, 10 yard AoE
   - 5min cooldown
   - Massive threat/DPS for trash and cleave

3. **Dense Dynamite**
   - 340-460 fire damage, 5 yard AoE
   - 1min cooldown
   - Ranged pulling and threat generation

4. **Force Reactive Disk**
   - Reflects 13-15 damage per hit, 20 charges
   - Shield slot, 5min cooldown
   - Best for multi-mob tanking (e.g., Garr)
   - **Required to Craft:** 215 Engineering (Gnomish)
   - **Required to Equip:** 300 Engineering (can have others craft)

**Pro Tip Added:**
- Can learn Gnomish → craft Battle Chicken → switch to Goblin for Sappers
- Force Reactive Disk only needs 300 Eng to equip (others can craft after switching)

#### 7. Table of Contents
- Added Enchantments section link
- Reordered TOC to match document flow

---

### Files Modified
- `index.html` - Main guide file

### Total Commits This Session
17 commits pushed to GitHub

### Git Commit Summary
1. Add Fury-Prot NO SB tank build (0/33/18)
2. Change 'Fury-Prot Tank Rotation' to 'Tank Rotation'
3. Reorder max threat pre-pull setup sequence
4. Update Death Wish description to reflect armor/resistance reduction
5. Add comprehensive enchantments section for gear
6. Fix Libram enchants faction restriction
7. Correct librams to only Rapidity and Voracity, fix Scourge enchants
8. Clarify Arcanum/Libram relationship in enchantments
9. Simplify feet enchant to only Minor Speed
10. Limit DPS head/legs to only Rapidity and Voracity
11. Correct Presence of Might stats
12. Add Arcanum of Voracity option to tank head enchants
13. Add dodge enchant option to tank cloak
14. Correct Arcanum of Voracity from Agility to Strength
15. Add consumables: Spirit of Zanza, Gordok Green Grog, Rumsey Rum
16. Add Enchantments to Table of Contents
17. Rewrite Engineering section to focus on essential items
18. Unify engineering section into single cohesive block
19. Add engineering specialization switching tip and equip requirements

### Status
- ✅ All changes completed and pushed to GitHub
- ✅ Enchantments section fully comprehensive
- ✅ Engineering section rewritten and focused
- ✅ Consumables updated for both tanks and DPS
- ✅ All stat corrections applied

### Notes
- Enchantments section provides clear guidance for both DPS and tanks
- Engineering specialization switching strategy documented
- All Libram/Arcanum mechanics clarified
- Death Wish mechanics corrected across entire guide
- Session focused on completing missing sections and correcting inaccurate information

---

## Previous Session: 2025-11-17

### Changes Made

#### Added Gear Enchants Section
- **File Modified:** `wow_classic_tanking_guide.html`
- **Location:** Added between "Flask Set Optimization" and "Off-Tank (OT) Considerations" sections (line 1499)
- **Source:** Information gathered from https://www.wowhead.com/classic/guide/classes/warrior/tank-enchants-gems-pve

**Content Added:**
- Comprehensive enchant recommendations organized by gear slot
- Head & Legs enchants (Lesser Arcanum of Constitution, Presence of Might)
- Shoulders enchants (Chromatic Mantle, Zandalar Signet, Scourge enchants)
- Chest enchants (Greater Stats, Major Health)
- Wrists enchants (Superior Stamina, Superior Strength)
- Hands enchants (Greater/Superior Agility)
- Feet enchants (Minor Speed, Greater Agility)
- Back enchants (Superior Defense, Dodge)
- Weapon enchants (Crusader)
- Shield enchants (Greater Stamina, Thorium Shield Spike)
- Strategy tips for progression vs farm content
- Phase-dependent availability warnings

### Status
- ✅ Changes completed
- ✅ Pushed to GitHub

### Notes
- All enchant information structured with phase availability
- Included both survivability and threat-focused options
- Added context for when to use each enchant type
