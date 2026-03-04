# Setup

## Part 1

- User sets the number of players
- Randomly select the same number of territories
- Randomly select a capital territory from among territories in play
- Randomly select a brenn
- Brenn clicks to flip the flock of crows

### Pseudocode generated

num_players = 2
players.1.name, players.2.name = 'Blake', 'Daniel'
active_territories = {cove, forest}
capital = 'cove'
territory.cove.citadels = 1
players.1.brenn = True
turn_direction = 'clockwise'

## Part 2

- Brenn places first man
- Snake Draft

### Pseudocode generated

territories.cove.player_1_clans = 2
territories.cove.player_2_clans = 1
territories.cove.chieftain = 'Blake'
territories.forest.player_2_clans = 1
territories.forest.chieftain = 'Daniel'
players.1.victory_conditions =  [2, 0, 0, 0]
players.2.victory_conditions = [1, 1, 0, 0]



# Assembly Phase

## Victory Conditions

- Check for pretender tokens
- If pretender, check for victory conditions

### Pseudocode generated

players.1.pretender, players.2.pretender = false, false

## Card distribution

- If nobody wins, distribute 4 cards
- Players pass 3, 2, 1 card

### Pseudocode generated

players.1.cards, players.2.cards = {geis, bard, ...}, {craftsmen and peasants, ...}



# Season Phase

## Standard gameplay

- Brenn plays a card or passes
- Next player plays a card or passes
...
- If both players pass, season ends

### Pseudocode generated



## War

 - One player uses a card that initiates a war
 - In turn order, players take turns entering citadels
 - If all citadels are full or no player wants to be in the citadel, proceed
 - Both players choose peace or one player chooses to attack
 - If one chooses to attack, the non-initiator chooses to drop man or card
 - Repeat steps 2-3 until both choose peace or only one side has exposed clans

 ### Pseudocode generated

