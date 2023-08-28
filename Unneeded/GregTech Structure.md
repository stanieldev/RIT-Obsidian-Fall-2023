
## 3 Steps
 -  API
 -  Registry
 -  Recipes

### API
Controls the behavior of blocks, items, etc.

### Registry
Initializes the blocks, items, etc.
This is where tags will go.

### Recipes
Where recipes are generated for items and stuff.


#### Note: 
Each step may have different folder structures, but hopefully places where each overlap will still have the same naming to make it easier to find.




## Example Directory Structure

## Blocks/
> <u>Blocks.java</u> (also includes things not below)
> MachineCasing.java
> MultiblockCasing.java
> HermeticCasing.java
> HeatingCoils.java
> ...

## Cables
> <u>Cables.java</u>
> ElectricalWires.java
> FluidPipes.java

## Covers/
> <u>Covers.java</u>
> ItemFilter.java
> MachineController.java
> ActivityDetector.java
> ...

## Create/
> Gearbox.java
> KineticMixer.java
> KineticInput.java
> KineticOutput.java
> ...

## Generated
> MaterialMetal.java
>  - Ingot, Block, Plate, etc
> MaterialGem.java
>  - Gem, Block, Plate, etc
> Ores.java
>  - Ore Outputs, ore drops, and worldgen
>  - Raw Ore Outputs
> Tools.java
>  - Tool heads and tool recipes / registration
> Fluids.java

## Items/
> <u>Items.java</u> (also includes things not below)
> FluidCells.java
> Batteries.java
> VoltageItems.java
> WaferItems.java
> Circuits.java
> VoltageTools.java
> Spraycan.java

## Machines/
> Steam and Electrical Single-Block Machines
> <u>Machines.java</u>
> Macerator.java
> Compressor.java
> ...

## Multiblocks/
> Steam and Electrical Multi-Block Machines
> <u>Multiblocks.java</u>
> ElectricBlastFurnace.java
> CryoFreezer.java
> ...

## Storage/
> <u>Storage.java</u>
> Chest.java
> Tank.java
> Crate.java
> Drum.java

## VoltageBlocks/
> Transformers.java
> Converters.java
> ItemHatch.java
> FluidHatch.java
> MufflerHatch.java
> ItemPassHatch.java
> FluidPassHatch.java
> DiodeHatch.java
> RotorHolder.java
> ...