
devel/inject-raws
=================
WARNING: THIS SCRIPT CAN PERMANENLY DAMAGE YOUR SAVE.

This script attempts to inject new raw objects into your
world. If the injected references do not match the actual
edited raws, your save will refuse to load, or load but crash.

This script can handle reaction, item and building definitions.

The savegame contains a list of the relevant definition tokens in
the right order, but all details are read from raws every time.
This allows just adding stub definitions, and simply saving and
reloading the game.

This is useful enough for modders and some users to justify the danger.

Usage example::

    devel/inject-raws trapcomp ITEM_TRAPCOMP_STEAM_PISTON workshop STEAM_ENGINE MAGMA_STEAM_ENGINE reaction STOKE_BOILER
