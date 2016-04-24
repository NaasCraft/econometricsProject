# Projet d'économétrie 2

_I. Haik et G. Demonet_

## Données

_blabla_

### Variables

- __Accident__ (fichier `ACCIDENT`) :

| Catégorie | Nom(s) | Page(s) | Description |
| --- | --- | --- | --- | --- |
| __Clé__ | ST_CASE | A-60 | GSA State element + assigned number |
| __Environnement__ | WEATHER | A-1 |  |
|  | CITY | A-2 |  |
|  | COUNTY | A-2 |  |
|  | LGT_COND | A-29 | Light condition |
|  | ROAD_FNC | A-49--52 | Road function class |
|  | SUR_COND | A-54 | Surface condition |
|  | SP_LIMIT | A-58 | Speed limit |
|  | STATE | A-59 |  |
| __Temps__ | YEAR | A-3 |  |
|  | MONTH | A-3 |  |
|  | DAY | A-3 |  |
|  | DAY_WEEK | A-3 | Day of the week (e.g. Monday) |
|  | HOUR, MINUTE | A-61--62 |  |
| __Description__ | HARM_EV | A-15--26 | Harmful event description |
|  | MAN_COLL | A-30--34 | Manner of collision (e.g. Front-to-Front) |
|  | PERSONS | A-38 | Number of person forms submitted |
|  | PEDS | A-36 | Number of non-motorists |
| __Conséquences__ | FATALS | A-9 | Number of fatalities |
|  | VE_FORM | A-70--71 | Number of vehicle forms submitted |
| __Facteurs__ | DRUNK_DR | A-8 | Number of drunk drivers involved in the crash |
|  | CF1, CF2, CF3 | A-40--41 | Related Factors Crash Level |

- __Véhicule__ (fichier `VEHICLE`) :

| Catégorie | Nom(s) | Page(s) | Description |
| --- | --- | --- | --- | --- |
| __Clés__ | ST_CASE | A-60 | GSA State element + assigned number |
|  | VEH_NO | V-182 | Vehicle number identifier |
| Description | BODY_TYP | V-2--10 |  |
|  | DEFORMED | V-30 | Extent of damage |
|  | MOD_YEAR | V-63 | Model year |
|  | MCYCL_DS | V-66 | Motorcycle Displacement in cc |
|  | VEH_CFi(1-2) | V-77--78 | Vehicle related factors |
|  | VIN_i(1-12) | V-95--97 | Vehicle identification number |
|  | MAKE | V-98--103 | Vehicle manufacturer |
| Contexte | DR_DRINK | V-18 | Driver drinking |
|  | DR_PRES | V-25 | Driver presence |
|  | OCCUPANTS, NUMOCCS | V-67 | Number of the individuals may have died in the crash |
|  | TRAV_SP (V-87) Travel speed estimate |
| Conducteur | DR_HGT, DR_WGT | V-19 | Driver height and weight |
|  | L_COMPL | V-20 | License compliance |
|  | CDL_STAT, L_STATUS | V-21--24 | License status |
|  | L_STATE | V-82--83 | Driver’s license state |
|  | D_VISIONi(1-3) | V-27 | Cause of vision obscured  |
|  | PREV_ACC | V-69 | Previously recorded crash |
|  | PREV_DWI | V-69 | Previously recorded driving while impaired |
|  | PREV_SPD | V-69 | Previously recorded speeding |
|  | DR_CFi(1-4) | V-71--76 | Driver related factors |
| Evènements | AVOID | V-16 | Crash avoidance maneuver |
|  | M_HARM | V-34--46 | Most harmful event (vehicle level) |
|  | VEH_MAN | V-104 | Vehicle maneuver just prior to the crash |
| Conséquences | DEATHS | V-31 | Number of fatalities in the vehicle |
|  | FIRE_EXP | V-32 | Fire occurrence |
|  | VIOLCHGi(1-3) | V-191--194 | Violations charged |

- __Individu__ (fichier `PERSON`) :

| Catégorie | Nom(s) | Page(s) | Description |
| --- | --- | --- | --- | --- |
| __Clés__ | ST_CASE | P-80 | GSA State element + assigned number |
|  | VEH_NO | P-94 | Vehicle number identifier |
| __Description__ | AGE | P-1 |  |
|  | SEX | P-77 |  |
|  | PER_NO | P-51 | Person number identifier |
|  | PER_TYP | P-52--53 |  |
|  | P_CFi(1-3) | P-56--62 | Person related factors |
|  | REST_USE | P-63 | Use of restraints |
|  | AIR_BAG | P-64 |  |
|  | AUT_REST, MAN_REST | P-65--66 | Protection system |
|  | SEAT_POS | P-74--76 | Seating position |
| __Alcool/drogues__ | ALC_STATUS | P-2 | Alcohol test status  |
|  | ALC_RES, TEST_RES | P-2--6 | Alcohol test result |
|  | DRINKING | P-3 | Alcohol involved  |
|  | DRUGRESi(1-3) | P-20--22 | Drug test results |
| __Evènements__ | EJECTION | P-23--24 |  |
|  | DEATH_DA, DEATH_MO | P-17 | Date of death (give info if not dead) |
|  | DEATH_TM | P-81 | Time of death |
|  | LAG_HRS, LAG_MINS | P-81 | Lag between crash and death |
|  | INJ_SEV | P-41 | Injury severity |
|  | HOSPITAL | P-84 | Transported for treatment |