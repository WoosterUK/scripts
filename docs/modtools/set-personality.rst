
modtools/set-personality
========================
Changes the personality of units.
Requires a trait, modifier, and a target.

Valid traits:

:all:
    Apply the edit to all the target's traits
:trait <ID>:
    ID of the trait to edit. For example, 0 or HATE_PROPENSITY.

Valid modifiers:

:set <0-100>:
    Set trait to given strength.
:tier <1-7>:
    Set trait to within the bounds of a strength tier.

    ===== ========
    Value Strength
    ===== ========
    1     Lowest
    2     Very Low
    3     Low
    4     Neutral
    5     High
    6     Very High
    7     Highest
    ===== ========

:modify <amount>:
    Modify current base trait strength by given amount.
    Negative values need a ``\`` before the negative symbol e.g. ``\-1``
:step <amount>:
    Modify current trait tier up/down by given amount.
    Negative values need a ``\`` before the negative symbol e.g. ``\-1``
:random:
    Set the trait to a new random value.
:average:
    Sets trait to the creature's caste's average value (as defined in the PERSONALITY creature tokens).

Valid targets:

:citizens:
    All (sane) citizens of your fort will be affected. Will do nothing in adventure mode.
:unit <UNIT ID>:
    The given unit will be affected.

If no target is given, the provided unit can't be found, or no unit id is given with the unit
argument, the script will try and default to targeting the currently selected unit.

Other arguments:

:help:
    Shows this help page.
:list:
    Prints a list of all facets + their IDs.
:noneed:
    By default, unit's needs will be recalculated to reflect new traits after every run.
    Use this argument to disable that functionality.
:listunit:
    Prints a list of all a unit's personality traits, with their modified trait value in brackets.
