StenoTray
=========

an Autolookup tool to work alongside Plover stenography software

StenoTray is intended to help new steno users to learn how to stroke new words, without having to go to the dictionary to look them up. 

StenoTray displays a little sidebar on your screen, and as you are typing, StenoTray is constantly trying to figure out what you are attempting to spell, and will display a list of possible choices, along with the shortest way of stroking them. Therefore, if you are stuck on a word, just sound-out the first syllable, or fingerspell the first few letters, and a list of words will appear - averting the need to turn Plover off, switch to the dictionary, do a search, memorize the stroke, switch back to your document, turn Plover back on, and continue typing.

StenoTray runs alongside Plover, and works by monitoring the Plover log file.  Therefore, you must enable "Log Translations" in Plover's configuration dialog for StenoTray to work.

There are several options that can be configured in StenoTray.
PLOVER_CONFIG - the path to your plover configuration file.  This is vital if StenoTray doesn't find it automatically.
LIMIT_RESULTS - default 0.  Limit the number of results StenoTray will display at any one time.  0 means no limit.
SIMPLIFY - (true or false)  Will simplify the strokes presented.  For example, KHROUPB (clown) would become KLOUN.
FONT SIZE - alters the size of the displayed text

All of these configuration options must be put in a config file named stenotray.cfg in your plover configuration directory ({HOME}/.config/plover/stenotray.cfg).  The format is one setting per line, as follows:

OPTION_NAME = setting
