Basic versionings
0.0.1: initial release

0.0.2
- fixed issue where "?" in village name couldn't be parsed
- fixed weekly reset of topfarm data
- fine tuned weekly topfarm data visualization

0.0.3
Improvements to topfarm page
- removed zero farm per hour datapoint
- fixed issue of duplicate data when user was in top10 farmers
- added option to look back historic weekly farm data

0.0.4
Fixes:
- fixed a bug where new trade route imports added to the existing routes table instead of updating the list
- fixed a bug where barracks/stables/workshop training times were wrongly calculated with building lvls
- fixed a bug where some roman troops had wrong cost values in the csv
- fixed a bug where alliance bonus values were wrong on the alliance info page
- fixed a bug where only one trade route was added when there are multiple present
- fixed a bug where village groupings were not parsed correctly
- fixed a bug where alliance bonuses were not calculated into troop production times
- fixed a bug where after the response info of the initial parsing buttons are not visible
- fixed a bug where on the account overview page only one village was visible per village groups
- fixed a bug where parsed villages couldnt calculate party costs

Improvements:
- added a grand total "all resourses sum" number to the net production table
- added a village building and resource field parser

0.0.5
Fixes:
- fixed a bug where trade route frequency defaulted to 1 hour instead of a proper count
- fixed a bug where various troops were listed at the wrong building when setting up queues
- fixed a bug where hospital building was removed when applied template/sorting


Improvements:
- added a village templates menu where we can add, modify or delete templates. Doesnt work properly yet Delete is good.
- right side menu res field type distribution now calculated by the parsed HTML data


---------------------------------------------------------
Later releases:

Errors found:

Improvements still needed:
- add an "inactive wh/granary fill time" table. Inactive means no new queues or parties, dont count those in, but calculate with trade routes and troops present
- add a "troops in villages" page parser, calculate crop consumption per villa from that - !!!IMPORTANT!!! - multi tribe troops (+ animals) are possible, that could break shit
- add a "time until accountwide negative crop" calculation from current net production + queues
- add an option to select hero items to adjust troop production time - queue cost
- add a farmlist parser. option to select "timer" route, select troop to that, by the income estimate how many rounds we sent
- include map.sql data in the tool
- add a farm visualized map
- fix manual trade route yield calculations
- add an optimal trade route calculator with village hopping. include option to count only still available merchants