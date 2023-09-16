# Chunky

Permissions
You will need OP to use commands.

On a dedicated server, type op <username> from the server console. If using single player, enable cheats.


## Commands

### Task Management

`chunky start Starts a new chunk generation task from the current selection`

`chunky pause Pauses the current chunk generation tasks, and saves progress`

`chunky continue Continues running current or saved chunk generation tasks`

`chunky cancel Stops the current chunk generation tasks, and cancels progress`

### Selection

`chunky world [world] Sets the currently selected world`

`chunky shape <shape> Set the shape to generate`

`chunky center <x> <z> Sets the current center block location`

`chunky radius <radius> Sets the current radius`

`chunky worldborder Set the center and radius to match the world border in the selected world`

`chunky spawn Set the center to the spawn point`

`chunky corners <x1> <z1> <x2> <z2> Set the selection by corner coordinates`

`chunky pattern <pattern> Set the preferred generation pattern`

`chunky selection Display the current selection`


### Miscellaneous

`chunky silent Toggle displaying update messages`

`chunky quiet <interval> Set the quiet interval in seconds for update messages`

`chunky trim Delete chunks outside selection`


### Examples

Generate chunks centered on 0,0 with a 1000 block radius in the overworld

chunky radius 1000
chunky start
Generate chunks centered on 100,-100 with a 5000 block radius in the nether

chunky center 100 -100
chunky radius 5000
chunky world the_nether
chunky start
Set a world border at 0, 0 with a 10000 block radius and generate chunks inside

worldborder center 0 0
worldborder set 20000
chunky worldborder
chunky start