# Tank Commander

Version 0.0.1-r0

## Introduction

**Tank Commander** is a simple table-top game where two players take turns to shoot at each other's tanks. The game is played on a hexagonal grid, and each player has a tank that can move and shoot in six directions. The simplest goal of the game is to destroy the opponent's units.

Players take turns activating a unit, performing a number of actions with it, and then ending their turn. The game is over when one tank is destroyed.

## Building your Tank

The basic tank starts with the following stats:

| Armor | Movement | Accuracy | Hull Points | Actions |
|-------|----------|----------|-------------|---------|
| 6/6/6 | 3        | 4+       | 4           | 5       |

It has a main turret gun with anti-tank (AT) rounds, with a range of 5 spaces.

Before the game begins, players can upgrade their tanks, spending up to 10 upgrade points on the following items:

- **Armor**: Increases the armor of the tank by 1 point. Costs 1 upgrade point per armor point, to a max of 3 per facing.
  - Side armor cannot exceed front armor.
  - Rear armor cannot exceed side armor.
- **Engine Upgrade**: Increases the movement range of the tank by 1. Costs 1 upgrade point.
- **Extended Barrel**: Increases the range of the main gun by 1. Costs 1 upgrade point.
- **Enhanced Optics**: Increases the accuracy of the main gun by 1. Costs 1 upgrade point.
- **High-Explosive (HE) Rounds**: Allows HE rounds to be loaded. Costs 1 upgrade point.
- **Anti-Infantry Weapons**: Allows the tank to fire at infantry units at a range of 2 spaces. Costs 1 upgrade point.
- **Smoke Launcher**: Allows the tank to deploy smoke, blocking line of sight through one space within a range of 2 spaces. Costs 1 upgrade point.
- **Lieutenant Commander**: Adds a Lieutenant Commander to the crew. Costs 1 upgrade point.
- **Air Support**: Allows the tank to call in an air strike during the battle. Costs 2 upgrade points.
- **Anti-Tank Mines**: Allows the tank to deploy anti-tank mines. Costs 1 upgrade point per space, up to 3 maximum.

For example, a tank could spend its upgrade points on the following upgrades:
- Armor: Front 8, Side 8, Rear 6 (4 points)
- Engine, Barrel, Optics: 3 points total
- Lieutenant Commander: 1 point
- Air Support: 2 points

The tank has a crew of 4 members:
- The **Commander** commands the tank
- The **Gunner** fires the turret gun and any other weapons
- The **Loader** loads the main gun
- The **Driver** moves the tank
- (Optional): The **Lieutenant Commander** can take over any role if the crew member is killed.

## Playing the Game

Players roll a die to determine who goes first. The player who rolls the highest number goes first.

On their turn, the player can perform actions by spending action points:

- **Move**: Move the tank forward one space.
- **Turn**: Rotate to the left or right 60 degrees. This can also rotate the turret, or not.
- **Rotate Turret**: Rotate the turret to the left or right 60 degrees.
- **Fire**: Fire the main gun at a target within range.
- **Load**: Load a round into the main gun. This is required before firing. (The gun starts the battle loaded.)
- **Fire Anti-Infantry Weapon**: Fire the anti-infantry weapon at a target within range.
- **Deploy Smoke**: Deploy smoke, blocking line of sight through a space until the end of the battle.
- **Extinguish Fire**: Extinguish a fire on the tank.
- **Call an Air Strike**: Call in an air strike. This can only be done once per battle.

### Firing the Main Turret Gun

Roll a die to determine if the shot hits. The player must roll equal to or higher than their accuracy score. If the shot hits, roll a die and add the round's strength. If the result is more than the target's armor on the the side it was hit, the target takes a penetrating hit. Otherwise, it's a glancing hit.

AT rounds have a strength of 6, HE rounds have a strength of 4.

### Inflicting Damage

A glancing hit wounds a crew member on a 4+. When a crew member is wounded, randomly select a living crew member to be wounded. If a wounded crew member is wounded again, they are killed.

A penetrating hit wounds a random crew member, and reduces the target's hull points by 1. If the target's hull points are reduced to 0, the tank is disabled -- it cannot perform any actions, and remains on the table.

A hit from an HE round can start a **Fire**. Roll a die. On a 5+, the tank is on fire. The tank's crew can use an action to extinguish the fire. If the fire is not extinguished, the tank loses 1 hull point at the end of each turn until the fire is extinguised.

At the end of every turn a disabled tank is on the table (including the turn it was disabled), roll a die. On a 4+, the ammunition cooks off. The tank is destroyed, and any units within 2 spaces of the tank are hit with an HE round with a strength of 4. The vehicle is replaced with a rubble terrain piece. If the tank's last hull point was lost to **Fire**, the ammunition cooks off immediately.

### Wounded Crew

If the Commander is wounded, the tank can perform 1 fewer action each turn. If the commander is killed, it can perform 2 fewer actions.

If the Gunner is wounded, the tank's accuracy is reduced by 1. If the gunner is killed, the tank cannot fire its weapons.

If the Loader is wounded, loading takes 2 action points. If the loader is killed, the tank cannot load its weapons (it can fire any remaining rounds that are already loaded, and any Anti-Infantry Weapons).

If the Driver is wounded, the tank's movement is reduced by 1. If the driver is killed, the tank cannot move.

If a Lieutenant Commander is replacing a killed crew member, they always performs the job of the crew member it is replacing as if that crew member was wounded, until the Lieutenant Commander is killed.

### Air Strike

Mark a space anywhere on the board. In the next turn, the player must roll a 6+ for the air strike to hit. On the following turn, it's a 5+, and then 4+, and so on. An air strike is never called on a roll of a 1.

When an air strike is carried out, the marked space is hit with an AT round with a strength of 6. Roll a die to determine the direction of the blast (1 is north, 2 is northeast, and so on). Then roll a die to determine the distance of the blast (1 is 1 space, 2 is 2 spaces, and so on). Each of those spaces are also hit with an AT round with a strength of 6.

### Terrain

- **Open Terrain**: No effect on movement or line of sight. This can be a road, or grass. Most of the board is open terrain.
- **Mud**: You must spend 2 action points to move out of a mud space. This can be a swamp, or a field.
- **Rubble**: You must spend 2 action points to move out of a rubble space. This can be a destroyed building, or the remains of an exploded tank.
- **Hill**: When a tank is immediately behind a hill space, enemy accuracy is -1. When a tank is on a hill space, all hits against it are taken against the rear armor value.
- **Forest**: When a tank is in or behind a forest space, enemy accuracy is -1.
- **Building**: Buildings are impassable terrain. Tanks can fire rounds at buildings to turn them into rubble.
- **Mines**: Tanks moving over mined spaces take an AT hit with a strength of 6. The mine is then removed from the board.

### Other Units

#### Infantry

Some battles may include infantry units. Infantry units can move 2 spaces, and can fire at tanks within 2 spaces. Infantry units have an armor value of 2, and a hull point value of 1. Infantry units can be destroyed by a hit from any main gun, or by an Anti-Infantry Weapon. Infantry can't be targeted if they are in an adjacent space to a friendly tank.

| Armor | Movement | Accuracy | Hull Points | Actions |
|-------|----------|----------|-------------|---------|
| 3/3/3 | 2        | 4+       | 1           | 3       |

Infantry units are equipped with Anti-Infantry Weapons with a range of 2 spaces, and a missile launcher with AT and HE rounds and a range of 3 spaces.

Infantry can take the following actions when activated:

- **Move**: Move the infantry unit one space in any direction.
- **Fire Missile Launcher**: Fire the missile launcher at a target within range, using either AT or HE rounds. (Rounds do not need to be loaded first)
- **Fire Anti-Infantry Weapon**: Fire the anti-infantry weapon at an infantry target within range.
- **Take Cover**: Enemies shooting this unit have -1 accuracy until the next turn. The unit cannot move or fire while in cover.
- **Capture Objective**: Capture an objective. The unit must share the space with the objective to capture it. They don't need to remain on the space to hold it.
- **Disarm Mines**: Remove an adjacent mine space from the board.
- **Mount Up / Dismount**: Infantry units can mount or dismount from a tank. They can only mount or dismount once per turn.
  - Infantry can ride on the outside of tanks. If the tank takes any hits while infantry are mounted on the outside, they are destroyed.
  - Infantry can ride inside Armored Personnel Carriers (APCs). See below.

### Armored Personnel Carriers (APCs)

| Armor | Movement | Accuracy | Hull Points | Actions |
|-------|----------|----------|-------------|---------|
| 4/4/4 | 3        | 4+       | 2           | 3       |

APCs are equipped with Anti-Infantry Weapons with a range of 3 spaces.

APCs have 4 upgrade points to spend at the beginning of the battle:

- **Armor**: Increases the armor of the tank by 1 point. Costs 1 upgrade point per armor point, to a max of 1 per facing.
  - Side armor cannot exceed front armor.
  - Rear armor cannot exceed side armor.
- **Engine Upgrade**: Increases the movement range of the tank by 1. Costs 1 upgrade point.
- **Smoke Launcher**: Allows the tank to deploy smoke, blocking line of sight through one space within a range of 2 spaces. Costs 1 upgrade point.

APCs can take the following actions when activated:

- **Move**: Move the APC forward one space.
- **Turn**: Rotate to the left or right 60 degrees.
- **Fire Anti-Infantry Weapon**: Fire the anti-infantry weapon at a target within range.
- **Deploy Smoke**: Deploy smoke, blocking line of sight through a space until the end of the battle.
- **Extinguish Fire**: Extinguish a fire on the tank.
